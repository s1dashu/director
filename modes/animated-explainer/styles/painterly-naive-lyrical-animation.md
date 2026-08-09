# 朴拙绘画感抒情动画

## 风格定位

以极端简化的人物、大块不透明手绘色面和受控的朴拙变形来组织画面。它不是在写实插画上叠加水粉纹理，而是主动删去绝大多数结构与细节，只保留辨认人物、动作、物体和空间所需的最少形状。人物近乎由几个钝拙色块拼成，环境也以概括形状而不是精细描绘成立；情绪主要来自姿态、尺度、距离、遮挡和空间包围，而不是五官刻画。整体应当亲密、内省、温柔而略带忧郁，同时保持当代感、清洁度和清楚的叙事层级。

## 稳定的视觉语言

- **先删细节，再以色面造型。** 把每个人物、物体与空间部分压缩成尽可能少的宽阔、不透明、哑光色块。先删除写实结构、内部纹理和装饰，再判断是否仍然能够辨认；只有影响叙事理解时才恢复一个细节。轮廓主要由相邻色面形成，只允许极少量松动笔触帮助辨认。
- **保留真实的绘画触感。** 色面内部允许看见轻微刷痕、颜料拖曳、覆盖差异、干涩边缘与纸面阻力；边缘柔钝、略有偏移，不机械光滑。纹理必须依附于绘画过程，不能变成脏污、仿古裂纹、满页噪点或装饰性做旧。
- **受控的朴拙变形。** 物体像从观察与记忆中画出，而不是用尺规或三维建模搭建。透视可以压扁、倾斜、正面化或轻微错位，比例可以为情绪和构图让步，但空间关系、人物动作与物体用途仍须一眼可懂。
- **人物必须超级简单。** 头部、头发、躯干和四肢分别作为少数钝拙形状处理，允许头身、手脚和关节被大胆压缩、放大或省略。脸不能成为视觉中心：眼睛只是小点或短笔，鼻子是一块或一笔，嘴巴是一条短痕；不画虹膜、眼睑、嘴唇体积、皮肤明暗、发丝、衣褶、纽扣、独立手指或解剖结构。人物要像凭记忆直接画出的形象，而不是完成度很高的人像插画。
- **让空间承担心理。** 通过人物与环境的尺度差、空旷或拥挤、被家具和建筑包围、偏离画面重心、相互靠近或隔开来表达脆弱、犹疑、孤独、安慰或压迫。表演保持安静，情绪先落在身体重量、肩背、手的位置、视线和停顿上。
- **使用关系性色彩。** 配色随题材自由变化，不固定任何色相。先建立一个统领气氛的主色域或压缩的综合色调，再以明度、冷暖或饱和度差异分出主体、空间层次和少量视觉重音。色彩应浓郁而哑光、统一而不浑浊，避免糖果式平均分色。
- **不规则但经过构图。** 允许形体歪斜、色面不对称和局部裁切，但视觉重心、叙事焦点与观看路径必须明确。构图根据当前内容决定，可以亲密、开阔、拥挤、正面或斜向，不能复制某一种固定房间、固定人物位置或固定元素数量。

## 通用风格 Prompt

先准确写清当前场景、人物、动作、关系、空间状态和可见结果，再追加以下风格段；方括号内容必须按当前作品替换。

