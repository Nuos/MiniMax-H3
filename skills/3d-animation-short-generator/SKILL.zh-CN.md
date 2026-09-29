# 3D Animation Short Generator｜三维动画短片生成器：逐段注释译本

源文件：[SKILL.md](./SKILL.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`6ddc1102a8c353b4be4c939444b24f62e5552cde`。本文件独立新增，不覆盖英文源文件或原有 `SKILL.cn.md`。词汇释义置于每段译文前，字段、工具名、路径与固定标记保持原样。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语；abbr. 缩写。本文件是学习译本，不是执行本轮视频生成的指令。

## 01｜名称与描述

**词汇释义**：animation /ˌænɪˈmeɪʃən/ n. 动画；short /ʃɔːt/ n. 短片；stylized /ˈstaɪlaɪzd/ adj. 风格化的；ordered /ˈɔːdəd/ adj. 有序的；production workflow /prəˈdʌkʃən ˈwɜːkfləʊ/ n. phr. 制作流程；project brief /ˈprɒdʒekt briːf/ n. phr. 项目简报；outline /ˈaʊtlaɪn/ n. 大纲；standardized /ˈstændədaɪzd/ adj. 标准化的；assembly /əˈsembli/ n. 组接；BGM abbr. Background Music，背景音乐；end-to-end /ˌend tə ˈend/ adj. 端到端的；narrative /ˈnærətɪv/ adj. 叙事性的；consistency /kənˈsɪstənsi/ n. 一致性；continuity /ˌkɒntɪˈnjuːəti/ n. 连贯性；standalone /ˈstændəˌləʊn/ adj. 独立的。

**译文**：名称为 `3d-animation-short-generator`。从故事创意出发，通过有序制作流程创建完整风格化三维动画短片，覆盖项目简报、故事大纲、人物与环境卡、标准化镜头规划、文字分镜或可选铅笔分镜、视频模型选择、单镜头生成、组接、背景音乐匹配与最终审阅。用户希望采用具有强人物一致性、场景连贯性、时序、摄影机、表演和声音控制的端到端叙事动画流程时使用。不适用于单张图片、简单编辑、照片级真人实拍或单个独立片段。

## 02｜兼容性

**词汇释义**：compatibility /kəmˌpætəˈbɪləti/ n. 兼容性；require /rɪˈkwaɪə/ v. 需要；canvas workspace /ˈkænvəs ˈwɜːkspeɪs/ n. phr. 画布工作区；choice card /tʃɔɪs kɑːd/ n. phr. 选择卡片；portable /ˈpɔːtəbəl/ adj. 可移植的；generic agent harness /dʒəˈnerɪk ˈeɪdʒənt ˈhɑːnɪs/ n. phr. 通用智能体运行框架。

**译文**：需要 MiniMax Hub 智能体，包括画布工作区、选择卡片以及 `hub_generate_image`／`hub_generate_video` 工具；不可直接移植到通用智能体运行框架。

## 03｜总体用途

**词汇释义**：story-first /ˈstɔːri fɜːst/ adj. 故事优先的；one-line idea /wʌn laɪn aɪˈdɪə/ n. phr. 一句话创意；artifact /ˈɑːtɪfækt/ n. 产物；creative gate /kriˈeɪtɪv ɡeɪt/ n. phr. 创作确认关口；expensive /ɪkˈspensɪv/ adj. 成本高的；high-impact /haɪ ˈɪmpækt/ adj. 影响较大的。

**译文**：用户希望从一句话创意做到最终剪辑视频、采用完整故事优先动画短片流程时，使用此 Skill。所有重要产物必须按制作顺序放到画布；在成本较高或影响较大的步骤前，通过用户选择卡片在创作关口暂停确认。

## 04｜核心规则与固定顺序

**词汇释义**：intake /ˈɪnteɪk/ n. 需求接收；screen size /skriːn saɪz/ n. phr. 画面尺寸；total duration /ˈtəʊtəl djʊəˈreɪʃən/ n. phr. 总时长；per-second directive /pɜː ˈsekənd dəˈrektɪv/ n. phr. 逐秒指令；spatial anchor chain /ˈspeɪʃəl ˈæŋkə tʃeɪn/ n. phr. 空间锚点链；self-check /self tʃek/ n. 自检；heavy iteration /ˈhevi ˌɪtəˈreɪʃən/ n. phr. 密集迭代；extract /ɪkˈstrækt/ v. 提取；fallback /ˈfɔːlbæk/ n. 回退；resolution /ˌrezəˈluːʃən/ n. 分辨率。

**译文**：核心规则：故事优先；接收用户需求后立即用选择卡片询问画面尺寸和总时长；画布产物有序；每个必需确认都用选择卡片。人物卡／场景卡之后固定顺序为：带逐秒指令、声音提示、空间锚点链的六列标准镜头表 → 镜头表自检关口 → 一个主文字分镜文档、每镜头一节（仅用户明确选择可视化时才加多格铅笔图；密集迭代镜头提取为独立文字节点）→ 视频模型选择卡片（默认 H3，Seedance 2.0 回退）与分辨率卡片 → 所选模型生成单镜头片段 → 完整组接并配背景音乐。最终视频必须清除全部分镜杂质。

## 全局视觉风格锁定

### 05｜适用产物

**词汇释义**：explicitly /ɪkˈsplɪsɪtli/ adv. 明确地；regardless /rɪˈɡɑːdləs/ adv. 无论；composite /ˈkɒmpəzɪt/ n. 合成成品；visual style /ˈvɪʒuəl staɪl/ n. phr. 视觉风格。

**译文**：除非用户明确要求其他视觉风格，全部人物卡、场景卡、镜头表、文字分镜、可选铅笔分镜、单镜头视频片段（不论选择哪种模型）、组接视频与最终合成都使用下列风格。

### 06｜渲染风格

**词汇释义**：Pixar-inspired /ˈpɪksɑː ɪnˈspaɪəd/ adj. 受皮克斯启发的；cartoon /kɑːˈtuːn/ adj. 卡通的；renderer /ˈrendərə/ n. 渲染器；high-end /ˌhaɪˈend/ adj. 高端的；animated feature /ˈænɪmeɪtɪd ˈfiːtʃə/ n. phr. 动画长片。

**译文**：渲染风格：受皮克斯启发的三维卡通渲染，C4D 与 Octane 渲染器观感，高端动画长片品质。C4D 指 Cinema 4D。

### 07｜人物设计

**词汇释义**：exaggerated /ɪɡˈzædʒəreɪtɪd/ adj. 夸张的；geometric simplification /ˌdʒiːəˈmetrɪk ˌsɪmplɪfɪˈkeɪʃən/ n. phr. 几何简化；material detail /məˈtɪəriəl ˈdiːteɪl/ n. phr. 材质细节；anatomy /əˈnætəmi/ n. 人体结构；shape language /ʃeɪp ˈlæŋɡwɪdʒ/ n. phr. 形状语言；readable silhouette /ˈriːdəbəl ˌsɪluˈet/ n. phr. 清楚易辨的轮廓；proportion /prəˈpɔːʃən/ n. 比例。

**译文**：人物设计：夸张的几何简化与出色材质细节相平衡。避免完全写实的人体结构；使用高层次形状语言、大而清楚的轮廓，适用时采用 Q 版比例。

### 08｜比例语言

**词汇释义**：friendly /ˈfrendli/ adj. 亲和的；head-tall /hed tɔːl/ adj. 以头高为单位的；childlike /ˈtʃaɪldlaɪk/ adj. 儿童般的；compact /kəmˈpækt/ adj. 紧凑的；recognizability /ˌrekəɡnaɪzəˈbɪləti/ n. 可辨识性。

**译文**：比例语言：亲和、风格化；可爱或儿童式人物通常为 2.5—3 头身，大头、紧凑身体、轮廓清楚、辨识度高。

### 09｜头发和毛发

**词汇释义**：sculpted clump /ˈskʌlptɪd klʌmp/ n. phr. 雕塑式发束；block shape /blɒk ʃeɪp/ n. phr. 块状形体；flyaway hair /ˈflaɪəweɪ heə/ n. phr. 飘散碎发；fuzzy rim /ˈfʌzi rɪm/ n. phr. 毛茸茸的边缘；tactile /ˈtæktaɪl/ adj. 有触感的。

**译文**：头发／毛发：强烈雕塑式发束与干净块状形体，结合边缘细碎飘发或毛绒轮廓细节，使毛发经过设计、又在光线下有真实触感。

### 10｜皮肤与材质

**词汇释义**：subsurface scattering /ˌsʌbˈsɜːfɪs ˈskætərɪŋ/ n. phr. 次表面散射；translucent /trænzˈluːsənt/ adj. 半透明的；reddish /ˈredɪʃ/ adj. 微红的；fingertip /ˈfɪŋɡətɪp/ n. 指尖；plastic /ˈplæstɪk/ adj. 塑料般的。

**译文**：皮肤／材质：温暖的次表面散射皮肤质感，柔和半透明红光透过耳朵、面颊、鼻子和指尖；避免硬塑料皮肤。

### 11｜表演与运动

**词汇释义**：lively /ˈlaɪvli/ adj. 生动的；squash-and-stretch /skwɒʃ ənd stretʃ/ n. phr. 挤压拉伸；brow /braʊ/ n. 眉；pupil /ˈpjuːpəl/ n. 瞳孔；line of action /laɪn əv ˈækʃən/ n. phr. 动作线；forward lean /ˈfɔːwəd liːn/ n. phr. 前倾；anticipation /ænˌtɪsɪˈpeɪʃən/ n. 预备动作；elastic body mechanics /ɪˈlæstɪk ˈbɒdi mɪˈkænɪks/ n. phr. 弹性身体运动机制；micro-expression /ˈmaɪkrəʊ ɪkˈspreʃən/ n. 微表情。

**译文**：表演风格：夸张、生动的迪士尼／皮克斯式人物动画，有挤压拉伸及显著的眉部、眼角、瞳孔、嘴唇和面颊形状变化。运动风格：高能量姿态、清楚动作线、前倾、强预备动作、快但易读的时序、富有弹性的身体运动和鲜活微表情。

### 12｜情感范围与负面限制

**词汇释义**：cuteness /ˈkjuːtnəs/ n. 可爱感；explosive expressiveness /ɪkˈspləʊsɪv ɪkˈspresɪvnəs/ n. phr. 爆发性表现力；deformation /ˌdiːfɔːˈmeɪʃən/ n. 变形；appeal /əˈpiːl/ n. 吸引力；photorealistic /ˌfəʊtəʊrɪəˈlɪstɪk/ adj. 照片级写实的；mannequin /ˈmænɪkɪn/ n. 人体模特；stiffness /ˈstɪfnəs/ n. 僵硬；lifeless /ˈlaɪfləs/ adj. 无生气的。

**译文**：情感范围：平衡可爱感与爆发性表现力；强烈情绪可以使用戏剧化面部形变，但保留人物魅力。负面风格限制：不使用照片级真人实拍、平面二维动漫、塑料玩具皮肤、僵硬人体模特姿势、写实人体结构式僵硬或无生气表情。

## STEP 0｜需求接收与画布计划

### 13｜采集创意与交付范围

**词汇释义**：rough premise /rʌf ˈpremɪs/ n. phr. 初步故事前提；blueprint /ˈbluːprɪnt/ n. 制作蓝图；asset /ˈæset/ n. 素材；extracted /ɪkˈstræktɪd/ adj. 已提取的；assembled /əˈsembəld/ adj. 已组接的。

**译文**：采集一句话创意或初步故事前提，以及想要的输出：仅蓝图、仅素材、带逐秒指令的标准镜头表、单份文字分镜文档（默认）加密集迭代镜头的独立文字节点及主动选用的多格铅笔分镜、单镜头片段（模型在步骤 7 选择）、组接主视频，或最终配乐合成影片。

### 14｜采集时长、画幅与声音要求

**词汇释义**：approximate length /əˈprɒksɪmət leŋθ/ n. phr. 大致片长；aspect ratio /ˈæspekt ˈreɪʃiəʊ/ n. phr. 宽高比；visual tone /ˈvɪʒuəl təʊn/ n. phr. 视觉基调；voiceover /ˈvɔɪsəʊvə/ n. 画外音；speech /spiːtʃ/ n. 说话声；default /dɪˈfɔːlt/ v. 默认采用。

**译文**：用户已说明时，记录大致片长和画面尺寸／宽高比；视觉基调默认温暖风格化三维动画；记录对白要求，即有对白、画外音或不说话。只有用户明确说明时才记录对白语言，不默认使用英语对白。

### 15｜立即确认制作格式

**词汇释义**：capture /ˈkæptʃə/ v. 采集；production format /prəˈdʌkʃən ˈfɔːmæt/ n. phr. 制作格式；landscape /ˈlændskeɪp/ adj. 横向的；vertical /ˈvɜːtɪkəl/ adj. 竖向的；square /skweə/ adj. 方形的；portrait /ˈpɔːtrət/ adj. 竖幅的；custom /ˈkʌstəm/ adj. 自定义的。

**译文**：采集用户输入后，项目简报或其他任何步骤之前，立即展示格式确认卡。画面尺寸／宽高比选项为：16:9 横幅（电影短片推荐）；9:16 竖向短片；1:1 方形；4:5 社交平台竖幅；自定义尺寸／比例。总时长选项为：30—60 秒（推荐）；15—30 秒；60—90 秒；90—180 秒；自定义时长。

### 16｜两项都确认后才能继续

**词汇释义**：proceed /prəˈsiːd/ v. 继续；supply /səˈplaɪ/ v. 提供；transition continuity /trænˈzɪʃən ˌkɒntɪˈnjuːəti/ n. phr. 转场连贯性；matching /ˈmætʃɪŋ/ n. 匹配；setting /ˈsetɪŋ/ n. 设置。

**译文**：用户选定画面尺寸／比例与总时长，或明确提供自定义值后，才能继续。将已确认值存入项目简报，并在镜头时间、转场连贯性、逐秒标准镜头表、单镜头分镜（默认文字，可选铅笔图）、单镜头片段、组接、背景音乐匹配和最终合成设置中复用。

### 17｜画布产物顺序

**词汇释义**：labeled /ˈleɪbəld/ adj. 带标签的；environment-only /ɪnˈvaɪrənmənt ˈəʊnli/ adj. 仅环境的；section /ˈsekʃən/ n. 小节；marker /ˈmɑːkə/ n. 标记；durable /ˈdjʊərəbəl/ adj. 需要持久保存的；dump /dʌmp/ v. 一股脑放出。

**译文**：依次创建或更新：1. 项目简报文本节点；2. 故事大纲文本节点；3. 带标签人物卡图像节点；4. 纯环境场景卡图像节点；5. 六列标准镜头信息表，逐行在 `Shot Description` 内包含逐秒指令；6. 一个 `<title> text storyboards` 文本节点，每镜头一节，沿用半旁白式结构，密集迭代镜头提取独立节点并在文档留下 `(extracted)`，主动选用铅笔图时另建图像节点；7. 所选模型生成的单镜头片段节点；8. 已组接主视频节点；9. 匹配背景音乐音频节点，以及最终背景音乐合成视频节点。不要只在聊天中堆积长制作内容，应把持久产物放到画布的文本、图像、视频或音频节点。

## STEP 1｜项目简报

### 18｜创建简报节点

**词汇释义**：concise /kənˈsaɪs/ adj. 简洁的；project title /ˈprɒdʒekt ˈtaɪtəl/ n. phr. 项目标题；text node /tekst nəʊd/ n. phr. 文本节点。

**译文**：编写简洁项目简报，写入以项目标题或 `项目简报` 命名的画布文本节点。

### 19｜简报内容

**词汇释义**：working title /ˈwɜːkɪŋ ˈtaɪtəl/ n. phr. 暂定标题；What-if /wɒt ɪf/ n. 假设性故事设想；emotional premise /ɪˈməʊʃənəl ˈpremɪs/ n. phr. 情感前提；target audience /ˈtɑːɡɪt ˈɔːdiəns/ n. phr. 目标观众；deliverable /dɪˈlɪvərəbəl/ n. 交付物；unspecified /ˌʌnˈspesɪfaɪd/ adj. 未指定的；initial risk /ɪˈnɪʃəl rɪsk/ n. phr. 初始风险；intent /ɪnˈtent/ n. 意图。

**译文**：包括暂定标题、一句话 What-if 设想、情感前提、目标观众感受、计划的主要交付物、已确认尺寸／比例、已确认总时长、对白模式与语言、初始风险，以及有对白时的对白意图。仅用户明确要求时使用具体语言；否则写 `language not specified`，对白保持最少，或需要时稍后再问。

### 20｜简报确认

**词汇释义**：regenerate /ˌriːˈdʒenəreɪt/ v. 重新生成；revise /rɪˈvaɪz/ v. 修订；refine /rɪˈfaɪn/ v. 细化；direction /dəˈrekʃən/ n. 方向。

**译文**：选择卡片包括：按此方向继续（推荐）；重新生成故事前提选项；修订情感前提；细化对白方向。用户作出选择或明确说继续后，才能前进。

## STEP 2｜故事大纲与关口

### 21｜大纲字段

**词汇释义**：protagonist /prəˈtæɡənɪst/ n. 主角；want /wɒnt/ n. 想要获得的东西；need /niːd/ n. 真正需要；flaw /flɔː/ n. 缺陷；world rule /wɜːld ruːl/ n. phr. 世界规则；causal story spine /ˈkɔːzəl ˈstɔːri spaɪn/ n. phr. 因果故事主干；payoff /ˈpeɪɒf/ n. 铺垫兑现；red-line check /red laɪn tʃek/ n. phr. 底线检查。

**译文**：创建名为 `故事大纲` 或 `story-outline` 的画布文本节点。包括主角的想要／需要／缺陷、核心世界规则、八节拍因果故事主干、情感锚点及其兑现、用户要求对白时的对白节拍，以及底线检查。

### 22｜故事关口检查

**词汇释义**：active /ˈæktɪv/ adj. 主动的；crisis /ˈkraɪsɪs/ n. 危机；intensify /ɪnˈtensɪfaɪ/ v. 加剧；coincidence /kəʊˈɪnsɪdəns/ n. 巧合；antagonistic pressure /ænˌtæɡəˈnɪstɪk ˈpreʃə/ n. phr. 对抗性压力；flat villain /flæt ˈvɪlən/ n. phr. 扁平反派；relationship change /rɪˈleɪʃənʃɪp tʃeɪndʒ/ n. phr. 关系变化；theme /θiːm/ n. 主题。

**译文**：检查主角是否主动行动；危机是否因主角缺陷而加剧；问题不能靠巧合解决；结尾要复用较早的情感锚点；对抗性压力不能只是扁平反派；对白应揭示关系变化，而非直接解释主题。

### 23｜大纲确认

**词汇释义**：beat /biːt/ n. 叙事节拍；emotion curve /ɪˈməʊʃən kɜːv/ n. phr. 情绪曲线；return /rɪˈtɜːn/ v. 返回。

**译文**：选择卡片包括：确认故事并继续（推荐）；修订节拍；修订情绪曲线；修订对白节拍；返回故事前提。

## STEP 3｜人物卡

### 24｜生成与推荐顺序

**词汇释义**：reference card /ˈrefərəns kɑːd/ n. phr. 参考卡；contrast /ˈkɒntrɑːst/ n. 对照；pressure character /ˈpreʃə ˈkærəktə/ n. phr. 施压人物；supporting character /səˈpɔːtɪŋ ˈkærəktə/ n. phr. 配角。

**译文**：生成人物参考卡，把每张图放入画布。推荐顺序为主角卡、对照／施压人物卡，以及可选配角卡。

### 25｜人物卡形式与标记

**词汇释义**：production reference sheet /prəˈdʌkʃən ˈrefərəns ʃiːt/ n. phr. 制作用参考图；downstream /ˌdaʊnˈstriːm/ adj. 后续流程的；bind /baɪnd/ v. 绑定；role label /rəʊl ˈleɪbəl/ n. phr. 角色功能标签；thief /θiːf/ n. 小偷；sidekick /ˈsaɪdkɪk/ n. 伙伴、助手；three-quarter view /ˌθriː ˈkwɔːtə vjuː/ n. phr. 四分之三角度视图。

**译文**：条件允许时，每张人物卡为 16:9 制作参考图。不同于最终视频，人物卡应有清楚可读标签，让后续生成绑定正确人物与道具。包含英语和／或项目语言的人物名称；角色标签，如主角、奶奶、小偷、伙伴、施压人物；主四分之三角度视图；正面／侧面／背面；表情。

### 26｜细节与身份锁定

**词汇释义**：material /məˈtɪəriəl/ n. 材质；handbag /ˈhændbæɡ/ n. 手提包；wallet /ˈwɒlɪt/ n. 钱包；skateboard /ˈskeɪtbɔːd/ n. 滑板；scarf /skɑːf/ n. 围巾；visual ID /ˈvɪʒuəl aɪ diː/ n. phr. 视觉身份标识；age range /eɪdʒ reɪndʒ/ n. phr. 年龄范围；body type /ˈbɒdi taɪp/ n. phr. 体型；do-not-change trait /duː nɒt tʃeɪndʒ treɪt/ n. phr. 禁止改变的特征。

**译文**：另包括材质／服装／道具细节；重要道具标签，如手提包、钱包、滑板、苹果筐、围巾、鞋、眼镜；在提示词中重复身份锁定；以及简短视觉身份注记，列出年龄范围、体型、发型、衣服颜色、标志性道具和不可更改特征。风格化三维动画人物应柔和、易读，并在后续图片和视频中保持一致。

### 27｜人物确认与改版成本

**词汇释义**：lock /lɒk/ v. 锁定；specific visual detail /spəˈsɪfɪk ˈvɪʒuəl ˈdiːteɪl/ n. phr. 特定视觉细节；warn /wɔːn/ v. 提醒；require /rɪˈkwaɪə/ v. 需要。

**译文**：主要人物卡生成后，展示：锁定人物设计并继续（推荐）；重新生成主角卡；调整特定视觉细节；增加人物卡。提醒用户：之后更改已锁定人物设计，可能需要重新生成镜头表、单镜头分镜、片段、组接主视频与最终合成。

## STEP 4｜场景卡

### 28｜纯环境限制

**词汇释义**：environment-only /ɪnˈvaɪrənmənt ˈəʊnli/ adj. 纯环境的；crowd figure /kraʊd ˈfɪɡə/ n. phr. 人群形象；cameo /ˈkæmiəʊ/ n. 短暂客串形象；belong /bɪˈlɒŋ/ v. 属于。

**译文**：生成场景参考卡，放在人物卡之后。场景卡只显示环境，不得有人物、人群、剪影、手、脸或角色客串。人物动作属于镜头表、单镜头多格铅笔分镜和单镜头片段，不属于场景卡。

### 29｜场景卡内容

**词汇释义**：overview /ˈəʊvəvjuː/ n. 总览；light state /laɪt steɪt/ n. phr. 光照状态；emotional sub-space /ɪˈməʊʃənəl sʌb speɪs/ n. phr. 承载情感的局部空间；continuity landmark /ˌkɒntɪˈnjuːəti ˈlændmɑːk/ n. phr. 连贯性标志物；persist /pəˈsɪst/ v. 保持；mailbox /ˈmeɪlbɒks/ n. 信箱。

**译文**：包括主要环境总览、白天／夜晚等关键光照状态、情感局部空间、连续性标志物及环境中的重要道具。标志物是同场景跨镜头必须保持画面位置的固定物体，例如厨房中岛、沙发、门框、树、信箱。

### 30｜场景确认

**词汇释义**：angle /ˈæŋɡəl/ n. 观察角度；lighting /ˈlaɪtɪŋ/ n. 光照；layout /ˈleɪaʊt/ n. 布局。

**译文**：选择卡片包括：锁定场景设计并继续（推荐）；重新生成场景卡；增加场景角度；调整光照或布局。

## STEP 5｜标准化镜头表视频提示词（六列）

### 31｜必需参考与最小执行约定

**词汇释义**：mandatory /ˈmændətəri/ adj. 必需的；schema /ˈskiːmə/ n. 结构规范；minimum runtime contract /ˈmɪnɪməm ˈrʌntaɪm ˈkɒntrækt/ n. phr. 最小执行约定；table-wide rule /ˈteɪbəl waɪd ruːl/ n. phr. 全表规则；approval /əˈpruːvəl/ n. 确认。

**译文**：人物卡和场景卡锁定后，用镜头信息表输出标准化视频提示词。这一步必须执行，不可与分镜或视频生成调换。必读并遵循 `references/shot-table-spec.md`，以获取精确六列结构、逐秒要求、全表规则、用户确认卡和必需的步骤 5.5 自检关口。

### 32｜六列及自检条件

**词汇释义**：continuity handoff /ˌkɒntɪˈnjuːəti ˈhændɒf/ n. phr. 连贯性衔接；reference anchor /ˈrefərəns ˈæŋkə/ n. phr. 参考锚点；hook type /hʊk taɪp/ n. phr. 抓手类型；audio/dialogue timing /ˈɔːdiəʊ ˈdaɪəlɒɡ ˈtaɪmɪŋ/ n. phr. 音频／对白时序。

**译文**：创建 `标准镜头信息表` 或 `standard-shot-table` 节点，严格使用六列：`Shot ID & Duration`、`Continuity Handoff`、`Reference Anchors (Spatial + Identity)`、`Hook Type`、`Shot Description (Per-Second Directives)`、`Audio & Dialogue Track`。每行必须有完整逐秒指令、前后衔接、参考锚点、抓手类型、音频和对白时间。制作分镜前运行参考文件规定的步骤 5.5 自检，未通过不可进入步骤 6。随后显示该参考文件定义的表格确认／自检卡片。

## STEP 6｜文字分镜文档与主动选用的铅笔图

### 33｜必读指南与模式确认

**词汇释义**：shot-level extraction /ʃɒt ˈlevəl ɪkˈstrækʃən/ n. phr. 镜头级提取；re-integration /ˌriːɪntɪˈɡreɪʃən/ n. 重新整合；visualization fallback /ˌvɪʒuəlaɪˈzeɪʃən ˈfɔːlbæk/ n. phr. 可视化回退。

**译文**：步骤 5.5 自检通过后，在创建任何分镜产物前先显示模式卡。必读 `references/storyboard-guidelines.md`，遵循默认单一文字文档、可选多格铅笔图、镜头级提取／重新整合、分镜确认卡和可视化回退规则。

### 34｜文字权威与独立节点

**词汇释义**：authoritative /ɔːˈθɒrɪtətɪv/ adj. 作为权威依据的；override /ˌəʊvəˈraɪd/ v. 取代；flag /flæɡ/ v. 标记；matching /ˈmætʃɪŋ/ adj. 匹配的。

**译文**：最小执行约定：默认只有一份权威文字分镜文档，每镜头一节；铅笔图仅为用户主动选用的可视化产物，绝不取代文字分镜；只有用户将某镜头标为密集迭代时，才提取独立文字节点；步骤 7 读取匹配文字小节或独立节点，不读取铅笔图。全部分镜确认后，进入视频模型选择卡片。

## STEP 7｜视频模型选择与单镜头片段

### 35｜模型和回退参考

**词汇释义**：model-specific /ˈmɒdəl spəˈsɪfɪk/ adj. 模型特定的；prompt shaping /prɒmpt ˈʃeɪpɪŋ/ n. phr. 提示词组织；retry ladder /ˌriːˈtraɪ ˈlædə/ n. phr. 重试阶梯；drift handling /drɪft ˈhændlɪŋ/ n. phr. 漂移处理；escalation /ˌeskəˈleɪʃən/ n. 逐级处理。

**译文**：任何片段渲染前，先显示模型与分辨率卡。必读 `references/model-selection.md`，了解 H3 默认、Seedance 2.0 回退、逐镜头混合、分辨率和模型特定提示词；必读 `references/fallback-policy.md`，了解各模型重试阶梯、漂移处理与逐级处理选择。

### 36｜逐镜头执行要求

**词汇释义**：high-stakes /ˌhaɪˈsteɪks/ adj. 成败影响较大的；repeated failure /rɪˈpiːtɪd ˈfeɪljə/ n. phr. 重复失败；unmarked /ʌnˈmɑːkt/ adj. 未标记的；strip /strɪp/ v. 去除；silently /ˈsaɪləntli/ adv. 未告知地；incorrect /ˌɪnkəˈrekt/ adj. 不正确的。

**译文**：H3 为推荐默认模型；对动画表演要求关键或 H3 反复失败时，Seedance 2.0 作回退。只有表格逐行标注模型时才允许混合，未标记行默认 H3。视频渲染前移除全部分镜专用标签。每段绑定已确认文字分镜、准确人物卡及准确场景卡。片段偏离已确认 `Reference Anchors` 时遵循回退文件，不得悄悄组接错误片段。

### 37｜片段分组和确认

**词汇释义**：shot order /ʃɒt ˈɔːdə/ n. phr. 镜头顺序；group /ɡruːp/ v. 分组；defined /dɪˈfaɪnd/ adj. 已定义的。

**译文**：全部片段渲染后，按镜头顺序放到画布，分组为 `<title> shot clips`，再显示源文所指 `references/model-selection.md` 中的片段确认卡。

**译注**：实际完整片段确认选项位于同目录 `references/fallback-policy.md`。源文上述引用按原样保留，未回写修订。

## STEP 8｜组接、背景音乐匹配与最终输出

### 38｜流程与参考文件

**词汇释义**：continuous track /kənˈtɪnjuəs træk/ n. phr. 连续音轨；composited video /ˈkɒmpəzɪtɪd ˈvɪdiəʊ/ n. phr. 合成视频；grouping discipline /ˈɡruːpɪŋ ˈdɪsəplɪn/ n. phr. 分组规范；latest asset /ˈleɪtɪst ˈæset/ n. phr. 最新素材。

**译文**：全部单镜头片段确认后，组接完整主视频，匹配或生成一条连续背景音乐，再输出最终合成。必读 `references/qc-checklist.md`，遵循组接、背景音乐、最终审阅、画布排序与分组、用户选择卡、重新生成及最新素材规范。

### 39｜最小交付约定

**词汇释义**：preserve /prɪˈzɜːv/ v. 保留；duck /dʌk/ v. 压低音量；reaction /riˈækʃən/ n. 反应；SFX abbr. Sound Effects，音效；trace /treɪs/ n. 痕迹；panel border /ˈpænəl ˈbɔːdə/ n. phr. 画格边框。

**译文**：严格保留已确认表格镜头顺序；只用最新已确认素材；对白、反应和重要音效出现时压低背景音乐；无明确要求不加字幕或文字；最终视频不得含分镜痕迹、标签、箭头、时间标记、画格边框或双重绑定标签。然后执行 `references/qc-checklist.md` 的最终审阅，交付最终已确认产物。

## Boundaries｜适用边界

### 40｜不适用任务

**词汇释义**：simple edit /ˈsɪmpəl ˈedɪt/ n. phr. 简单编辑；logo design /ˈləʊɡəʊ dɪˈzaɪn/ n. phr. 标志设计；pure prompt consultation /pjʊə prɒmpt ˌkɒnsəlˈteɪʃən/ n. phr. 纯提示词咨询；character breakdown /ˈkærəktə ˈbreɪkdaʊn/ n. phr. 人物拆解。

**译文**：不要将此 Skill 用于单图、简单编辑、单片段动画、标志设计或纯提示词咨询。用户只要提示词时，使用视频提示词流程；用户只要人物卡时，使用人物拆解流程。
