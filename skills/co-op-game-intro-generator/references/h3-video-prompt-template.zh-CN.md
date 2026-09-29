# H3 Video Prompt Template｜H3 视频提示词模板：逐段注释译本

源文件：[h3-video-prompt-template.md](./h3-video-prompt-template.md)。固定源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`9eaaa0dcd5d63be0f388434343f6c76b8bb56523`。本文件新增于源文件同目录，不修改源文。英文段落先作词汇释义再翻译；已有中文段落保留其信息，为嵌入的英文术语补注。单花括号变量、时间段、玩家编号、身体左右侧和界面文字保持对应。n. 名词；v. 动词；adj. 形容词；adv. 副词；n. phr. 名词短语；v. phr. 动词短语；abbr. 缩写。

## 一、Prompt principle：提示词原则

### 01｜方法

**词汇释义**：principle /ˈprɪnsəpəl/ n. 原则；confirmation image /ˌkɒnfəˈmeɪʃən ˈɪmɪdʒ/ n. phr. 确认图；fixed framework /fɪkst ˈfreɪmwɜːk/ n. phr. 固定框架；dynamic /daɪˈnæmɪk/ adj. 动态的；identity /aɪˈdentəti/ n. 身份；palette-linked /ˈpælət lɪŋkt/ adj. 与配色联动的；UI abbr. User Interface，用户界面。

**译文**：采用与 GPT 确认图提示词相同的方法：**固定的视频事件框架＋按用户风格动态填充＋锁定人物身份＋与配色联动的界面系统。**

### 02｜保持事件结构，重写视觉处理

**词汇释义**：blindly /ˈblaɪndli/ adv. 盲目地；preserve /prɪˈzɜːv/ v. 保留；timeline /ˈtaɪmlaɪn/ n. 时间线；equipment logic /ɪˈkwɪpmənt ˈlɒdʒɪk/ n. phr. 装备逻辑；visual treatment /ˈvɪʒuəl ˈtriːtmənt/ n. phr. 视觉处理；surface /ˈsɜːfɪs/ n. 表面；city-world /ˈsɪti wɜːld/ n. 城市世界。

**译文**：视频提示词不能盲目保留源提示词的默认风格。它必须保留时间线、界面事件、玩家位置、装备逻辑和文字结构，同时按用户选定风格动态重写视觉处理、配色、人物渲染、光照、界面表面、图标和城市世界风格。

## 二、Priority order：优先级顺序

### 03｜六级优先顺序

**词汇释义**：priority /praɪˈɒrəti/ n. 优先级；confirmed /kənˈfɜːmd/ adj. 已确认的；reference /ˈrefərəns/ n. 参考；comparison /kəmˈpærɪsən/ n. 对比；height /haɪt/ n. 身高；body /ˈbɒdi/ n. 身体。

**译文**：依次为：1. 用户选定风格 `{visual_style}`；2. 已确认图片／界面参考 `{ui_ref}`；3. PLAYER 1 身份参考 `{player1_ref}`；4. PLAYER 2 身份参考 `{player2_ref}`；5. 身高／体型对比参考 `{height_ref}`；6. 固定的源视频事件框架。

## 三、Reference roles：参考素材的作用

### 04｜界面参考

**词汇释义**：menu hierarchy /ˈmenjuː ˈhaɪərɑːki/ n. phr. 菜单层级；typography scale /taɪˈpɒɡrəfi skeɪl/ n. phr. 字体尺寸层级；integration /ˌɪntɪˈɡreɪʃən/ n. 融合；composition logic /ˌkɒmpəˈzɪʃən ˈlɒdʒɪk/ n. phr. 构图逻辑。

**译文**：`{ui_ref}`：已确认的第一张图像。用它锁定界面布局、菜单层级、色彩系统、字体尺寸、按钮结构、人物与游戏的融合，以及整体构图逻辑。

### 05｜玩家一身份参考

**词汇释义**：identity anchor /aɪˈdentəti ˈæŋkə/ n. phr. 身份锚点；hairstyle /ˈheəstaɪl/ n. 发型；facial proportion /ˈfeɪʃəl prəˈpɔːʃən/ n. phr. 五官比例；nickname mapping /ˈnɪkneɪm ˈmæpɪŋ/ n. phr. 昵称映射。

