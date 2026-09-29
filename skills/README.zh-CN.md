# MiniMax H3 Skills｜逐段词汇注释与简体中文译本

源文件：[README.md](./README.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`c030de54dbc0798e680140b657fc7c79e9ef9a48`。本文件为独立学习译本，不覆盖原文件。各段按源文次序先释义，再翻译。n. 名词；v. 动词；adj. 形容词；adv. 副词；n. phr. 名词短语；v. phr. 动词短语；abbr. 缩写。命令、标识符与路径保持原样；本文不执行所翻译的安装或生成指令。

## 01｜目录内容

**词汇释义**：directory /dəˈrektəri/ n. 目录；skill /skɪl/ n. 技能模块；bundled /ˈbʌndəld/ adj. 随包附带的；prompt writing /prɒmpt ˈraɪtɪŋ/ n. phr. 提示词编写；style-specific /staɪl spəˈsɪfɪk/ adj. 特定风格的；installable /ɪnˈstɔːləbəl/ adj. 可安装的；reference material /ˈrefərəns məˈtɪəriəl/ n. phr. 参考资料。

**译文**：本目录包含 [MiniMax H3](../README.md) 附带的 Skill：1 个提示词编写 Skill 和 8 个特定风格视频生成 Skill。每个 Skill 都有独立文件夹，其中包含可安装的 `SKILL.md`、所需参考资料，以及风格类 Skill 的中文版本 `SKILL.cn.md`。

## 02｜Status：状态

**词汇释义**：actively /ˈæktɪvli/ adv. 积极地、持续地；maintain /meɪnˈteɪn/ v. 维护；evolve /ɪˈvɒlv/ v. 演进；bilingual /baɪˈlɪŋɡwəl/ adj. 双语的；currently /ˈkʌrəntli/ adv. 当前。

**译文**：这些 Skill 正在持续维护，仍在演进。8 个风格 Skill 附有双语 `SKILL.md`／`SKILL.cn.md`；`h3-prompt-writing` 目前只有英文。

**译注**：“目前只有英文”对应源版本状态。本次新增学习译本并不回写或改动该源句。

## 03｜Installation：安装

**词汇释义**：install /ɪnˈstɔːl/ v. 安装；CLI abbr. Command-Line Interface，命令行界面；list /lɪst/ v. 列出；available /əˈveɪləbəl/ adj. 可用的；repository /rɪˈpɒzɪtəri/ n. 仓库；single /ˈsɪŋɡəl/ adj. 单个的。

**译文**：使用 [skills CLI](https://github.com/vercel-labs/skills) 安装 Skill：

```bash
# 列出此仓库中全部可用 Skill
npx skills add https://github.com/MiniMax-AI/MiniMax-H3 --list

# 安装全部 Skill
npx skills add https://github.com/MiniMax-AI/MiniMax-H3 --skill '*'

# 安装单个 Skill
npx skills add https://github.com/MiniMax-AI/MiniMax-H3 --skill h3-prompt-writing
```

## 04｜h3-prompt-writing：H3 提示词编写

源入口：[SKILL.md](h3-prompt-writing/SKILL.md)。

**词汇释义**：structured /ˈstrʌktʃəd/ adj. 结构化的；generation /ˌdʒenəˈreɪʃən/ n. 生成；rewrite /ˌriːˈraɪt/ v. 改写；multimodal /ˌmʌltiˈməʊdəl/ adj. 多模态的；request /rɪˈkwest/ n. 要求；integrated /ˈɪntɪɡreɪtɪd/ adj. 综合的；soundscape /ˈsaʊndskeɪp/ n. 声景；non-diegetic /ˌnɒn daɪəˈdʒetɪk/ adj. 非故事空间内声音的；align /əˈlaɪn/ v. 对齐；keyframe /ˈkiːfreɪm/ n. 关键帧；reference label /ˈrefərəns ˈleɪbəl/ n. phr. 参考标签。

**译文**：为 T2VA、I2VA、FL2VA、L2VA、Ref2VA 五种生成模式编写结构化的 MiniMax H3 视频生成提示词。该 Skill 将多模态要求改写为 H3 提示词结构，包括 `integrated_multimodal_description`、`overall_soundscape` 和 `non_diegetic_music`；同时对齐关键帧，并为图像、视频和音频定义参考标签。它在 [references/](h3-prompt-writing/references/) 下附带两份指南。

**词汇释义**：base /beɪs/ adj. 基础的；text /tekst/ n. 文本；mode /məʊd/ n. 模式；full-reference /fʊl ˈrefərəns/ adj. 全参考的。

**译文**：[base-en.txt](h3-prompt-writing/references/base-en.txt) 对应基础文本／关键帧模式；[ref-en.txt](h3-prompt-writing/references/ref-en.txt) 对应全参考 Ref2VA 模式。

## 05｜minimalist-product-ad-generator：极简产品广告生成器

![极简产品广告示例](../assets/minimalist-product-ad-generator.gif)

**词汇释义**：minimalist /ˈmɪnɪməlɪst/ adj. 极简主义的；e-commerce /ˈiːˌkɒmɜːs/ n. 电子商务；promotion /prəˈməʊʃən/ n. 推广；launch /lɔːntʃ/ n. 发布；variant /ˈveəriənt/ n. 变体、款式；extract /ɪkˈstrækt/ v. 提取；selling point /ˈselɪŋ pɔɪnt/ n. phr. 卖点；concise /kənˈsaɪs/ adj. 简洁的；ad copy /æd ˈkɒpi/ n. phr. 广告文案；beat-synced /biːt sɪŋkt/ adj. 与节拍同步的；typography /taɪˈpɒɡrəfi/ n. 字体编排；storyboard /ˈstɔːribɔːd/ n. 分镜；premium /ˈpriːmiəm/ adj. 高品质的；polished /ˈpɒlɪʃt/ adj. 精致成熟的；talking-head /ˈtɔːkɪŋ hed/ adj. 人物面对镜头口播的；demo /ˈdeməʊ/ n. 演示；KOC abbr. Key Opinion Consumer，关键意见消费者。

**译文**：将产品图像和广告要求转化为干净、极简的产品广告短片，用于电商推广和产品发布。该 Skill 确认画幅与产品款式，提取卖点，编写简洁英文广告文案，规划与节拍同步的字体编排和分镜，并以精致运镜语言生成高品质产品影片。它不适用于 KOC 人物口播广告、通用剪辑或复杂屏幕演示。

[英文源文件](minimalist-product-ad-generator/SKILL.md) · [原有中文版本](minimalist-product-ad-generator/SKILL.cn.md)

## 06｜3d-animation-short-generator：三维动画短片生成器

![三维动画短片示例](../assets/3d-animation-short-generator.gif)

**词汇释义**：stylized /ˈstaɪlaɪzd/ adj. 风格化的；ordered /ˈɔːdəd/ adj. 有序的；production workflow /prəˈdʌkʃən ˈwɜːkfləʊ/ n. phr. 制作流程；project brief /ˈprɒdʒekt briːf/ n. phr. 项目简报；outline /ˈaʊtlaɪn/ n. 大纲；environment card /ɪnˈvaɪrənmənt kɑːd/ n. phr. 环境设定卡；standardized /ˈstændədaɪzd/ adj. 标准化的；pencil storyboard /ˈpensəl ˈstɔːribɔːd/ n. phr. 铅笔分镜图；assembly /əˈsembli/ n. 组接；BGM abbr. Background Music，背景音乐；narrative /ˈnærətɪv/ adj. 叙事性的；consistency /kənˈsɪstənsi/ n. 一致性；continuity /ˌkɒntɪˈnjuːəti/ n. 连贯性；photorealistic /ˌfəʊtəʊrɪəˈlɪstɪk/ adj. 照片级写实的；standalone /ˈstændəˌləʊn/ adj. 独立的。

**译文**：从故事创意出发，通过有序制作流程创建完整的风格化三维动画短片：项目简报、故事大纲、人物与环境卡、标准化镜头规划、文字分镜或可选铅笔分镜、视频模型选择、单镜头生成、组接、背景音乐匹配，以及最终审阅。它面向端到端叙事动画，重视人物一致性、场景连贯性，以及时间、摄影机、表演和声音控制。不适用于单张图片、简单编辑、照片级真人实拍，或单个独立片段。

[英文源文件](3d-animation-short-generator/SKILL.md) · [原有中文版本](3d-animation-short-generator/SKILL.cn.md)

## 07｜papercraft-stop-motion-explainer：纸艺定格解说生成器

![纸艺定格示例](../assets/papercraft-stop-motion-explainer.gif)

**词汇释义**：tactile /ˈtæktaɪl/ adj. 有触感的；handmade /ˌhændˈmeɪd/ adj. 手工制作的；papercraft /ˈpeɪpəkrɑːft/ n. 纸艺；learning goal /ˈlɜːnɪŋ ɡəʊl/ n. phr. 学习目标；visual metaphor /ˈvɪʒuəl ˈmetəfə/ n. phr. 视觉隐喻；layered /ˈleɪəd/ adj. 分层的；diorama /ˌdaɪəˈrɑːmə/ n. 微缩立体景；prop /prɒp/ n. 道具；preview /ˈpriːvjuː/ n. 预览；staged approval /steɪdʒd əˈpruːvəl/ n. phr. 分阶段确认；production-ready /prəˈdʌkʃən ˈredi/ adj. 可直接用于制作的；cut-paper /kʌt ˈpeɪpə/ n. 剪纸；pop-up book /ˈpɒpʌp bʊk/ n. phr. 立体书；miniature /ˈmɪnətʃə/ adj. 微缩的。

**译文**：通过有触感的手工纸艺画面解释科学、教育或一般知识。该 Skill 提取学习目标和视觉隐喻，提出创意方向，设计纸艺人物、分层微缩布景与道具，创建预览概念以及图像和视频提示词，并通过阶段确认和审阅清单规划分镜、运镜、转场与声音。它输出可用于制作的纸艺定格解说总包，或选定资产，例如静帧提示词、系列图片提示词、短视频提示词或分镜。最适合剪纸、立体书、分层微缩景观及微缩定格解说。

[英文源文件](papercraft-stop-motion-explainer/SKILL.md) · [原有中文版本](papercraft-stop-motion-explainer/SKILL.cn.md)

## 08｜brand-promo-video-generator：品牌宣传视频生成器

![品牌宣传示例](../assets/brand-promo-video-generator.gif)

**词汇释义**：marketer /ˈmɑːkɪtə/ n. 营销人员；promotional /prəˈməʊʃənəl/ adj. 宣传推广的；provenance /ˈprɒvənəns/ n. 素材来源；narrative direction /ˈnærətɪv dəˈrekʃən/ n. phr. 叙事方向；precise beat /prɪˈsaɪs biːt/ n. phr. 精确的叙事节拍；imagery /ˈɪmɪdʒəri/ n. 图像内容；voiceover /ˈvɔɪsəʊvə/ n. 画外音；pre-delivery /priː dɪˈlɪvəri/ adj. 交付前的；capability /ˌkeɪpəˈbɪləti/ n. 能力；use case /juːs keɪs/ n. phr. 使用场景；call to action /kɔːl tə ˈækʃən/ n. phr. 行动号召；showcase /ˈʃəʊkeɪs/ n. 展示；authorized /ˈɔːθəraɪzd/ adj. 已授权的；claim /kleɪm/ n. 宣传主张。

**译文**：面向为品牌、产品、网站、应用、店铺或个人项目制作宣传内容的营销人员和创作者。该 Skill 整理品牌事实与素材出处，选定叙事方向，规划精确节拍与镜头，生成需要的图片、视频、画外音或音乐，并完成组接和交付前审阅。输出突出产品能力、使用场景及行动号召的宣传短片。最适合新品发布、网站展示和社交推广；不应用于在缺乏授权素材时模仿真实品牌标记，也不能编造产品宣传主张。

[英文源文件](brand-promo-video-generator/SKILL.md) · [原有中文版本](brand-promo-video-generator/SKILL.cn.md)

## 09｜music-video-subtitle-generator：音乐视频字幕生成器

![音乐视频字幕示例](../assets/music-video-subtitle-generator.gif)

**词汇释义**：musician /mjuːˈzɪʃən/ n. 音乐人；lyric typography /ˈlɪrɪk taɪˈpɒɡrəfi/ n. phr. 歌词字体编排；vocal timing /ˈvəʊkəl ˈtaɪmɪŋ/ n. phr. 人声时序；beat-reactive /biːt riˈæktɪv/ adj. 随节拍响应的；spatial /ˈspeɪʃəl/ adj. 空间化的；decompose /ˌdiːkəmˈpəʊz/ v. 拆解；audit /ˈɔːdɪt/ v. 审计；route /ruːt/ v. 分配到相应工具；MV abbr. Music Video，音乐视频；stitching /ˈstɪtʃɪŋ/ n. 拼接；subtitle-driven /ˈsʌbtaɪtəl ˈdrɪvən/ adj. 由字幕驱动的。

**译文**：面向制作带歌词字体编排的人工智能音乐视频或情感短片的音乐人、视频创作者和社交媒体编辑。该 Skill 分析节拍与人声时序，分离人物、场景和文字参考，设计随节拍响应的空间字体编排，将长作品拆解为相连镜头，审计提示词，并把生成任务分配给 H3 或其他视频工具。输出音乐视频概念、镜头提示词、歌词文字方案及拼接指导。最适合风格化音乐视频和字幕驱动的音乐画面。

[英文源文件](music-video-subtitle-generator/SKILL.md) · [原有中文版本](music-video-subtitle-generator/SKILL.cn.md)

## 10｜co-op-game-intro-generator：双人合作游戏开场生成器

![双人合作游戏开场示例](../assets/co-op-game-intro-generator.gif)

**词汇释义**：co-op /ˈkəʊɒp/ adj. 合作式的；menu /ˈmenjuː/ n. 菜单；opening animation /ˈəʊpənɪŋ ˌænɪˈmeɪʃən/ n. phr. 开场动画；identity cue /aɪˈdentəti kjuː/ n. phr. 身份识别线索；approval image /əˈpruːvəl ˈɪmɪdʒ/ n. phr. 用于确认的图像；coordinated /kəʊˈɔːdɪneɪtɪd/ adj. 协调一致的；icon /ˈaɪkɒn/ n. 图标；UI abbr. User Interface，用户界面；copy /ˈkɒpi/ n. 文案；event timing /ɪˈvent ˈtaɪmɪŋ/ n. phr. 事件时序；interaction /ˌɪntərˈækʃən/ n. 交互。

**译文**：创建双人合作游戏菜单或开场动画。该 Skill 锁定身份线索，基于固定菜单框架生成供确认的图像，使色彩、按钮、图标和字体协调一致；然后使用已确认结果重新构建人物、界面文案与事件时序指令，供最终视频使用。输出包含两个人物、玩家卡片和菜单交互动效的合作游戏开场。最适合游戏概念、人物主导的菜单和社交内容。

[英文源文件](co-op-game-intro-generator/SKILL.md) · [原有中文版本](co-op-game-intro-generator/SKILL.cn.md)

## 11｜paper-collage-explainer-generator：纸张拼贴解说生成器

![纸张拼贴示例](../assets/paper-collage-explainer-generator.gif)

**词汇释义**：narration /nəˈreɪʃən/ n. 旁白、叙述；abstract /ˈæbstrækt/ adj. 抽象的；tactile /ˈtæktaɪl/ adj. 有触感的；collage /ˈkɒlɑːʒ/ n. 拼贴；visual metaphor /ˈvɪʒuəl ˈmetəfə/ n. phr. 视觉隐喻；halftone /ˈhɑːftəʊn/ n. 网点半色调；still /stɪl/ n. 静帧图；SFX abbr. Sound Effects，音效；viewpoint /ˈvjuːpɔɪnt/ n. 观点；B-roll /ˈbiːrəʊl/ n. 辅助画面素材。

**译文**：为旁白、知识点、观点或抽象主题赋予有触感的纸张拼贴表达。该 Skill 提取含义，提出视觉隐喻，准备制作计划和分镜，生成经确认的半色调拼贴静帧，再创建带纸张运动及触感音效的定格片段，可选进行最终组接。默认保留拼贴音效；除非用户提出要求，否则不添加背景音乐、画外音或字幕。最适合解说、观点、故事画面和社交媒体辅助素材。

[英文源文件](paper-collage-explainer-generator/SKILL.md) · [原有中文版本](paper-collage-explainer-generator/SKILL.cn.md)

## 12｜handdrawn-live-video-generator：手绘与实拍混合视频生成器

![手绘实拍混合示例](../assets/handdrawn-live-video-generator.gif)

**词汇释义**：surreal /səˈrɪəl/ adj. 超现实的；blend /blend/ v. 融合；rough /rʌf/ adj. 粗糙的；glowing /ˈɡləʊɪŋ/ adj. 发光的；live-action /ˌlaɪvˈækʃən/ adj. 真人实拍的；physical contact /ˈfɪzɪkəl ˈkɒntækt/ n. phr. 物理接触；morphing /ˈmɔːfɪŋ/ n. 连续形变；escape route /ɪˈskeɪp ruːt/ n. phr. 逃离路线；delayed /dɪˈleɪd/ adj. 延迟的；handheld chase /ˈhændheld tʃeɪs/ n. phr. 手持追拍；stroke texture /strəʊk ˈtekstʃə/ n. phr. 笔触质感；jump scare /dʒʌmp skeə/ n. phr. 突发惊吓；plush /plʌʃ/ adj. 毛绒的；CG abbr. Computer Graphics，计算机图形。

**译文**：创建把粗糙发光手绘动画与实拍空间融合的超现实短视频。该 Skill 澄清物理接触方式，设计连续形变、逃离路线和带延迟的手持追拍，再用用户语言编写可复用的 15 秒、16:9 视频提示词。确认后，它推荐使用 MiniMax H3 生成，并检查接触真实感、摄影机延迟、粗糙发光笔触质感，以及非恐怖基调。最适合单场景创意片段，不适用于精致计算机图形、恐怖突发惊吓、毛绒人物或多场景切镜。

[英文源文件](handdrawn-live-video-generator/SKILL.md) · [原有中文版本](handdrawn-live-video-generator/SKILL.cn.md)

## 13｜Contribute：参与贡献

**词汇释义**：contribute /kənˈtrɪbjuːt/ v. 贡献；improve /ɪmˈpruːv/ v. 改善；community /kəˈmjuːnəti/ n. 社区；optimize /ˈɒptɪmaɪz/ v. 优化；PR abbr. Pull Request，拉取请求；credit reward /ˈkredɪt rɪˈwɔːd/ n. phr. 额度奖励。

**译文**：这些 Skill 仍在改进，欢迎社区贡献。优化已有 Skill 或新增 Skill 时，请提交拉取请求；贡献或优化 Skill 可获得 API 额度奖励。

**译注**：奖励表述来自固定源版本，只作翻译，不构成对当前活动资格或额度的核验。
