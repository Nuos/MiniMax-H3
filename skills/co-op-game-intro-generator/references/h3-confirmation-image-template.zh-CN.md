# H3 Confirmation Image Template｜H3 确认图模板：逐段注释译本

源文件：[h3-confirmation-image-template.md](./h3-confirmation-image-template.md)。固定源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`9f12841baab1e6de990c753e9659d41efe8fb0b5`。本译本依据实际英文模板编写，与源文件并列；不覆盖源文件。单花括号变量、玩家标识和菜单文案保留原样。n. 名词；v. 动词；adj. 形容词；adv. 副词；n. phr. 名词短语；v. phr. 动词短语；abbr. 缩写。命令式句子均为所翻译的模板内容，不表示本次调用生成工具。

## 01｜Core Rule：核心规则

**词汇释义**：confirmation /ˌkɒnfəˈmeɪʃən/ n. 确认；polished /ˈpɒlɪʃt/ adj. 精修完善的；landscape /ˈlændskeɪp/ adj. 横向的；cooperative /kəʊˈɒpərətɪv/ adj. 合作式的；independent /ˌɪndɪˈpendənt/ adj. 独立的；UI abbr. User Interface，用户界面；framework /ˈfreɪmwɜːk/ n. 框架；fixed /fɪkst/ adj. 固定的；dynamic /daɪˈnæmɪk/ adj. 动态的。

**译文**：为合作游戏主菜单生成一张精修的 16:9 横向确认图。图像由两个独立系统组成：界面框架（固定）与视觉风格（动态）。

**词汇释义**：layout /ˈleɪaʊt/ n. 布局；composition /ˌkɒmpəˈzɪʃən/ n. 构图；information hierarchy /ˌɪnfəˈmeɪʃən ˈhaɪərɑːki/ n. phr. 信息层级；interaction logic /ˌɪntərˈækʃən ˈlɒdʒɪk/ n. phr. 交互逻辑；reading flow /ˈriːdɪŋ fləʊ/ n. phr. 阅读动线；readability /ˌriːdəˈbɪləti/ n. 可读性。

**译文**：界面框架规定布局、构图、信息层级、交互逻辑、阅读动线、菜单结构和可读性。这些元素必须保持不变。

**词汇释义**：artistic appearance /ɑːˈtɪstɪk əˈpɪərəns/ n. phr. 美术外观；rendering medium /ˈrendərɪŋ ˈmiːdiəm/ n. phr. 表现媒介；costume language /ˈkɒstjuːm ˈlæŋɡwɪdʒ/ n. phr. 服装设计语言；typography /taɪˈpɒɡrəfi/ n. 字体编排；motif /məʊˈtiːf/ n. 视觉母题；art direction /ɑːt dəˈrekʃən/ n. phr. 美术方向；conflict /kənˈflɪkt/ v. 冲突；prioritize /praɪˈɒrətaɪz/ v. 优先采用。

**译文**：`{visual_style}` 只控制美术外观，包括表现媒介、材质、色彩语言、光照情绪、环境风格、人物设计、服装语言、界面材质、图标语言、字体外观、装饰母题和整体氛围。改变 `{visual_style}` 应像为同一套专业设计的游戏菜单更换美术方向，绝不是重新设计界面本身。任何默认描述与 `{visual_style}` 冲突时，优先采用 `{visual_style}`，同时保留界面框架。

## 02｜Design Goal：设计目标

**词汇释义**：premium /ˈpriːmiəm/ adj. 高品质的；commercial /kəˈmɜːʃəl/ adj. 商业的；console game /ˈkɒnsəʊl ɡeɪm/ n. phr. 主机游戏；mockup /ˈmɒkʌp/ n. 设计效果稿；promotional artwork /prəˈməʊʃənəl ˈɑːtwɜːk/ n. phr. 宣传美术图；integrated /ˈɪntɪɡreɪtɪd/ adj. 融合的；interaction focus /ˌɪntərˈækʃən ˈfəʊkəs/ n. phr. 交互焦点。

**译文**：制作高品质商业主机游戏主菜单效果稿，采用 16:9 横向格式。图像应结合精修游戏宣传美术的质量与专业游戏界面的清晰性。人物和界面必须自然融合，具有鲜明视觉层级、出色可读性、干净构图和明确交互焦点。