**译文**：`{player1_ref}`：PLAYER 1 的身份锚点。锁定准确面孔、发型、眼镜（有时）、五官比例、身体身份特征，以及与 `{player1_name}` 的昵称对应关系。

### 06｜玩家二身份参考

**词汇释义**：exact face /ɪɡˈzækt feɪs/ n. phr. 准确的面孔；body identity /ˈbɒdi aɪˈdentəti/ n. phr. 身体身份特征；lock /lɒk/ v. 锁定。

**译文**：`{player2_ref}`：PLAYER 2 的身份锚点。锁定准确面孔、发型、五官比例、身体身份特征，以及与 `{player2_name}` 的昵称对应关系。

### 07｜体型对比参考

**词汇释义**：visible contrast /ˈvɪzəbəl ˈkɒntrɑːst/ n. phr. 可见差异；prevent /prɪˈvent/ v. 防止；identical /aɪˈdentɪkəl/ adj. 完全相同的；body proportion /ˈbɒdi prəˈpɔːʃən/ n. phr. 身体比例。

**译文**：`{height_ref}`：体型对比锚点。锁定两位玩家可见的体型差异，防止身体比例变得相同。

## 四、Global style baseline：全局风格基准

### 08｜风格与固定基准

**词汇释义**：baseline /ˈbeɪslaɪn/ n. 基准；visual style /ˈvɪʒuəl staɪl/ n. phr. 视觉风格；commercial game UI /kəˈmɜːʃəl ɡeɪm juː aɪ/ n. phr. 商业游戏界面。

**正文**：整体画风必须优先服从用户选择：`{visual_style}`。保留固定基准：游戏主菜单 UI、高品质游戏宣传片质感、UI 与角色深度融合、现代商业游戏 UI 设计、极强视觉冲击力、画面简洁干净、避免过度装饰。其余视觉层面根据 `{visual_style}` 动态拓展：角色画风、表情气质、服装语言、色彩系统、灯光冷暖、UI 材质、按钮图标、字体质感、城市加载后的世界风格。

## 五、Palette system：配色系统

### 09｜全程联动配色

**词汇释义**：palette /ˈpælət/ n. 配色；functional accent /ˈfʌŋkʃənəl ˈæksent/ n. phr. 功能强调色；HUD abbr. Head-Up Display，抬头显示界面，此处指游戏状态叠加界面；loading bar /ˈləʊdɪŋ bɑː/ n. phr. 加载进度条。

**正文**：根据 `{visual_style}` 推导视频全程色彩，但必须保持 UI 色彩联动：xx 色作为主体背景／世界主色；xx 色作为 UI 主体颜色；xx 色作为文字颜色；xx 色作为功能强调色；红色作为危险／退出／警示提示色；整体颜色控制在 5 种以内；高对比撞色、鲜明现代、符合 `{visual_style}` 的色彩语言。

**正文**：视频中的菜单、装备面板、玩家卡、按钮、HUD、加载条、图标和文字都必须沿用同一色彩系统，不得随机新增无关颜色。

## 六、Character identity and style lock：人物身份与风格锁定

### 10｜PLAYER 1

**词汇释义**：identity lock /aɪˈdentəti lɒk/ n. phr. 身份锁定；agile /ˈædʒaɪl/ adj. 敏捷的；mechanical claw /mɪˈkænɪkəl klɔː/ n. phr. 机械爪；lightweight /ˈlaɪtweɪt/ adj. 轻量的；slender /ˈslendə/ adj. 纤细的。

**正文**：PLAYER 1：五官信息参考 `{player1_ref}`，必须保留脸、人脸比例、发型、眼镜（如有）、个人身份和 `{player1_name}` 昵称对应关系。表情、画风、服装和机械装备的视觉处理根据 `{visual_style}` 动态优化。PLAYER 1 始终位于左侧，偏高挑／修长／敏捷，装备色为功能强调色，机械爪轻量、纤细、灵活。

### 11｜PLAYER 2

