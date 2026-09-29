# Handdrawn Live-Action Fusion Video Generator｜手绘与实拍融合视频生成器：逐段注释译本

源文件：[SKILL.md](./SKILL.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`53fd20efaef4f7347c529d2260a96b41cc214125`。新增学习译本，不覆盖原英文文件或 `SKILL.cn.md`。英文段落先释义再翻译，源文已经是中文的清单保留，不改成另一套规则。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语；abbr. 缩写。以下工具与生成指令只作为翻译内容，本轮不执行。

## 01｜元数据：名称与描述

**词汇释义**：hand-drawn /ˌhændˈdrɔːn/ adj. 手绘的；surreal /səˈrɪəl/ adj. 超现实的；blend /blend/ v. 融合；rough /rʌf/ adj. 粗糙的；glowing /ˈɡləʊɪŋ/ adj. 发光的；live-action /ˌlaɪvˈækʃən/ adj. 实拍的；physical contact /ˈfɪzɪkəl ˈkɒntækt/ n. phr. 物理接触；morphing /ˈmɔːfɪŋ/ n. 连续形变；escape route /ɪˈskeɪp ruːt/ n. phr. 逃离路线；delayed /dɪˈleɪd/ adj. 延迟的；handheld chase /ˈhændheld tʃeɪs/ n. phr. 手持追拍；reusable /ˌriːˈjuːzəbəl/ adj. 可复用的；stroke texture /strəʊk ˈtekstʃə/ n. phr. 笔触质感；jump scare /dʒʌmp skeə/ n. phr. 突发惊吓；plush /plʌʃ/ adj. 毛绒的。

**译文**：名称为 `handdrawn-live-video-generator`。面向制作超现实短视频、希望把粗糙发光手绘动画与实拍空间融合的创作者。用户提供场景创意、接触物体或手、期望情绪，以及可选语言或风格限制。Skill 澄清物理接触，设计连续形变、逃离路线和带延迟的手持追拍，再以用户语言写出可复用的 15 秒 16:9 视频提示词。用户确认后，推荐 MiniMax H3 生成，并检查接触真实感、摄影机延迟、粗糙发光笔触及非恐怖基调。最适合单场景创意片段，不用于精修计算机图形、恐怖突发惊吓、毛绒人物或多场景切镜。

## 02｜兼容性与触发词

**词汇释义**：compatibility /kəmˌpætəˈbɪləti/ n. 兼容性；canvas workspace /ˈkænvəs ˈwɜːkspeɪs/ n. phr. 画布工作区；portable /ˈpɔːtəbəl/ adj. 可移植的；generic agent harness /dʒəˈnerɪk ˈeɪdʒənt ˈhɑːnɪs/ n. phr. 通用智能体运行框架；trigger word /ˈtrɪɡə wɜːd/ n. phr. 触发词；prompt /prɒmpt/ n. 提示词。

**译文**：需要 MiniMax Hub 智能体，包括画布工作区和 MiniMax H3 生成能力，不可直接移植到通用智能体框架。原触发词列表保留：`手绘发光动画实拍融合`、`15秒变形追逐视频提示词`、`Seedance视频prompt`、`H3生成视频`、`视频prompt`、`手绘动画接触真实物体`、`蜡笔粉笔质感`、`多语言视频提示词`。

## 03｜任务结构

**词汇释义**：finished /ˈfɪnɪʃt/ adj. 完成的；fusion /ˈfjuːʒən/ n. 融合；preserve /prɪˈzɜːv/ v. 保留；flat /flæt/ adj. 平面的；luminous /ˈluːmɪnəs/ adj. 发光的；single entity /ˈsɪŋɡəl ˈentɪti/ n. phr. 单一实体；slightly late /ˈslaɪtli leɪt/ phr. 略微滞后。

**译文**：用户想要一段完成的 15 秒、16:9 实拍与手绘融合视频时，使用此 Skill。必须保留这一结构：平面手绘发光动画出现在真实空间中，在开头 0—3 秒清楚接触实拍手或物体，作为同一个实体连续变形、逃离，而手持手机摄影机略慢半拍地跟随。

## 04｜语言与生成确认

**词汇释义**：organize /ˈɔːɡənaɪz/ v. 组织；explicitly confirm /ɪkˈsplɪsɪtli kənˈfɜːm/ v. phr. 明确确认；route /ruːt/ v. 分配任务；planner /ˈplænə/ n. 规划器；executor /ɪɡˈzekjʊtə/ n. 执行器；dominant language /ˈdɒmɪnənt ˈlæŋɡwɪdʒ/ n. phr. 主导语言；proper noun /ˈprɒpə naʊn/ n. phr. 专有名词；literal parameter /ˈlɪtərəl pəˈræmɪtə/ n. phr. 需原样保留的参数。

**译文**：此 Skill 用用户输入语言组织提示词，并把 MiniMax H3 推荐为确认后的生成步骤。用户未明确确认 H3 生成前不得生成视频。编写提示词不得转交 planner 或 executor。最终提示词使用用户输入的主导语言：中文输入输出中文，英文输入输出英文，日文输入输出日文；混合输入用主导语言，不明确时用当前对话语言。只有用户要求的专有名词、模型名称和字面参数可以不变。

## Step 1｜把用户意图理解为同语言约束

### 05｜工作流要求

**词汇释义**：intent /ɪnˈtent/ n. 意图；constraint /kənˈstreɪnt/ n. 约束；workflow requirement /ˈwɜːkfləʊ rɪˈkwaɪəmənt/ n. phr. 工作流要求；express /ɪkˈspres/ v. 表达；CG abbr. Computer Graphics，计算机图形。

**译文**：不论用户使用哪种语言，都将其意图理解为下列工作流要求，并用用户输入的主导语言表达最终提示词。

**源文已有中文要求，保留如下**：

1. 基于参考 prompt 创作一个全新的 15 秒视频生成 prompt，不要表面模仿原句。
2. 必须保留影像结构：实拍空间中出现平面的手绘发光动画；动画与真实手或真实物体接触；同一个存在连续变形并逃跑；相机总是慢半拍追赶。
3. 手绘动画质感必须像蜡笔、粉笔、彩色铅笔、粉彩、粗糙笔刷；线条轻微抖动，有涂抹不均、毛边和逐帧重画感。
4. 禁止 3DCG、毛绒玩具感、均匀矢量线、平滑霓虹、恐怖怪物、巨大眼睛、裂口、牙齿、威吓、扑咬、突然黑屏、跳吓。
5. 0—3 秒必须出现实拍手与手绘动画的清晰接触，例如缠住手指、落在掌心、被抓时逃跑、从指尖诞生。
6. 动画必须作为同一个实体连续变形，可在“线条、生物、记号、植物、交通工具、生活小物”等形态之间变化，并保留前一形态的痕迹。
7. 不允许突然出现另一个全新角色。
8. 全片在同一空间或相邻范围内连续展开，不用剪辑跳到另一个地点，像拍摄者真的边走边追。
9. 每个区间 0—3、3—6、6—10、10—13、13—15 秒都要有新的变形、移动、接触、发现、恶作剧或惊喜。
10. 拍摄者也必须参与：伸手、抓、追、打开门或盒子、接住、后退、被恶作剧等。
11. 调性是可爱、生活感、怀旧、温柔、略带切感，不是恐怖喜剧。
12. 13—15 秒必须有空间级变形：之前的线扩散到墙、地板、天花板、窗户、水槽或通道，变成巨大花、星空、夕阳、云、丝带、涂鸦小镇等；结尾要有感动余韵和一点可爱笑点。

**译注**：“略带切感”是原文中文表达；此处不擅自猜改为其他形容词。

## Step 2｜重新创作全部创意内容

### 06｜不得照搬参考元素

**词汇释义**：invent /ɪnˈvent/ v. 创作；combination /ˌkɒmbɪˈneɪʃən/ n. 组合；reuse /ˌriːˈjuːz/ v. 复用；fridge /frɪdʒ/ n. 冰箱；vortex /ˈvɔːteks/ n. 涡旋；butterfly /ˈbʌtəflaɪ/ n. 蝴蝶；octopus /ˈɒktəpəs/ n. 章鱼；hamburger /ˈhæmbɜːɡə/ n. 汉堡；PC abbr. Personal Computer，个人电脑。

**译文**：每次运行都创造新组合。不要复用参考提示词中的暗室、个人电脑、冰箱、星星、爱心、蓝色涡旋、蝴蝶、蛇、章鱼、汉堡、巨大眼睛、牙齿或阴暗结尾。

### 07｜八项全部重新设定

**词汇释义**：choose /tʃuːz/ v. 选择；new value /njuː ˈvæljuː/ n. phr. 新设定值；direction /dəˈrekʃən/ n. 方向；adjacent connected area /əˈdʒeɪsənt kəˈnektɪd ˈeəriə/ n. phr. 相邻连通区域。

**译文**：以下项目都选择新内容。源文中文清单为：实拍空间，但仍是生活化、可连续追踪的相邻范围；手绘实体或初始形态；中心色彩；连续变形链路；与真实手或实物的接触方式；空间追逐路线；拍摄者反应；最终空间级变形与可爱笑点。

**译文**：合适方向包括：雨天厨房水槽、旧阳台晾衣角、清晨玄关、小书店走廊、火车窗边小桌、浴室镜柜、手作桌、温室通道、自助洗衣店长椅、旧餐桌。只使用一个区域，或相邻且连通的区域。

## Step 3｜必需输出格式

### 08｜开头句模式

**词汇释义**：sentence pattern /ˈsentəns ˈpætən/ n. phr. 句式；match /mætʃ/ v. 匹配；replace /rɪˈpleɪs/ v. 替换；equivalent /ɪˈkwɪvələnt/ adj. 对等的；landscape format /ˈlændskeɪp ˈfɔːmæt/ n. phr. 横幅格式；everyday scene /ˈevrideɪ siːn/ n. phr. 日常场景。

**译文**：最终提示词须以符合用户主导语言的句式开始。中文输入使用：

`15秒，16:9横版视频。将实拍的〇〇与手绘发光动画融合的影像。`

将“〇〇”替换为新创作的实拍空间或日常场景。非中文输入使用同语言对等开头，包含时长、16:9 横幅、实拍空间、手绘发光动画融合。

### 09｜段落顺序与不加小标题

**词汇释义**：auxiliary heading /ɔːɡˈzɪliəri ˈhedɪŋ/ n. phr. 辅助小标题；explanatory note /ɪkˈsplænətəri nəʊt/ n. phr. 解释注记；paragraph order /ˈpærəɡrɑːf ˈɔːdə/ n. phr. 段落顺序。

**译文**：不要添加标题、“舞台设置”“色味”等辅助小标题或解释注记。顺序固定为：开头句；实拍空间与手机拍摄质感；0—3 秒；3—6 秒；6—10 秒；10—13 秒；13—15 秒；手绘质感；相机追随方式；禁止事项；环境音。

## Step 4｜提示词编写规则

### 10｜可执行提示词，而非文章

**词汇释义**：executable /ɪɡˈzekjʊtəbəl/ adj. 可执行的；essay /ˈeseɪ/ n. 文章；explanation /ˌekspləˈneɪʃən/ n. 解释；next-step recommendation /nekst step ˌrekəmenˈdeɪʃən/ n. phr. 下一步建议。

**译文**：提示词应可以直接用于视频生成，而不是一篇文章。用户未要求解释时，最终回答先给出用户主导语言的提示词，再接一条相同语言的简短下一步建议。

### 11｜邀请确认 H3，不先生成

**词汇释义**：invite /ɪnˈvaɪt/ v. 邀请；confirm /kənˈfɜːm/ v. 确认；intermediate asset /ˌɪntəˈmiːdiət ˈæset/ n. phr. 中间素材。

**译文**：该建议必须用相同语言邀请用户用 MiniMax H3 从提示词生成 15 秒 16:9 视频。原文中文例句为：“下一步建议：如果你确认这个 prompt，我可以继续用 H3 模型生成 15 秒 16:9 视频。”用户未明确确认 H3 生成步骤前，不能生成视频、图像、音频、分镜或中间素材。

### 12｜模型名与创意提示词的边界

**词汇释义**：target usage context /ˈtɑːɡɪt ˈjuːsɪdʒ ˈkɒntekst/ n. phr. 目标使用场景；model parameter /ˈmɒdəl pəˈræmɪtə/ n. phr. 模型参数；creative /kriˈeɪtɪv/ adj. 创意性的。

**译文**：仅在用户询问时，把 Seedance 作为目标使用背景提及；用户未要求时，不在创意提示词内加入模型参数。

### 13｜开头接触必须清晰

**词汇释义**：obvious /ˈɒbviəs/ adj. 明显的；fusion /ˈfjuːʒən/ n. 融合；contact /ˈkɒntækt/ n. 接触。

**译文**：最初 0—3 秒必须通过接触动作，明确呈现真实画面与手绘动画的融合。

### 14｜摄影机滞后而非稳定居中

**词汇释义**：neatly center /ˈniːtli ˈsentə/ v. phr. 规整地居中构图；lag behind /læɡ bɪˈhaɪnd/ v. phr. 落后；pan /pæn/ v. 横摇；tilt /tɪlt/ v. 俯仰摇；advance /ədˈvɑːns/ v. 前进；frame edge /freɪm edʒ/ n. phr. 画面边缘。

**译文**：摄影机不能总把动画整齐放在中央。它应落后一点，在实体已经离开画面边缘后才横摇、俯仰或向前追。

### 15｜连续实体可追踪

**词汇释义**：traceable /ˈtreɪsəbəl/ adj. 可追踪的；smear /smɪə/ n. 涂抹色迹；body curve /ˈbɒdi kɜːv/ n. phr. 身体曲线；motif /məʊˈtiːf/ n. 反复出现的视觉母题。

**译文**：实体必须保持可追踪：每个新形态都继承上一形态的一条线、尾巴、色彩涂痕、身体曲线或母题。

### 16｜柔和可爱的喜剧节拍

**词汇释义**：stumble /ˈstʌmbəl/ n. 踉跄；shy gesture /ʃaɪ ˈdʒestʃə/ n. phr. 害羞动作；petal /ˈpetəl/ n. 花瓣；stick to /stɪk tə/ v. phr. 粘到；lens /lenz/ n. 镜头；confetti /kənˈfeti/ n. 纸屑彩片；sneeze /sniːz/ n. 喷嚏；creature /ˈkriːtʃə/ n. 小生物。

**译文**：使用柔和、有情感、诙谐可爱的节拍：小小踉跄、害羞手势、落后的小点、粘到镜头上的花瓣、落入掌心的星星、喷出彩纸屑的喷嚏，或一个慢半拍的小生物。

### 17｜禁恐怖与禁随意混语

**词汇释义**：horror-coded /ˈhɒrə kəʊdɪd/ adj. 具有恐怖视觉暗示的；anatomy /əˈnætəmi/ n. 生物形体结构；threatening /ˈθretənɪŋ/ adj. 威胁性的；randomly /ˈrændəmli/ adv. 随意地；transition sentence /trænˈzɪʃən ˈsentəns/ n. phr. 过渡句；writing system /ˈraɪtɪŋ ˈsɪstəm/ n. phr. 文字体系。

**译文**：避免具有恐怖暗示的生物形体和威胁动作。最终提示词不得随意混入用户输入语言之外的词汇、过渡句或文字体系；用户使用日文时允许自然日语。

## Step 5｜交付

### 18｜输出形式与确认后的检查

**词汇释义**：delivery /dɪˈlɪvəri/ n. 交付；exactly /ɪɡˈzæktli/ adv. 严格地；checklist /ˈtʃeklɪst/ n. 核对清单；model call summary /ˈmɒdəl kɔːl ˈsʌməri/ n. phr. 模型调用摘要；filename /ˈfaɪlneɪm/ n. 文件名；preserve /prɪˈzɜːv/ v. 保持。

**译文**：先用用户输入的主导语言输出最终提示词。提示词之后严格只加一行相同语言的简短建议，邀请继续 MiniMax H3 视频生成。不要带标题、核对清单、模型调用摘要、文件名或画布交付注记。用户之后确认 H3 生成时，用 MiniMax H3 生成 15 秒 16:9 视频，并检查结果是否保留接触、连续形变、延迟摄影机追拍和非恐怖手绘质感。