## 03｜Overall Style：整体风格

**词汇释义**：user-selected /ˈjuːzə sɪˈlektɪd/ adj. 用户选定的；illustration /ˌɪləˈstreɪʃən/ n. 插画；palette /ˈpælət/ n. 配色；treatment /ˈtriːtmənt/ n. 处理方式；unified /ˈjuːnɪfaɪd/ adj. 统一的；incompatible /ˌɪnkəmˈpætəbəl/ adj. 不兼容的；regardless /rɪˈɡɑːdləs/ adv. 不论。

**译文**：遵循用户选定的视觉风格 `{visual_style}`。该风格控制表现媒介、插画风格、材质、配色语言、环境、人物外观、服装设计、界面外观、图标语言、字体处理、装饰元素和氛围。所有视觉元素必须属于同一套统一美术语言，不要在同一图中混合不兼容风格。不论风格如何变化，界面框架、布局、层级、构图和交互逻辑均保持一致。

## 04｜Color Palette：配色

**词汇释义**：derive /dɪˈraɪv/ v. 推导；primary /ˈpraɪməri/ adj. 主要的；functional accent /ˈfʌŋkʃənəl ˈæksent/ n. phr. 功能强调色；highlight /ˈhaɪlaɪt/ n. 高亮；warning /ˈwɔːnɪŋ/ n. 警告；border /ˈbɔːdə/ n. 边框；visual effect /ˈvɪʒuəl ɪˈfekt/ n. phr. 视觉效果；unrelated /ˌʌnrɪˈleɪtɪd/ adj. 无关的。

**译文**：根据 `{visual_style}` 推导整个色彩系统。使用 `{main_background_color}` 作为主背景色，`{ui_body_color}` 作为主要界面颜色，`{text_color}` 作为主要文字颜色，`{functional_accent_color}` 作为交互高亮色。红色仅用于警告、危险或退出动作。整体配色限制为五个主要颜色。所有按钮、玩家卡、图标、边框、高亮、装饰元素、字体和视觉效果必须遵循同一色彩系统，不引入选定配色之外的无关颜色。

## 05｜Composition：构图

**词汇释义**：playable character /ˈpleɪəbəl ˈkærəktə/ n. phr. 可操作游戏角色；surround /səˈraʊnd/ v. 环绕；block /blɒk/ v. 遮挡；decorative strip /ˈdekərətɪv strɪp/ n. phr. 装饰条；wooden plank /ˈwʊdən plæŋk/ n. phr. 木板；stone slab /stəʊn slæb/ n. phr. 石板；scroll /skrəʊl/ n. 卷轴；negative space /ˈneɡətɪv speɪs/ n. phr. 留白。

**译文**：使用固定 16:9 横向布局。将 `{character_count}` 名可操作角色放在中央，作为视觉主体。界面围绕人物而不遮挡。玩家信息卡放在左上角，主菜单竖排于右侧。底部放一条横向装饰带，自然适配 `{visual_style}`，例如丝带、警示带、木板、石板、能量条或卷轴。保持清楚的 Z 形阅读动线：玩家卡 → 人物 → 菜单 → Continue 按钮。Continue 按钮始终是主要视觉焦点。保持充足留白和出色可读性。

## 06｜Background：背景

**词汇释义**：compete /kəmˈpiːt/ v. 争夺注意；subtle texture /ˈsʌtəl ˈtekstʃə/ n. phr. 细微纹理；visual noise /ˈvɪʒuəl nɔɪz/ n. phr. 视觉噪声；dense decoration /dens ˌdekəˈreɪʃən/ n. phr. 密集装饰；scratch /skrætʃ/ n. 划痕；paint splatter /peɪnt ˈsplætə/ n. phr. 油漆泼溅；distracting /dɪˈstræktɪŋ/ adj. 分散注意的。

**译文**：生成由 `{visual_style}` 自然推导的背景。背景服务界面，而不与界面争夺注意。重要界面元素后方保持足够干净留白。只在与所选风格相符的位置使用细微纹理、环境细节和装饰母题。避免过多视觉噪声、密集装饰、厚重污垢、划痕、油漆泼溅或分散注意的纹理。整体背景应精致、高品质、现代，并适用于商业游戏菜单。