**词汇释义**：stocky /ˈstɒki/ adj. 矮壮的；amber /ˈæmbə/ n./adj. 琥珀／琥珀色的；mechanical fist /mɪˈkænɪkəl fɪst/ n. phr. 机械拳；heavy /ˈhevi/ adj. 厚重的。

**正文**：PLAYER 2：五官信息参考 `{player2_ref}`，必须保留脸、人脸比例、发型、个人身份和 `{player2_name}` 昵称对应关系。表情、画风、服装和机械装备的视觉处理根据 `{visual_style}` 动态优化。PLAYER 2 始终位于右侧，偏矮壮／宽厚／力量型，装备色为琥珀红或与危险／力量提示一致的暖色，机械拳厚重、宽大、有重量。

### 12｜身份禁用项

**词汇释义**：identity swapping /aɪˈdentəti ˈswɒpɪŋ/ n. phr. 身份对调；merge /mɜːdʒ/ v. 融合；nickname /ˈnɪkneɪm/ n. 昵称。

**正文**：禁止角色身份交换、脸部互相融合、昵称交换、两人体型趋同。

## 七、Fixed timeline framework：固定时间线框架

### [0秒–2秒]｜双人主菜单

**词汇释义**：high-angle /ˈhaɪ ˈæŋɡəl/ adj. 高角度的；wide shot /waɪd ʃɒt/ n. phr. 远景镜头；push in /pʊʃ ɪn/ v. phr. 摄影机推进；blink /blɪŋk/ v. 眨眼。

**正文**：景别／机位：高角度俯拍大全景，延续 `{ui_ref}` 的构图逻辑。镜头从上方轻微下压并缓慢推进。

**正文**：画面内容：PLAYER 1（`{player1_name}`）和 PLAYER 2（`{player2_name}`）并排坐在画面中央，PLAYER 1 在左，PLAYER 2 在右，抬头看向摄像机。两人只有自然呼吸、眨眼和轻微身体动作。

**词汇释义**：READY /ˈredi/ adj. 准备就绪；START NEW GAME /stɑːt njuː ɡeɪm/ v. phr. 开始新游戏；CONTINUE /kənˈtɪnjuː/ v. 继续；SETTINGS /ˈsetɪŋz/ n. 设置；EXIT GAME /ˈeksɪt ɡeɪm/ v. phr. 退出游戏。

**正文**：UI 结构：左上角玩家资料卡准确显示 `PLAYER 1`、`{player1_name}`、`READY`。顶部中央或左上双卡系统中的第二张资料卡准确显示 `PLAYER 2`、`{player2_name}`、`READY`。右侧纵向菜单准确显示 `START NEW GAME`、`CONTINUE`、`SETTINGS`、`EXIT GAME`。`CONTINUE` 是视觉中心和主高亮按钮。中文释义只帮助理解，不替换这些画内英文文案。

**词汇释义**：dynamic style fill /daɪˈnæmɪk staɪl fɪl/ n. phr. 动态风格填充；hierarchy /ˈhaɪərɑːki/ n. 层级；hover /ˈhɒvə/ n. 悬停；ambience /ˈæmbiəns/ n. 环境氛围。

**正文**：动态风格填充：主菜单背景、地面纹理、按钮形态、图标、字体、边框、辉光和贴纸质感全部根据 `{visual_style}` 优化，但保留 `{ui_ref}` 的布局和层级。

**正文**：声音：菜单环境音、轻微 UI hover 声、点击前的低频电子氛围。若生成无音频，则忽略声音执行。

### [2秒–4秒]｜PLAYER 1 右臂配置

**词汇释义**：medium shot /ˈmiːdiəm ʃɒt/ n. phr. 中景；right arm /raɪt ɑːm/ n. phr. 右臂；equipment /ɪˈkwɪpmənt/ n. 装备；phantom /ˈfæntəm/ n./adj. 幽灵／幻影的；grip /ɡrɪp/ n. 抓握；claw /klɔː/ n. 爪；CHRONOS 为装备名中的专名，不擅自改动。

**正文**：景别／机位：中景，镜头从主菜单平滑推近 PLAYER 1 的右臂，PLAYER 2 仍在背景中可见，不消失、不变形。