```text
[CURRENT CONCRETE SCENE, CHARACTERS, ACTIONS, RELATIONSHIPS, SPATIAL CONDITIONS, AND VISIBLE OUTCOME]. Radically simplified painterly-naive 2D lyrical animation. Abstraction and shape reduction take priority over likeness, anatomy and illustrative detail. Reduce every person, animal, object and environmental feature to the fewest broad, blunt, irregular color masses needed for recognition; remove all nonessential internal description. Build the image directly with opaque matte gouache- and tempera-like shapes rather than drawing accurate forms and coloring them in. Human figures are primitive, weighty and deliberately awkward: a simple head mass, one hair mass, a block-like torso and abbreviated limbs with bold intuitive proportion distortion. Faces contain only tiny dot or dash eyes, one crude nose shape and a short mouth mark. Do not render irises, eyelids, lips, cheek modeling, skin shading, individual hair strands, fabric folds, buttons, separate fingers, musculature or realistic anatomy. Treat clothing as one or two uninterrupted painted masses and treat animals through a simple silhouette rather than fur detail. Simplify furniture, architecture and landscape into flattened, tilted, gently compressed planes with no measured perspective and almost no small descriptive marks. Let contours emerge where adjacent color fields meet; use only a few loose dark strokes where an action would otherwise become unclear. Preserve broad brush drag, uneven pigment coverage, softened or dry edges, slight overpainting and gentle surface tooth, tactile but clean. Let emotion arise through posture, bodily weight, gaze direction, scale, spacing, enclosure, overlap and the pressure of surrounding shapes, never through a detailed face. Choose an adaptable relational palette for the actual subject: one coherent atmospheric color field, forms separated through intentional value, temperature and saturation relationships, and contrast reserved for the narrative focus without prescribing fixed hues. Compose every scene for its own content, with a clear emotional center and purposeful mass distribution. The result feels extremely simple, abstract, hand-painted, intimate, psychologically observant, contemporary, quietly lyrical and gently melancholic; childlike in directness but sophisticated in composition. No polished narrative illustration, no portrait rendering, no facial realism, no detailed eyes, no hair strands, no clothing detail, no individual fingers, no realistic fur, no clean vector geometry, no uniform ink outline, no corporate explainer look, no anime or chibi conventions, no photorealism, no glossy 3D, no precise academic anatomy, no rigid linear perspective, no dense cross-hatching, no vintage-paper stains, no grunge overlay, no decorative clutter, no literal mood icons, no random text, no logo, no watermark.
```

## 撰写图像 Prompt

- 先描述一个可以被画出来的具体处境，再决定哪几块形状构成主体、环境和心理压力；不要只写抽象情绪词。
- 明确人物的身体重量、手的位置、视线、与他人或环境的距离，以及环境如何围住、托住、压缩或释放人物；不要描述眼睛颜色、皱纹、发型细节、服装结构和其他会诱导写实刻画的信息。
- 人物身份优先通过整体轮廓、一个最必要的识别特征、姿态和上下文表达；不要罗列人物相貌。一个识别特征已经足够时，其他特征全部删除。
- 描述最重要的综合色调和对比关系即可，不枚举固定色卡。题材需要明亮、温暖、高饱和或低饱和时都可以变化，只要色彩仍作为统一的情绪结构工作。
- 复杂场景可以拥有丰富元素，但每个元素都要参与叙事、空间或色面节奏；简洁场景也不能退化为人物站在空白背景上的通用插图。

## 撰写视频 Prompt

- 运动延续绘画媒介：使用克制的逐帧重画、边缘轻微沸腾、颜料形状的细小位移和分层视差，让画面有生命但不持续抖动。
- 角色表演以身体重心转移、迟疑、停顿、视线、手部小动作和人与空间的接触为主。需要强烈事件时可以大幅运动，但动作仍由清楚的起点、受力、反应和终点构成。
- 镜头运动应服务于尺度与空间关系，例如缓慢靠近暴露人物的脆弱、拉远显示包围或隔离、横移揭示人物之间的距离。不要为了“艺术感”无目的漂移。
- 切镜后继续保持综合色调、颜料质感、人物造型原则与心理空间逻辑；不要求每镜复刻同一种构图或静态忧郁姿势。

## 明确排除

- 不把朴拙误写成儿童乱画、低完成度草稿、错误肢体或无法辨认的空间。
- 不生成“写实比例和细致五官，只是表面带水粉刷痕”的传统叙事插画；这正是该风格的主要失败类型。
- 不把手绘感误写成统一黑线加平涂，也不使用精确矢量曲线、塑料般光滑色块或三维体积渲染。
- 不依赖固定房间、固定人物、固定配色、固定构图、固定元素数量或固定题材来维持风格。
- 不用仿古纸、污渍、划痕、密集排线和颗粒滤镜堆砌“传统感”；画面应有材料性，但仍清新、克制并适合当代影像。