## 07｜Character Style：人物风格

**词汇释义**：body proportion /ˈbɒdi prəˈpɔːʃən/ n. phr. 身体比例；facial stylization /ˈfeɪʃəl ˌstaɪlaɪˈzeɪʃən/ n. phr. 面部风格化；lighting response /ˈlaɪtɪŋ rɪˈspɒns/ n. phr. 光照响应；identity anchor /aɪˈdentəti ˈæŋkə/ n. phr. 身份锚点；reinterpret /ˌriːɪnˈtɜːprɪt/ v. 重新诠释；override /ˌəʊvəˈraɪd/ v. 覆盖、取代。

**译文**：所有人物严格遵循 `{visual_style}`。它决定表现媒介、身体比例、面部风格化、服装语言、材质处理、光照响应、动画风格和整体人物品质。只有身份锚点和姿态固定；脸部渲染、眼睛设计、鼻部简化、嘴形、皮肤处理、表情风格和头部比例，都必须按 `{visual_style}` 重新诠释。不得以任何默认人物风格取代 `{visual_style}`。

## 08｜Character A / PLAYER 1：人物 A／玩家一

### Identity：身份

**词汇释义**：identity mapping /aɪˈdentəti ˈmæpɪŋ/ n. phr. 身份映射；donate /dəʊˈneɪt/ v. 此处指提供；recognizable /ˈrekəɡnaɪzəbəl/ adj. 可辨识的；face silhouette /feɪs ˌsɪluˈet/ n. phr. 面部轮廓；distinctive trait /dɪˈstɪŋktɪv treɪt/ n. phr. 独特特征；photographic realism /ˌfəʊtəˈɡræfɪk ˈrɪəlɪzəm/ n. phr. 摄影写实性；swap /swɒp/ v. 对调。

**译文**：人物参考图 1 仅用于身份映射。它只提供身份锚点：可辨识的脸部轮廓、发型、眼镜（有时）、相对五官比例和独特个人特征；不提供摄影写实性、真实皮肤纹理、现实光照、相机画质或原图风格。不要丢失人物身份锚点，但须把面孔重新设计为 `{visual_style}`。全部脸部渲染、眼睛设计、鼻部简化、嘴形、皮肤处理、表情风格与头部比例均遵循 `{visual_style}`。不要与其他人物交换身份。

### Appearance：外观

**词汇释义**：appearance /əˈpɪərəns/ n. 外观；outfit /ˈaʊtfɪt/ n. 服装；accessory /əkˈsesəri/ n. 配饰；silhouette /ˌsɪluˈet/ n. 轮廓。

**译文**：人物渲染、表情、服装、材质与配饰完全由 `{visual_style}` 推导，同时保持可辨识的可操作游戏角色轮廓。

### Action：动作

**词汇释义**：cross-legged /ˌkrɒsˈleɡd/ adj. 盘腿的；support /səˈpɔːt/ v. 支撑；upper body /ˈʌpə ˈbɒdi/ n. phr. 上半身；lean backward /liːn ˈbækwəd/ v. phr. 后倾；upward /ˈʌpwəd/ adv. 向上。

**译文**：人物 A 盘腿坐在地上，双手撑地支撑身体，上半身略微后倾，向上看摄影机。

## 09｜Character B / PLAYER 2：人物 B／玩家二

### Identity：身份

**词汇释义**：reference image /ˈrefərəns ˈɪmɪdʒ/ n. phr. 参考图；relative facial proportion /ˈrelətɪv ˈfeɪʃəl prəˈpɔːʃən/ n. phr. 相对五官比例；skin treatment /skɪn ˈtriːtmənt/ n. phr. 皮肤处理；head proportion /hed prəˈpɔːʃən/ n. phr. 头部比例；redesign /ˌriːdɪˈzaɪn/ v. 重新设计。