**正文**：UI 结构：右侧主菜单收缩滑出；带功能强调色识别线的 UI 面板从左侧滑入，准确显示 `PLAYER 1`、`RIGHT ARM EQUIPMENT`。装备列表中先高亮 `PHANTOM GRIP`，随后选区移动至 `CHRONOS CLAW`。其中 `RIGHT ARM EQUIPMENT` 意为“右臂装备”；装备名称原样保留。

**词汇释义**：forearm /ˈfɔːrɑːm/ n. 前臂；knuckle /ˈnʌkəl/ n. 指节；piston /ˈpɪstən/ n. 活塞；connector /kəˈnektə/ n. 连接件；LED abbr. Light-Emitting Diode，发光二极管。

**正文**：动作：PLAYER 1 的右袖口自动打开，轻量机械结构从前臂下方展开。手指分开，修长爪状指节滑入并逐一锁定，内部短暂露出精细线路、微型活塞和金属连接件。配置完成后，功能强调色 LED 依次亮起。

**词汇释义**：precision /prɪˈsɪʒən/ n. 精密性；flexible /ˈfleksəbəl/ adj. 灵活的；locking /ˈlɒkɪŋ/ n. 锁定；sound /saʊnd/ n. 声音。

**正文**：动态风格填充：机械结构、UI 面板材质、图标、线条、锁定动画和光效根据 `{visual_style}` 优化，但必须轻量、精密、灵活，符合 PLAYER 1 身形，不改变脸、发型和服装主体。

**正文**：声音：精密机械展开声、轻快 UI 切换音、细小锁定声。

### [4秒–7秒]｜PLAYER 2 重型手臂配置

**词汇释义**：armament /ˈɑːməmənt/ n. 装备、武装配置；customization /ˌkʌstəmaɪˈzeɪʃən/ n. 定制；hand /hænd/ n. 手；forearm /ˈfɔːrɑːm/ n. 前臂；elbow /ˈelbəʊ/ n. 肘；upper arm /ˈʌpə ɑːm/ n. phr. 上臂。

**正文**：景别／机位：中景，摄影机沿两人之间平滑横移并绕向 PLAYER 2 左侧。PLAYER 1 留在背景中，轻轻观察自己完成配置的机械手。

**正文**：UI 结构：新的暖色／琥珀红识别 UI 滑入，准确显示 `PLAYER 2`、`ARMAMENT CUSTOMIZATION`。面板以网格形式展示 `HAND`、`FOREARM`、`ELBOW`、`UPPER ARM`；选区快速但清晰地在四个组件之间切换。上述身体部位依次为手、前臂、肘和上臂。

**词汇释义**：armor /ˈɑːmə/ n. 装甲；guide rail /ɡaɪd reɪl/ n. phr. 导轨；bearing /ˈbeərɪŋ/ n. 轴承；hydraulic /haɪˈdrɒlɪk/ adj. 液压的；indicator /ˈɪndɪkeɪtə/ n. 指示器。

**正文**：动作：PLAYER 2 左臂外套袖口分段打开，厚重前臂护板向外弹开，旧组件脱离，新型装甲沿导轨滑入；肘关节替换为厚实机械轴承，宽大的机械手重新组合并锁定。更换过程中短暂露出粗壮线路、液压活塞和深色金属骨架。每个部件锁定时亮起低调暖色指示灯。

**词汇释义**：heavy-duty /ˌheviˈdjuːti/ adj. 重型的；contrast /ˈkɒntrɑːst/ n. 对比；motor /ˈməʊtə/ n. 电机；feedback /ˈfiːdbæk/ n. 反馈。

**正文**：动态风格填充：重型机械臂、UI 面板、组件图标、材质、光效根据 `{visual_style}` 优化，但必须厚重、宽大、有力量感，与 PLAYER 1 的轻量机械爪形成清晰对比。

**正文**：声音：低沉电机声、重型机械扣合声、厚重锁定反馈。

### [7秒–8.5秒]｜双人确认配置

**词汇释义**：confirm /kənˈfɜːm/ v. 确认；config abbr. configuration，配置；shared button /ʃeəd ˈbʌtən/ n. phr. 共享按钮；cursor /ˈkɜːsə/ n. 光标；energy pulse /ˈenədʒi pʌls/ n. phr. 能量脉冲。

