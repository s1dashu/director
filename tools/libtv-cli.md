# LibTV CLI 执行路径

## 支持状态

LibTV CLI 是本 skill 当前唯一正式维护、实际验证最充分的图片、音频和视频生成路径。当用户没有指定工具且本地没有可用的多模态 CLI 时，优先建议安装 LibTV CLI；不未经用户同意擅自安装。

## 执行前置条件

1. 确认 `libtv` 已安装且可执行。
2. 确认已登录。
3. 确认当前工作区与画布绑定正确。
4. 解析并记录目标 `projectUuid`。
5. 实时查询目标模型、schema、输入模式、素材数量、文件格式、时长、画幅、分辨率和声音能力。

缺少任一前置条件时明确报错并停止，不静默切换其他工具。

## 模型与参数

- 仅在 LibTV 中，将 `GPT-Image-2` 解析为 `Lib Image`、`Nano Banana Pro` 解析为 `General image Pro`、`Nano Banana 2` 解析为 `General image V2`；其他 CLI 不得沿用这些别名。Midjourney 不再假定映射为 `悠船`，每次必须实时搜索。2026-08-09 实测当前图片模型列表不再提供 `悠船`、`Midjourney` 或历史 `mj-v8.2`，因此不可新建 Midjourney 节点；旧画布中保存的 `mj-v8.2` 参数只作为历史记录，不得绕过现行 schema 强行复用。平台重新返回可解析的 Midjourney `modelName` 与完整 schema 后，才能恢复调用。
- 给 `libtv node ... -s "model=..."` 传模型时，逐字使用 `libtv model search` 返回的 `matches[].modelName`，包括空格、大小写与标点；不改用 `modelKey`。
- 当前已验证的 Seedance 默认选择是 Seedance 2.0 Pro；LibTV 中对应 Seedance 2.0 VIP（`star-video2`）。正式调用仍以实时搜索与 schema 为准。
- 每次创建或重生成节点都显式传入实际 `duration`、`ratio`、`resolution`、`enableSound`、`count` 和 `modeType`，不继承旧画布、复制节点或模型默认值。
- 使用 Seedance 2.0 系列时，用户未明确要求高分辨率则显式使用 `720p`。用户要求 `1080p`、`4K` 或其他档位时，先以实时 schema 确认支持；不支持时停止，不静默降级。
- 时长、画幅、分辨率、声音开关、数量和 `modeType` 只通过 CLI 参数传递，不写进创作 Prompt。

## 参考素材与音色

- 平台内部的素材上传、节点连接、任务运行与生成结果下载全部通过官方 `libtv` 命令完成，不自行构造 HTTP 请求。
- LibTV 节点只在所属画布内有效。跨画布复用时，先通过 CLI 下载标准化本地文件，再通过 CLI 上传到目标画布。
- 音频只承担音色参考时，即使只连接一份音频，也一般显式使用实时 schema 支持的 `mixed2video`，不仅因只有音频就改用 `audio2video`。
- 平台要求有效视觉输入时，只连接当前片段真实需要的人物或视频参考，不为通过校验接入无关素材。

### LibTV 音色能力边界

- 正式生成前分别查询音频模型与目标视频模型的实时 schema。LibTV 的音频节点可以先生成一段固定音色的语音，再作为上游音频节点连接到 Seedance；这与 Seedance 视频节点“直接选择平台音色 ID”是两回事。
- 2026-08-09 使用 LibTV CLI 1.1.1 与 1.1.3 查询：`Minimax-speech-2.8-hd` 与 `Minimax-speech-2.8-turbo` 暴露 `voiceCard`、语速、声调、音量和音色调节参数，schema 默认卡为“少女音色”（`voiceId=female-shaonv`）并带预览 URL；这只证明平台 schema 声明了能力，不证明 CLI 已把指定参数正确提交给模型。
- 当前上述模型的 `config.advancedSettings` 是包含 `groupKey` 与 `fields` 的分组对象数组。CLI 1.1.1 和 1.1.3 会把这些对象错误解析成 `[object Object]`，拒绝写入正确嵌套字段；把 `voiceCard`、`voice_setting_voice_id` 或调节参数写到 `params` 顶层虽然可能成功建节点，节点回读仍显示 `advancedSettings:{}`，不得运行或宣称指定 voice ID 生效。必须等 CLI 修复后先创建不运行节点，并回读确认真实 `originalField` 已进入 `params.advancedSettings`，才允许生成候选。
- 同次查询中，CLI schema 只返回默认 `voiceCard`，没有返回可枚举的完整音色列表；LibTV CLI 也没有独立的 voice catalog 命令。在 CLI 能稳定枚举并解析完整 `voiceId` 之前，不得声称可以从命令行任意浏览或选择 LibTV 的全部平台音色，也不得猜测未返回的音色 ID。
- Seedance 2.0 VIP（`star-video2`）视频 schema 没有直接的 `voiceId` 或 `voiceCard` 参数。固定角色声音必须通过已确认音频参考节点传入，或仅靠 Prompt 新建声音后再建立音频锚点；不能把 Minimax 的音色 ID 直接写进 Seedance 参数。
- 2026-08-09 的 `star-video2` 实时 schema：`mixed2video` 总媒体输入 1–15 个，最多 9 张图片、3 条视频、3 条音频。角色音色与人物、场景、武魂等视觉参考共同输入时使用 `mixed2video`；超过 3 个独立说话角色音色时优先拆分片段。
- 可选路线按可靠性排序：优先上传 director 已登记且用户确认的标准化 WAV；其次为当前作品独立生成并确认的角色音色锚点；LibTV TTS 内置音色只有在 CLI 返回明确 `voiceId`、成功生成候选且用户听审确认后，才可登记为该角色的项目音色。

## 可追溯性与落盘

- 解析画布后，正式创建节点、生成、上传和下载命令都显式传入 `-p <projectUuid>`。
- 每次命令返回后核对实际 `projectUuid`、节点 ID、任务 ID、终态和资源 URL，并保留 stderr 与失败状态。
- 当前作品的独立视频片段和最终成片统一下载到 `<作品目录>/video/`，文件直接平铺并用补零编号排序，例如 `片段01.mp4`、`片段02.mp4`。
- 任一任务未返回成功终态，或节点 ID、任务 ID、资源 URL 缺失时，停止后续批量生成或拼接。