**译文**：人物参考图 2 仅用于身份映射。它只提供身份锚点：可辨识脸部轮廓、发型、眼镜（有时）、相对五官比例和独特个人特征；不提供摄影写实性、真实皮肤纹理、现实光照、相机画质或原图风格。不要丢失人物身份锚点，但须把面孔重新设计为 `{visual_style}`。全部脸部渲染、眼睛设计、鼻部简化、嘴形、皮肤处理、表情风格和头部比例均遵循 `{visual_style}`。不要与其他人物交换身份。

### Appearance：外观

**词汇释义**：rendering /ˈrendərɪŋ/ n. 渲染；expression /ɪkˈspreʃən/ n. 表情；material /məˈtɪəriəl/ n. 材质；recognizable /ˈrekəɡnaɪzəbəl/ adj. 可辨识的。

**译文**：人物渲染、表情、服装、材质与配饰完全由 `{visual_style}` 推导，同时保持可辨识的可操作游戏角色轮廓。

### Action：动作

**词汇释义**：rest /rest/ v. 自然放置；cross-legged /ˌkrɒsˈleɡd/ adj. 盘腿的；lean forward /liːn ˈfɔːwəd/ v. phr. 前倾；directly /dəˈrektli/ adv. 直接地。

**译文**：人物 B 盘腿坐在地上，双手自然放在腿前，上半身略微前倾，直接看向摄影机。

## 10｜Lighting：光照

**词汇释义**：primary top light /ˈpraɪməri tɒp laɪt/ n. phr. 顶部主光；secondary fill light /ˈsekəndəri fɪl laɪt/ n. phr. 辅助补光；ambient bounce /ˈæmbiənt baʊns/ n. phr. 环境反射光；contact shadow /ˈkɒntækt ˈʃædəʊ/ n. phr. 接触阴影；rim lighting /rɪm ˈlaɪtɪŋ/ n. phr. 轮廓光；global illumination /ˈɡləʊbəl ɪˌluːmɪˈneɪʃən/ n. phr. 全局光照；separation /ˌsepəˈreɪʃən/ n. 分离度。

**译文**：光照遵循 `{visual_style}`，同时保持清楚可读。适当时使用顶部主光、辅助补光、柔和环境反射、接触阴影、轻柔轮廓光和高品质全局光照。面孔保持清楚可见。人物自然融入环境，同时与背景保持鲜明分离。

## 11｜Game UI：游戏界面

**词汇释义**：information architecture /ˌɪnfəˈmeɪʃən ˈɑːkɪtektʃə/ n. phr. 信息架构；surface texture /ˈsɜːfɪs ˈtekstʃə/ n. phr. 表面纹理；border treatment /ˈbɔːdə ˈtriːtmənt/ n. phr. 边框处理；corner shape /ˈkɔːnə ʃeɪp/ n. phr. 边角形状；interaction effect /ˌɪntərˈækʃən ɪˈfekt/ n. phr. 交互效果；assembled /əˈsembəld/ adj. 拼装的。

**译文**：创建专业商业主机游戏主菜单。菜单结构、交互层级、间距、构图、阅读动线和信息架构保持固定。`{visual_style}` 只改变界面美术外观。

**译文**：所选风格可以影响界面材质、表面纹理、边框处理、边角形状、装饰母题、色彩表现、光照处理、图标语言、字体外观和交互效果；绝不能改变菜单层级、按钮顺序、按钮位置、玩家卡位置、构图、交互逻辑、信息架构和可读性。整个界面应像一套专业设计的游戏界面系统，而非各自分离元素的拼装。

## 12｜UI Visual Language：界面视觉语言

**词汇释义**：panel /ˈpænəl/ n. 面板；edge treatment /edʒ ˈtriːtmənt/ n. phr. 边缘处理；visual weight /ˈvɪʒuəl weɪt/ n. phr. 视觉分量；feedback /ˈfiːdbæk/ n. 反馈；leather /ˈleðə/ n. 皮革；hologram /ˈhɒləɡræm/ n. 全息影像；ceramic /səˈræmɪk/ n. 陶瓷；carved /kɑːvd/ adj. 雕刻的；watercolor paper /ˈwɔːtəkʌlə ˈpeɪpə/ n. phr. 水彩纸。