**正文**：景别／机位：中景拉回，镜头平滑回到双人构图，PLAYER 1 左侧，PLAYER 2 右侧。

**正文**：UI 结构：两组装备面板向画面中央汇合，形成共享按钮，准确显示 `CONFIRM CONFIG`，即“确认配置”。按钮边框、辉光、图标和贴纸质感根据 `{visual_style}` 优化，但层级清晰、文字可读。

**词汇释义**：uncross /ˌʌnˈkrɒs/ v. 解开交叉姿势；knee /niː/ n. 膝；clench /klentʃ/ v. 握紧；retract /rɪˈtrækt/ v. 收缩。

**正文**：动作：光标点击按钮，功能强调色能量脉冲流过 PLAYER 1 的机械爪，暖色／琥珀红能量脉冲流过 PLAYER 2 的机械拳。所有 UI 面板快速向内收缩并消失。两人同时解开交叉的双腿并调整坐姿：PLAYER 1 轻盈抬起单膝，修长机械爪依次活动手指；PLAYER 2 一只脚稳稳踩地，厚重机械拳缓慢握紧。

**正文**：声音：确认提示音、双色能量脉冲、UI 收缩声。

### [8.5秒–10秒]｜双人世界加载

**词汇释义**：loading /ˈləʊdɪŋ/ n. 加载；progress /ˈprəʊɡres/ n. 进度；shared loading bar /ʃeəd ˈləʊdɪŋ bɑː/ n. phr. 共享加载条；texture /ˈtekstʃə/ n. 纹理。

**正文**：景别／机位：全景，底部共享加载条出现。

**正文**：UI 结构：加载条准确显示 `LOADING`。进度从 0% 快速填充至 100%。左半段使用 PLAYER 1 的功能强调色，右半段使用 PLAYER 2 的暖色／力量色。HUD 和加载条的形态、边框、纹理、字体根据 `{visual_style}` 优化，但必须清晰可读。

**词汇释义**：environment transformation /ɪnˈvaɪrənmənt ˌtrænsfəˈmeɪʃən/ n. phr. 环境转化；construction barrier /kənˈstrʌkʃən ˈbæriə/ n. phr. 施工围挡；graffiti /ɡrəˈfiːti/ n. 涂鸦；alley /ˈæli/ n. 巷道；hard cut /hɑːd kʌt/ n. phr. 硬切。

**正文**：环境转化：黄色平面环境连续转化为游戏世界。警戒线变成真实街道道路标记和施工围挡；墨迹／纹理化为潮湿路面反光或符合 `{visual_style}` 的地面光影；平面涂鸦扩展成建筑墙面的喷绘；黑色背景区域形成城市阴影和深巷入口。

**正文**：关键约束：转化必须连续自然，不使用硬切，不用烟雾遮挡，不改变两位角色身份。

**正文**：声音：加载上升音、环境从菜单氛围过渡到城市氛围。

### [10秒–15秒]｜双人进入游戏世界

**词汇释义**：third-person /ˌθɜːd ˈpɜːsən/ adj. 第三人称的；tracking shot /ˈtrækɪŋ ʃɒt/ n. phr. 跟拍镜头；cooperative view /kəʊˈɒpərətɪv vjuː/ n. phr. 合作视角；stand up /stænd ʌp/ v. phr. 站起。

**正文**：景别／机位：大全景转第三人称跟拍。加载 100% 的瞬间，两名角色同时起身。摄影机平滑下降并绕到两人身后，变成稳定第三人称双人合作视角。

**词汇释义**：skyline /ˈskaɪlaɪn/ n. 天际线；industrial pipe /ɪnˈdʌstriəl paɪp/ n. phr. 工业管道；cyberpunk /ˈsaɪbəpʌŋk/ n. 赛博朋克；vehicle /ˈviːɪkəl/ n. 载具；architecture /ˈɑːkɪtektʃə/ n. 建筑。

