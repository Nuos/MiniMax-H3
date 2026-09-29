# Co-op Game Intro Generator｜双人合作游戏开场生成器：逐段注释译本

源文件：[SKILL.md](./SKILL.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`3b10d360e35b8a9be6b7233df0273107f9342849`。本文件独立新增，不覆盖原文件或已有 `SKILL.cn.md`。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语；abbr. 缩写。所有生成规则仅作翻译，本轮未调用图像或视频生成。

## 01｜名称与描述

**词汇释义**：co-op /ˈkəʊɒp/ adj. 合作式的；intro /ˈɪntrəʊ/ n. 开场；two-player /tuː ˈpleɪə/ adj. 双人的；menu /ˈmenjuː/ n. 菜单；identity cue /aɪˈdentəti kjuː/ n. phr. 身份线索；approval image /əˈpruːvəl ˈɪmɪdʒ/ n. phr. 供确认的图像；framework /ˈfreɪmwɜːk/ n. 框架；coordinated /kəʊˈɔːdɪneɪtɪd/ adj. 协调一致的；typography /taɪˈpɒɡrəfi/ n. 字体编排；UI abbr. User Interface，用户界面；copy /ˈkɒpi/ n. 文案；event timing /ɪˈvent ˈtaɪmɪŋ/ n. phr. 事件时序；replication /ˌreplɪˈkeɪʃən/ n. 精确复制。

**译文**：名称为 `co-op-game-intro-generator`。面向制作双人合作游戏菜单或开场动画的用户。用户提供两位玩家名称、游戏标题、目标视觉风格和可选人物参考图。Skill 锁定身份线索，在固定菜单框架中生成供确认的图像，使颜色、按钮、图标和字体编排协调；然后以已确认图像为基础，重新组织最终视频的人物、界面文案和事件时间指令。输出包含两个人物、玩家卡片与菜单交互动效的合作游戏开场。最适合游戏概念、人物主导菜单和社交内容；不适用于可玩游戏开发、复杂多页面界面、真实品牌标志的精确复制或没有人物的通用标题序列。

## 02｜兼容性

**词汇释义**：require /rɪˈkwaɪə/ v. 需要；canvas workspace /ˈkænvəs ˈwɜːkspeɪs/ n. phr. 画布工作区；portable /ˈpɔːtəbəl/ adj. 可移植的；agent harness /ˈeɪdʒənt ˈhɑːnɪs/ n. phr. 智能体运行框架。

**译文**：需要 MiniMax Hub 智能体，包括画布工作区和 MiniMax H3 生成；不能直接移植到通用智能体框架。

## 03｜确认图优先的流程

**词汇释义**：visual direction /ˈvɪʒuəl dəˈrekʃən/ n. phr. 视觉方向；collect /kəˈlekt/ v. 收集；reference /ˈrefərəns/ n. 参考；framework-preserving /ˈfreɪmwɜːk prɪˈzɜːvɪŋ/ adj. 保留框架的。

**译文**：用户想制作合作游戏开场视频，并希望先用一张图确认视觉方向、再生成最终 H3 视频时使用。工作流采集风格、玩家名、游戏标题及可选人物参考，然后先创建保留框架的确认图，再生成 H3 视频。

## Required References｜必需参考文件

### 04｜模板不是可有可无的背景

**词汇释义**：mandatory runtime input /ˈmændətəri ˈrʌntaɪm ˈɪnpʊt/ n. phr. 必需执行输入；optional /ˈɒpʃənəl/ adj. 可选的；background note /ˈbækɡraʊnd nəʊt/ n. phr. 背景说明。

**译文**：以下两份模板是运行时必需输入，不是可选背景说明。

### 05｜确认图模板

**词汇释义**：fill /fɪl/ v. 填充；field /fiːld/ n. 字段；palette /ˈpælət/ n. 配色；layout /ˈleɪaʊt/ n. 布局；negative constraint /ˈneɡətɪv kənˈstreɪnt/ n. phr. 负面限制。

**译文**：步骤 3 构建确认图提示词、步骤 4 生成首张确认图时，使用 `references/h3-confirmation-image-template.md`。按顺序填充字段，不跳过框架、配色、界面、人物、字体、布局或负面限制字段。

### 06｜视频模板与缺失处理

**词汇释义**：refill /ˌriːˈfɪl/ v. 重新填充；motion direction /ˈməʊʃən dəˈrekʃən/ n. phr. 运动方向；unavailable /ˌʌnəˈveɪləbəl/ adj. 不可用的；incomplete /ˌɪnkəmˈpliːt/ adj. 不完整的；improvise /ˈɪmprəvaɪz/ v. 临时自行编造。

**译文**：步骤 6 重新填充最终 MiniMax H3 视频提示词时，使用 `references/h3-video-prompt-template.md`。按已确认图、玩家与游戏数据、最终界面文字、事件时序、运动方向及负面限制填充。任何模板不可用时，停止并报告 Skill 包不完整，不得临时发明另一套提示词结构。

## STEP 1｜询问视觉风格

### 07｜风格最高优先级

**词汇释义**：preset /ˈpriːset/ n. 预设；custom /ˈkʌstəm/ adj. 自定义的；top priority /tɒp praɪˈɒrəti/ n. phr. 最高优先级；supplemental /ˌsʌplɪˈmentəl/ adj. 补充的；texture /ˈtekstʃə/ n. 质感；rendering /ˈrendərɪŋ/ n. 渲染；outfit /ˈaʊtfɪt/ n. 服装。

**译文**：让用户选择预设风格或输入自定义风格。该风格具有最高优先级，控制补充风格措辞、配色语言、背景质感、人物渲染、表情、服装方向、界面颜色、按钮／图标风格及字体质感。

## STEP 2｜采集玩家与游戏信息

### 08｜只映射人物身份，不继承照片质感

**词汇释义**：identity mapping /aɪˈdentəti ˈmæpɪŋ/ n. phr. 身份映射；recognizable /ˈrekəɡnaɪzəbəl/ adj. 可辨识的；face silhouette /feɪs ˌsɪluˈet/ n. phr. 面部轮廓；relative facial proportion /ˈrelətɪv ˈfeɪʃəl prəˈpɔːʃən/ n. phr. 相对五官比例；distinctive trait /dɪˈstɪŋktɪv treɪt/ n. phr. 显著特征；inherit /ɪnˈherɪt/ v. 继承；photographic realism /ˌfəʊtəˈɡræfɪk ˈrɪəlɪzəm/ n. phr. 摄影写实性；redesign /ˌriːdɪˈzaɪn/ v. 重新设计。

**译文**：采集 PLAYER 1 名称、PLAYER 2 名称和游戏标题。用户提供人物图时，只把两位玩家参考用于身份映射：可辨识脸部轮廓、发型、眼镜、五官相对比例和独特特征。不要继承摄影写实性、皮肤纹理、现实光照、相机画质或原图风格；保留身份锚点，同时按选定风格重新设计脸。

## STEP 3｜构建 GPT 确认图提示词

### 09｜固定框架与动态风格

**词汇释义**：GPT abbr. Generative Pre-trained Transformer，生成式预训练 Transformer；skeleton /ˈskelɪtən/ n. 骨架；fixed /fɪkst/ adj. 固定的；dynamic /daɪˈnæmɪk/ adj. 动态的；palette-linked /ˈpælət lɪŋkt/ adj. 与配色联动的。

**译文**：加载并遵循 `references/h3-confirmation-image-template.md`，把它作为必需提示词骨架。采用固定框架＋动态风格填充＋配色联动结构。

### 10｜Overall Style：整体风格

**词汇释义**：promo poster /ˈprəʊməʊ ˈpəʊstə/ n. phr. 宣传海报；deep integration /diːp ˌɪntɪˈɡreɪʃən/ n. phr. 深度融合；commercial /kəˈmɜːʃəl/ adj. 商业的；visual impact /ˈvɪʒuəl ˈɪmpækt/ n. phr. 视觉冲击；over-decoration /ˌəʊvə ˌdekəˈreɪʃən/ n. 过度装饰。

**译文**：始终保留游戏主菜单界面、高品质游戏宣传海报、界面与人物深度融合、现代商业游戏界面设计、强视觉冲击、干净构图，以及避免过度装饰。其他风格词随所选风格添加。

### 11｜Color Palette：配色

**词汇释义**：main color /meɪn ˈkʌlə/ n. phr. 主色；functional accent /ˈfʌŋkʃənəl ˈæksent/ n. phr. 功能强调色；danger accent /ˈdeɪndʒə ˈæksent/ n. phr. 危险提示强调色；high-contrast /ˌhaɪ ˈkɒntrɑːst/ adj. 高对比的；color blocking /ˈkʌlə ˈblɒkɪŋ/ n. phr. 色块拼接；type /taɪp/ n. 字体、印刷字。

**译文**：始终遵循：xx 为主色、xx 为界面主体色、xx 为文字色、xx 为功能强调色、红色为危险强调色；配色控制在五色以内，高对比色块，清新现代观感，以及 xx 风格的色彩语言。后续所有界面／按钮／图标／字体颜色都须匹配此配色。

### 12｜Composition：构图

**词汇释义**：landscape /ˈlændskeɪp/ adj. 横幅的；full-frame /fʊl freɪm/ adj. 满画面的；caution tape /ˈkɔːʃən teɪp/ n. phr. 警示带；graffiti /ɡrəˈfiːti/ n. 涂鸦；Z reading path /zed ˈriːdɪŋ pɑːθ/ n. phr. Z 形阅读路径；negative space /ˈneɡətɪv speɪs/ n. phr. 留白；hierarchy /ˈhaɪərɑːki/ n. 层级。

**译文**：保留 16:9 横幅、满幅背景、居中的 x 名人物、环绕而不遮挡人物的界面、左上玩家卡、右侧竖排菜单、底部警示带、少量角落涂鸦、Z 形阅读路线、充足留白、清晰层级；Continue 是视觉焦点。

### 13｜Background：背景

**词汇释义**：solid-color /ˈsɒlɪd ˈkʌlə/ adj. 纯色的；dense scratch /dens skrætʃ/ n. phr. 密集划痕；ink splash /ɪŋk splæʃ/ n. phr. 墨水飞溅；paint splatter /peɪnt ˈsplætə/ n. phr. 油漆泼溅；spray-paint /ˈspreɪpeɪnt/ n. 喷漆；premium /ˈpriːmiəm/ adj. 高品质的；derive /dɪˈraɪv/ v. 从……取得。

**译文**：遵循纯 xx 背景、轻微 xx 纹理、大块纯色留白，纹理只作细节；避免重污垢、密集划痕、过多墨点和大片油漆泼溅，只加少量黑色边缘喷漆细节；背景干净、现代、高品质且以界面为先。xx 及补充项由所选风格推导。

### 14｜Character Style：人物风格

**词汇释义**：strictly /ˈstrɪktli/ adv. 严格地；expand /ɪkˈspænd/ v. 展开；dimension guidance /daɪˈmenʃən ˈɡaɪdəns/ n. phr. 描述维度指导；fixed style /fɪkst staɪl/ n. phr. 固定风格。

**译文**：严格根据选定风格展开。源文本只用于提示应描述哪些维度，不作为固定风格。

### 15｜Character A：人物 A

**词汇释义**：facial feature /ˈfeɪʃəl ˈfiːtʃə/ n. phr. 五官特征；compatible /kəmˈpætəbəl/ adj. 相容的；khaki /ˈkɑːki/ adj. 卡其色的；cargo pants /ˈkɑːɡəʊ pænts/ n. phr. 工装裤；adventurer /ədˈventʃərə/ n. 冒险者；cross-legged /ˌkrɒsˈleɡd/ adj. 盘腿的；backward lean /ˈbækwəd liːn/ n. phr. 身体后倾。

**译文**：五官来自人物图 1；表情、渲染、服装跟随所选风格。可选且兼容的服装维度包括卡其短夹克、黑内搭、黑工装裤、棕色靴子、冒险者装束。固定动作：盘腿坐、双手撑地、略微后倾、向上看。

### 16｜Character B：人物 B

**词汇释义**：thick jacket /θɪk ˈdʒækɪt/ n. phr. 厚外套；burgundy /ˈbɜːɡəndi/ adj. 酒红色的；padded lining /ˈpædɪd ˈlaɪnɪŋ/ n. phr. 加厚衬里；inner shirt /ˈɪnə ʃɜːt/ n. phr. 内搭衬衫；forward lean /ˈfɔːwəd liːn/ n. phr. 前倾。

**译文**：五官来自人物图 2；表情、渲染与服装跟随所选风格。兼容的可选服装维度包括绿色厚外套、酒红色加厚衬里、白内搭衬衫、黑裤子与厚靴。固定动作：盘腿坐、双手放在腿前、略微前倾、看向摄影机。

### 17｜Lighting：光照

**词汇释义**：top main light /tɒp meɪn laɪt/ n. phr. 顶部主光；fill /fɪl/ n. 补光；ambient reflection /ˈæmbiənt rɪˈflekʃən/ n. phr. 环境反射；contact shadow /ˈkɒntækt ˈʃædəʊ/ n. phr. 接触阴影；rim light /rɪm laɪt/ n. phr. 轮廓光；GI abbr. Global Illumination，全局光照。

**译文**：保留顶部主光、左上暖／冷补光、下方柔和环境反射、柔软阴影、接触阴影、轮廓光、高品质全局光照，以及人物背景自然融合。冷暖选择取决于风格。

### 18｜Game UI：游戏界面

**词汇释义**：console /ˈkɒnsəʊl/ n. 游戏主机；unified /ˈjuːnɪfaɪd/ adj. 统一的；rounded rectangle /ˈraʊndɪd ˈrektæŋɡəl/ n. phr. 圆角矩形；tilt /tɪlt/ n. 倾斜；drip /drɪp/ n. 滴落痕迹；sticker /ˈstɪkə/ n. 贴纸；readability /ˌriːdəˈbɪləti/ n. 可读性；outline /ˈaʊtlaɪn/ n. 描边；glow /ɡləʊ/ n. 辉光。

**译文**：保留主机游戏菜单、统一按钮尺寸、圆角矩形、轻微倾斜、少量喷漆／滴落元素、现代干净贴纸设计、可读性及不过度装饰。按钮主体、描边与辉光颜色必须匹配配色。

### 19｜Layout Rules：布局规则

**词汇释义**：horizontal /ˌhɒrɪˈzɒntəl/ adj. 水平的；radius /ˈreɪdiəs/ n. 半径；adapt /əˈdæpt/ v. 适应；single-line /ˈsɪŋɡəl laɪn/ adj. 单行的；wrapping /ˈræpɪŋ/ n. 自动换行；centered /ˈsentəd/ adj. 居中的；margin /ˈmɑːdʒɪn/ n. 边距；spacing /ˈspeɪsɪŋ/ n. 间距。

**译文**：保留横向长按钮、统一宽／高／圆角，宽度适应文字；标题只用单行，不换行、不做双行标题；文字居中，边距与间距一致。

### 20｜Buttons：按钮

**词汇释义**：highlighted /ˈhaɪlaɪtɪd/ adj. 高亮的；hover /ˈhɒvə/ n. 悬停；click state /klɪk steɪt/ n. phr. 点击状态；visually consistent /ˈvɪʒuəli kənˈsɪstənt/ phr. 视觉一致；exit cue /ˈeksɪt kjuː/ n. phr. 退出提示。

**译文**：颜色取自配色，图标取自所选风格。Continue 为大型视觉中心高亮按钮，带悬停／点击状态；Start New Game 在 Continue 上方；Settings 保持视觉一致；Exit Game 使用危险／退出提示，可用红色强调。

### 21｜Player Cards：玩家卡

**词汇释义**：irregular /ɪˈreɡjʊlə/ adj. 不规则的；edge damage /edʒ ˈdæmɪdʒ/ n. phr. 边缘破损；three-level /θriː ˈlevəl/ adj. 三级的；nickname /ˈnɪkneɪm/ n. 昵称；bold sans-serif /bəʊld sænz ˈserɪf/ n. phr. 粗体无衬线字；industrial sticker /ɪnˈdʌstriəl ˈstɪkə/ n. phr. 工业贴纸。

**译文**：保留左上 x 位玩家信息卡、不规则矩形卡、描边、轻微边损、左侧标志／图标、右侧三级信息（PLAYER 标签、昵称、READY）、粗体无衬线字体和工业贴纸设计。卡片颜色、描边、READY 颜色及标志风格随配色与选定风格。

### 22｜Icon System：图标系统

**词汇释义**：derive /dɪˈraɪv/ v. 推导；stacking /ˈstækɪŋ/ n. 叠放、堆叠；minimal quantity /ˈmɪnɪməl ˈkwɒntəti/ n. phr. 最少数量；steal focus /stiːl ˈfəʊkəs/ v. phr. 抢夺焦点。

**译文**：图标风格取自所选风格，颜色取自配色。只排一行，不换行、不堆叠；每个界面区域最多一行，数量尽量少，尺寸统一，绝不抢焦点。

### 23｜Typography：字体编排

**词汇释义**：all caps /ɔːl kæps/ n. phr. 全大写；weight /weɪt/ n. 字重；tight tracking /taɪt ˈtrækɪŋ/ n. phr. 紧字距；heavy stroke /ˈhevi strəʊk/ n. phr. 粗笔画；hierarchy /ˈhaɪərɑːki/ n. 层级；texture /ˈtekstʃə/ n. 质感。

**译文**：保留粗体无衬线、全大写、类似 Anton／Impact／Burbank／Tungsten 的字重、紧字距、粗笔画、清晰层级和单行排版。不得换行，按钮宽度适应文字，不得有双行菜单标题。颜色与质感跟随配色和所选风格。

## STEP 4｜生成首张确认图

### 24｜只生成一张

**词汇释义**：filled /fɪld/ adj. 已填充的；framework structure /ˈfreɪmwɜːk ˈstrʌktʃə/ n. phr. 框架结构；visibly dominant /ˈvɪzəbli ˈdɒmɪnənt/ phr. 在视觉上占主导。

**译文**：从填充后的 `references/h3-confirmation-image-template.md` 只生成一张确认图。保留框架结构，同时使所选风格明显占主导。

## STEP 5｜等待确认

### 25｜未确认不生成视频

**词汇释义**：approval /əˈpruːvəl/ n. 确认；identity /aɪˈdentəti/ n. 身份；return /rɪˈtɜːn/ v. 返回。

**译文**：用户未确认图片前不能生成视频。用户改变风格、名字、游戏标题、身份或图片方向时，返回图像提示词步骤。

## STEP 6｜重新填充视频提示词，并用 MiniMax H3 生成

### 26｜按已确认结果重新填写

**词汇释义**：load /ləʊd/ v. 加载；refill /ˌriːˈfɪl/ v. 重新填充；confirmed /kənˈfɜːmd/ adj. 已确认的；negative constraint /ˈneɡətɪv kənˈstreɪnt/ n. phr. 负面限制。

**译文**：确认之后加载 `references/h3-video-prompt-template.md`，用已确认风格、人物参考、玩家名称、游戏标题、界面文字、事件时序、运动方向和负面限制重新填充最终视频提示词。用 MiniMax H3 生成最终视频。

## STEP 7｜修复常见失败

### 27｜文字、身份和风格修复

**词汇释义**：unreadable /ʌnˈriːdəbəl/ adj. 不可读的；identity swap /aɪˈdentəti swɒp/ n. phr. 身份对调；drift /drɪft/ v. 漂移；reuse /ˌriːˈjuːz/ v. 复用；preserve /prɪˈzɜːv/ v. 保留；outfit anchor /ˈaʊtfɪt ˈæŋkə/ n. phr. 服装锚点；rewrite /ˌriːˈraɪt/ v. 重写。

**译文**：文字难辨时减少画面文字；身份对调时强化姓名、位置和颜色；面孔漂移时复用上传参考，明确保持身份锚点、发型和服装锚点，同时保持所选风格的脸部渲染。风格不明显时，重写 Overall Style、Color Palette、Character Style、Background、Game UI、Buttons、Icons、Typography，而不是改动布局框架。