**译文**：由 `{visual_style}` 推导完整界面外观。它决定按钮材质、边框语言、面板材质、装饰细节、边缘处理、视觉分量、高亮风格、交互反馈、阴影处理和纹理语言。可用材质包括木、石、纸、皮革、布、玻璃、水晶、全息影像、霓虹、金属、陶瓷、雕刻表面、彩绘表面、魔法能量、像素块、水彩纸、笔墨、漫画图形，以及任何自然属于 `{visual_style}` 的其他材质。全部界面元素共用同一材质语言与美术风格。

## 13｜Button Layout Rules：按钮布局规则

**词汇释义**：vertical rhythm /ˈvɜːtɪkəl ˈrɪðəm/ n. phr. 竖向排列节奏；design family /dɪˈzaɪn ˈfæməli/ n. phr. 同一设计系列；adapt /əˈdæpt/ v. 适应；single line /ˈsɪŋɡəl laɪn/ n. phr. 单行；wrapping /ˈræpɪŋ/ n. 自动换行；stacked text /stækt tekst/ n. phr. 堆叠文字；padding /ˈpædɪŋ/ n. 内边距；clutter /ˈklʌtə/ n. 杂乱。

**译文**：所有菜单按钮竖排在右侧，保持一致的竖向节奏。各按钮属于同一设计系列。按钮宽度自动适应文字长度，全部菜单标题单行显示；禁止自动换行、禁止堆叠文字。文字水平居中，内边距一致，按钮之间等距，避免视觉杂乱。

## 14｜Continue Button：继续按钮

**词汇释义**：dominant /ˈdɒmɪnənt/ adj. 占主导的；emphasis /ˈemfəsɪs/ n. 强调；distinctive /dɪˈstɪŋktɪv/ adj. 独特的；engraving /ɪnˈɡreɪvɪŋ/ n. 刻纹；holographic /ˌhɒləˈɡræfɪk/ adj. 全息的；embossed /ɪmˈbɒst/ adj. 浮雕压纹的；animated cue /ˈænɪmeɪtɪd kjuː/ n. phr. 动态提示。

**译文**：Continue 按钮始终是主要视觉焦点。使用自然属于 `{visual_style}` 的强调方式使其突出，例如尺寸更大、对比更强、颜色更亮、独特材质、特殊边框、照明、辉光、刻纹、魔法能量、全息效果、浮雕边框或动态视觉提示。如果辉光或霓虹与 `{visual_style}` 冲突，不要强行使用。Continue 按钮应立即吸引玩家注意。

## 15｜Start New Game Button：开始新游戏按钮

**词汇释义**：secondary button /ˈsekəndəri ˈbʌtən/ n. phr. 次级按钮；appearance /əˈpɪərəns/ n. 外观；style-appropriate /staɪl əˈprəʊpriət/ adj. 与风格相符的；single-line text /ˈsɪŋɡəl laɪn tekst/ n. phr. 单行文字。

**译文**：放在 Continue 上方。使用标准次级按钮外观，视觉语言与选定风格一致；合适时加一个小型、符合风格的图标。保持单行文字。

## 16｜Settings Button：设置按钮

**词汇释义**：settings /ˈsetɪŋz/ n. 设置；icon /ˈaɪkɒn/ n. 图标；proportion /prəˈpɔːʃən/ n. 比例；spacing /ˈspeɪsɪŋ/ n. 间距；hierarchy /ˈhaɪərɑːki/ n. 层级。

**译文**：使用标准次级按钮外观，并采用一个由 `{visual_style}` 自然推导的设置图标。保持比例、间距和层级一致。

## 17｜Exit Game Button：退出游戏按钮

**词汇释义**：danger indicator /ˈdeɪndʒə ˈɪndɪkeɪtə/ n. phr. 危险指示；accent /ˈæksent/ n. 强调；dominant color /ˈdɒmɪnənt ˈkʌlə/ n. phr. 主导颜色；exit /ˈeksɪt/ n. 退出。

**译文**：使用标准次级按钮外观。红色只作为危险指示，应是强调色而不是主导色。适合时添加一个风格相符的退出图标。

## 18｜Player Cards：玩家卡片