**正文**：世界风格：完整游戏世界根据 `{visual_style}` 动态生成。保留游戏开场进入世界的结构：密集建筑、道路、标志灯、招牌、人群或动态背景、快速经过的载具、电线、工业管道、远处城市天际线。具体世界材质、建筑形态、招牌设计、光影和动效必须服从 `{visual_style}`；不要让源默认赛博朋克风格压过用户选择，除非用户选择的是赛博朋克。

**词汇释义**：rear view /rɪə vjuː/ n. phr. 背面视图；slender /ˈslendə/ adj. 修长的；stocky /ˈstɒki/ adj. 矮壮的；side by side /saɪd baɪ saɪd/ adv. 并肩地。

**正文**：角色关系：清楚展示两人的背影和体型差异：PLAYER 1 左侧，高挑修长，轻量机械爪自然垂下；PLAYER 2 右侧，矮壮宽厚，重型机械拳微微抬起。PLAYER 1 率先迈步，PLAYER 2 紧随其后，两人并肩进入街道。

**词汇释义**：mini-map /ˈmɪni mæp/ n. 小地图；status bar /ˈsteɪtəs bɑː/ n. phr. 状态栏；mission marker /ˈmɪʃən ˈmɑːkə/ n. phr. 任务标记；fade in /feɪd ɪn/ v. phr. 淡入；footstep /ˈfʊtstep/ n. 脚步声。

**正文**：HUD 结构：HUD 淡入。右上角出现小地图；左下角出现两组独立状态栏：`{player1_name}`、`{player2_name}`。`{player1_name}` 状态栏使用 PLAYER 1 功能强调色，`{player2_name}` 状态栏使用 PLAYER 2 暖色／力量色。前方街道中央出现共享任务标记。

**正文**：声音：城市环境氛围、远处载具声、脚步声、HUD 淡入提示音。

## 八、Negative constraints：负面限制

### 13｜完整限制段

**词汇释义**：duplicated /ˈdjuːplɪkeɪtɪd/ adj. 重复的；swapping /ˈswɒpɪŋ/ n. 对调；merged body /mɜːdʒd ˈbɒdi/ n. phr. 融合身体；identical /aɪˈdentɪkəl/ adj. 完全相同的；split screen /splɪt skriːn/ n. phr. 分屏；gruesome /ˈɡruːsəm/ adj. 可怖血腥的；dismemberment /dɪsˈmembəmənt/ n. 肢解；weapon /ˈwepən/ n. 武器；excessive /ɪkˈsesɪv/ adj. 过度的；misspelled /ˌmɪsˈspeld/ adj. 拼写错误的；branded interface /ˈbrændɪd ˈɪntəfeɪs/ n. phr. 带品牌识别的界面；watermark /ˈwɔːtəmɑːk/ n. 水印。

**译文**：不要第三名玩家；除非用户明确要求，不要女性人物；不要重复人物、人物对调、用户名对调、身体融合或相同身体比例；不要改变面孔、发型或身份；不要缺少 PLAYER 1 或 PLAYER 2；不要分屏、硬切、随机摄影机抖动、悬浮肢体、可怖肢解或武器。除非用户风格选择要求，不要过度霓虹或紫色背景。不要不可读界面、随机字母、拼错用户名、额外菜单选项、官方游戏标志、复制的品牌界面或水印。

---

## 校对说明（不属于源模板）

本源模板是 **15 秒、六时间段、装备配置后进入城市世界** 的方案，不是 8 秒静态菜单微动方案。时间段为 0–2、2–4、4–7、7–8.5、8.5–10、10–15 秒；PLAYER 1 配置右臂，PLAYER 2 配置左臂；最后两人起身、摄影机下降绕后并跟拍。不得以“不站起”“不换到游戏世界”“镜头不环绕”替换这些源动作。

源文一方面要求全局配色服从用户风格，另一方面在 8.5–10 秒段固定写“黄色平面环境”；这一张力按原文保留，实际改编时另行决策。源文要求玩家保持左右关系，同时安排局部环绕机位；实际制作仍需做轴线检查，翻译不自动证明空间连续性已经通过。`ARMAMENT CUSTOMIZATION` 作为界面原文保留，但源文最后明确禁止武器，不能把它擅自扩写成武器展示。