**词汇释义**：nickname /ˈnɪkneɪm/ n. 昵称；status /ˈsteɪtəs/ n. 状态；READY /ˈredi/ adj. 已准备好；automatically /ˌɔːtəˈmætɪkli/ adv. 自动地；visually connected /ˈvɪʒuəli kəˈnektɪd/ phr. 在视觉上相连。

**译文**：在左上角为 `{character_count}` 位玩家建立信息系统。外观遵循 `{visual_style}`，卡片材质、边框、边角、纹理、阴影、装饰和图标都由所选风格推导。每卡包含玩家标签、玩家昵称和 READY 状态。名称对应为 `PLAYER 1`／`{player1_name}`，`PLAYER 2`／`{player2_name}`。READY 始终使用功能强调色。卡片保持高度可读，并在视觉上与其余界面相连。

## 19｜Icon System：图标系统

**词汇释义**：outline /ˈaʊtlaɪn/ n. 轮廓；solid filled /ˈsɒlɪd fɪld/ adj. 实心填充的；geometric /ˌdʒiːəˈmetrɪk/ adj. 几何的；engraved /ɪnˈɡreɪvd/ adj. 阴刻的；rune /ruːn/ n. 符文；glyph /ɡlɪf/ n. 字形符号；origami /ˌɒrɪˈɡɑːmi/ n. 折纸；embossed /ɪmˈbɒst/ adj. 凸纹的；low-poly /ləʊ ˈpɒli/ adj. 低多边形的。

**译文**：由 `{visual_style}` 推导全部图标，整个界面使用同一个图标系列。可采用的图标语言包括：极简描边、实心填充、几何、漫画、像素、阴刻、雕刻、彩绘、笔刷、符文、字形符号、全息、水晶、剪纸、折纸、浮雕压纹、低多边形、扁平设计或风格化三维。

**词汇释义**：perspective /pəˈspektɪv/ n. 透视；stroke language /strəʊk ˈlæŋɡwɪdʒ/ n. phr. 笔画语言；color hierarchy /ˈkʌlə ˈhaɪərɑːki/ n. phr. 色彩层级；recognizable /ˈrekəɡnaɪzəbəl/ adj. 可辨识的；functional /ˈfʌŋkʃənəl/ adj. 具有功能的；vertical stacking /ˈvɜːtɪkəl ˈstækɪŋ/ n. phr. 竖向堆叠。

**译文**：所有图标共用相同美术风格、材质语言、透视、光照处理、笔画语言和色彩层级。图标应简洁、可辨识、有功能。每个界面区块最多包含一行水平图标；不换行、不竖向堆叠。图标应服务界面，而非主导界面。

## 20｜Typography：字体编排

**词汇释义**：font family /fɒnt ˈfæməli/ n. phr. 字体家族；decorative treatment /ˈdekərətɪv ˈtriːtmənt/ n. phr. 装饰处理；wear pattern /weə ˈpætən/ n. phr. 磨损纹样；contrast /ˈkɒntrɑːst/ n. 对比；wrap /ræp/ v. 换行。

**译文**：字体层级保持固定，字体外观遵循 `{visual_style}`。风格控制字体家族、装饰处理、纹理、材质、描边、光照、阴影及磨损纹样。保持出色可读性、鲜明视觉层级、单行菜单按钮、一致间距和高对比。按钮宽度始终适应文字长度，绝不让菜单标题换成多行。

## 21｜Game Title：游戏标题

**词汇释义**：branding element /ˈbrændɪŋ ˈelɪmənt/ n. phr. 品牌识别元素；imitate /ˈɪmɪteɪt/ v. 模仿；original /əˈrɪdʒənəl/ adj. 原创的；title treatment /ˈtaɪtəl ˈtriːtmənt/ n. phr. 标题视觉处理；meaningless /ˈmiːnɪŋləs/ adj. 无意义的。

**译文**：显示游戏标题 `{game_title}`。它应成为菜单主要的品牌识别元素，材质、装饰风格、字体和渲染均遵循 `{visual_style}`。避免模仿现有商业游戏标志；按选定风格创作原创标题设计。标题保持高度可读，不添加随机符号或无意义字母。

## 22｜Interaction States：交互状态

**词汇释义**：active /ˈæktɪv/ adj. 处于活动状态的；hover /ˈhɒvə/ n. 悬停；pressed state /prest steɪt/ n. phr. 按下状态；pulse /pʌls/ n. 脉冲；illumination /ɪˌluːmɪˈneɪʃən/ n. 照明；ink spread /ɪŋk spred/ n. phr. 墨色扩散；brush bloom /brʌʃ bluːm/ n. phr. 笔触晕开；emboss /ɪmˈbɒs/ n. 压纹效果；flashing /ˈflæʃɪŋ/ n. 闪烁。

**译文**：把界面表现为处于活动状态的游戏菜单。按钮可显示自然属于 `{visual_style}` 的适当交互反馈，例如悬停、按下状态、魔法辉光、能量脉冲、全息高亮、刻纹发光、墨色扩散、笔触晕开、金属反射、纸张压纹、动态边框或像素闪烁。只用与选定风格自然相符的效果，不把现代界面特效强加到不兼容的美术风格中。

## 23｜Rendering：渲染

**词汇释义**：AAA-quality /ˌtrɪpəl ˈeɪ ˈkwɒləti/ adj. 3A 级品质的；cohesive /kəʊˈhiːsɪv/ adj. 协调统一的；production /prəˈdʌkʃən/ n. 制作成品；presentation /ˌprezənˈteɪʃən/ n. 呈现；balanced /ˈbælənst/ adj. 均衡的；finish /ˈfɪnɪʃ/ n. 成品观感。

**译文**：生成精修的 3A 级商业游戏菜单美术图。人物、环境、界面、字体、图标和装饰元素应像同一个协调统一的制作成品。保持高品质渲染、鲜明视觉层级、专业商业呈现、高可读性、均衡构图和干净成品观感。

## 24｜Negative Constraints：负面限制

**词汇释义**：split screen /splɪt skriːn/ n. phr. 分屏；duplicated /ˈdjuːplɪkeɪtɪd/ adj. 重复的；identity swap /aɪˈdentəti swɒp/ n. phr. 身份对调；photorealistic /ˌfəʊtəʊrɪəˈlɪstɪk/ adj. 照片级写实的；pasted /ˈpeɪstɪd/ adj. 粘贴的；distorted /dɪˈstɔːtɪd/ adj. 变形的；overlapping /ˌəʊvəˈlæpɪŋ/ adj. 重叠的；watermark /ˈwɔːtəmɑːk/ n. 水印；overwhelming /ˌəʊvəˈwelmɪŋ/ adj. 喧宾夺主的。

**译文**：不要分屏；不要重复人物；不要身份对调；不要丢失身份锚点。除非 `{visual_style}` 明确要求照片级写实，否则不要写实面孔；不要把真实照片脸贴到风格化身体上；不要脸部风格不匹配。不要改变发型；不要不可读界面、变形按钮、重叠界面、随机文字、随机符号、水印、复制的游戏标志、品牌化界面、不一致图标风格、混杂界面材质、过多装饰、喧宾夺主的背景、视觉杂乱、破坏的布局或低可读性。

## 25｜Medium Lock：表现媒介锁定

**词汇释义**：medium /ˈmiːdiəm/ n. 表现媒介；key art /kiː ɑːt/ n. phr. 核心宣传美术图；mockup /ˈmɒkʌp/ n. 设计效果稿；artistic appearance /ɑːˈtɪstɪk əˈpɪərəns/ n. phr. 美术外观。

**译文**：呈现为精修商业游戏核心宣传美术与专业主机游戏主菜单效果稿的结合。界面保持固定，仅美术外观随 `{visual_style}` 改变。

---

**校对说明**：本源文件是英文模板，使用 `{visual_style}` 等单花括号变量；不存在 `{{STYLE_NAME}}` 一类双花括号变量。本译本没有把它改写为另一份中文框架。此模板允许随风格改变字体和界面材质，而同目录主 Skill 某些段落更倾向固定粗无衬线与贴纸语言；这是源文件之间的适配张力，不能通过翻译悄悄删掉任一要求。实际执行需单独协调，翻译本身不作规则改造。
