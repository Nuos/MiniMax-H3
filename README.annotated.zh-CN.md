# MiniMax H3｜英文 README 逐段词汇注释与简体中文译本

源文件：[README.md](./README.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源文件 Git blob：`bdfd2473d24434599913d8d9edb9b96a6dc13603`。

本文件新增于英文源文件所在目录，不覆盖已有 `README.zh-CN.md`。译文对应上述固定版本，不将源文中的发布计划解释为当前完成状态。各段按原文章节顺序提供词汇释义与完整译文；英文全文留在相邻源文件。字段、模型名、代码标识、标签、时间和对白保持原样。n. 名词；v. 动词；adj. 形容词；adv. 副词；n. phr. 名词短语；v. phr. 动词短语；abbr. 缩写。技术缩写给出全称，不为产品名杜撰音标。

![MiniMax H3](assets/minimax-h3-header.gif)

## 01｜页首导航

**词汇释义**：website /ˈwebsaɪt/ n. 网站；license /ˈlaɪsəns/ n. 许可证；API abbr. Application Programming Interface，应用程序编程接口；English /ˈɪŋɡlɪʃ/ n. 英语；GitHub、Hugging Face、ModelScope、Discord 为平台名称，保留原名。

**译文**：页首提供 Hailuo AI、API、MiniMax 网站、GitHub、Hugging Face、ModelScope、微信、Discord 与许可证入口；语言导航包括英文、简体中文、韩文和日文。原链接保持在 [英文源文件](./README.md) 的页首导航中。

## 02｜Prompt Writing Skill：提示词编写 Skill

### P01｜安装

**词汇释义**：prompt /prɒmpt/ n. 提示词；writing /ˈraɪtɪŋ/ n. 编写；skill /skɪl/ n. 技能模块；install /ɪnˈstɔːl/ v. 安装；bundled /ˈbʌndəld/ adj. 随包附带的；repository /rɪˈpɒzɪtəri/ n. 仓库。

**译文**：安装 H3 提示词编写 Skill；它是本仓库附带的九个 Skill 之一：

```bash
npx skills add https://github.com/MiniMax-AI/MiniMax-H3 --skill h3-prompt-writing
```

### P02｜两份参考指南

**词汇释义**：ship /ʃɪp/ v. 随产品提供；guide /ɡaɪd/ n. 指南；keyframe /ˈkiːfreɪm/ n. 关键帧；full-reference /fʊl ˈrefərəns/ adj. 全参考的；mode /məʊd/ n. 模式。

**译文**：该 Skill 在 `skills/h3-prompt-writing/references/` 下附带两份提示词指南：`base-en.txt` 对应文本／关键帧模式，`ref-en.txt` 对应全参考 Ref2VA 模式。

### P03｜智能体兼容性

**词汇释义**：compatibility /kəmˌpætəˈbɪləti/ n. 兼容性；plain /pleɪn/ adj. 纯文本形式的；external /ɪkˈstɜːnəl/ adj. 外部的；agent /ˈeɪdʒənt/ n. 智能体；SDK abbr. Software Development Kit，软件开发工具包；harness /ˈhɑːnɪs/ n. 承载智能体运行的框架；optional /ˈɒpʃənəl/ adj. 可选的；metadata /ˈmetədeɪtə/ n. 元数据；default /dɪˈfɔːlt/ adj. 默认的；specification /ˌspesɪfɪˈkeɪʃən/ n. 规范；limit /ˈlɪmɪt/ v. 限制。

**译文**：智能体兼容性：`h3-prompt-writing` 由普通 Markdown 与参考文件构成，没有外部 API 调用，因此可以用于 Claude Code、Claude Agent SDK、Cursor、Windsurf、基于 OpenAI 的智能体／Codex、LangChain，或任何能读取 `SKILL.md` 和本地文件的运行框架。附带的 `skills/h3-prompt-writing/agents/openai.yaml` 按照原文所链接的 OpenAI Skill 规范，仅为 ChatGPT/Codex 技能界面添加可选界面元数据，包括显示名称、描述和默认提示词；它不把该 Skill 限制为只能供 OpenAI 智能体使用。

### P04｜另外八个 Skill

**词汇释义**：remaining /rɪˈmeɪnɪŋ/ adj. 剩余的；style-specific /staɪl spəˈsɪfɪk/ adj. 针对特定风格的；canvas /ˈkænvəs/ n. 画布；workflow /ˈwɜːkfləʊ/ n. 工作流程；node /nəʊd/ n. 节点；choice card /tʃɔɪs kɑːd/ n. phr. 选择卡片；portable /ˈpɔːtəbəl/ adj. 可移植的；generic /dʒəˈnerɪk/ adj. 通用的。

**译文**：其余八个是为 MiniMax Hub 画布工作流制作的特定风格视频生成 Skill，依赖 `hub_generate_video`、`hub_generate_image`、画布节点、选择卡片等，并不能直接移植到通用智能体框架。

| 原始名称与路径 | 词汇释义 | 中文含义 |
|---|---|---|
| [minimalist-product-ad-generator](skills/minimalist-product-ad-generator/SKILL.md) | minimalist /ˈmɪnɪməlɪst/ adj. 极简主义的；product /ˈprɒdʌkt/ n. 产品；ad /æd/ n. 广告；generator /ˈdʒenəreɪtə/ n. 生成器 | 极简产品广告生成器 |
| [3d-animation-short-generator](skills/3d-animation-short-generator/SKILL.md) | animation /ˌænɪˈmeɪʃən/ n. 动画；short /ʃɔːt/ n. 短片 | 三维动画短片生成器 |
| [papercraft-stop-motion-explainer](skills/papercraft-stop-motion-explainer/SKILL.md) | papercraft /ˈpeɪpəkrɑːft/ n. 纸艺；stop-motion /ˌstɒpˈməʊʃən/ n. 定格动画；explainer /ɪkˈspleɪnə/ n. 解说内容 | 纸艺定格解说生成器 |
| [brand-promo-video-generator](skills/brand-promo-video-generator/SKILL.md) | brand /brænd/ n. 品牌；promo /ˈprəʊməʊ/ n. 宣传片 | 品牌宣传视频生成器 |
| [music-video-subtitle-generator](skills/music-video-subtitle-generator/SKILL.md) | subtitle /ˈsʌbtaɪtəl/ n. 字幕 | 音乐视频字幕生成器 |
| [co-op-game-intro-generator](skills/co-op-game-intro-generator/SKILL.md) | co-op /ˈkəʊɒp/ adj. 合作式的；intro /ˈɪntrəʊ/ n. 开场 | 合作游戏开场生成器 |
| [paper-collage-explainer-generator](skills/paper-collage-explainer-generator/SKILL.md) | collage /ˈkɒlɑːʒ/ n. 拼贴 | 纸张拼贴解说生成器 |
| [handdrawn-live-video-generator](skills/handdrawn-live-video-generator/SKILL.md) | hand-drawn /ˌhændˈdrɔːn/ adj. 手绘的；live /laɪv/ adj. 实拍／现场的 | 手绘与实拍结合的视频生成器 |

## 03｜Online API 与 Online App：在线接口与应用

### P05｜在线 API

**词汇释义**：online /ˌɒnˈlaɪn/ adj. 在线的；directly /dəˈrektli/ adv. 直接地；global /ˈɡləʊbəl/ adj. 全球的；CN abbr. China，中国区。

**译文**：通过 API 直接使用 MiniMax-H3。全球区入口为 [platform.minimax.io](https://platform.minimax.io/docs/api-reference/video-generation-v2-create)，中国区入口为 [platform.minimaxi.com](https://platform.minimaxi.com/docs/api-reference/video-generation-v2-create)。

### P06｜在线应用

**词汇释义**：app /æp/ n. 应用程序；web app /web æp/ n. phr. 网页应用；desktop /ˈdesktɒp/ adj. 桌面端的。

**译文**：通过应用直接使用 MiniMax-H3。网页应用：全球区 [hailuoai.video](https://hailuoai.video/tools/minimax-h3)，中国区 [hailuoai.com](https://hailuoai.com/)。桌面应用：全球区 [hub.minimax.io](https://hub.minimax.io/)，中国区 [hub.minimaxi.com](https://hub.minimaxi.com/)。

## 04｜System Overview：系统概述

### P07｜总体能力

**词汇释义**：general-purpose /ˌdʒenərəl ˈpɜːpəs/ adj. 通用的；omni-modal /ˌɒmniˈməʊdəl/ adj. 全模态的；generative /ˈdʒenərətɪv/ adj. 生成式的；unified /ˈjuːnɪfaɪd/ adj. 统一的；context /ˈkɒntekst/ n. 上下文；native /ˈneɪtɪv/ adj. 原生的；stereo /ˈsteriəʊ/ adj. 立体声的；resolution /ˌrezəˈluːʃən/ n. 分辨率；duration /djʊəˈreɪʃən/ n. 时长；generalization /ˌdʒenərəlaɪˈzeɪʃən/ n. 泛化；pre-training /ˌpriːˈtreɪnɪŋ/ n. 预训练；instruction /ɪnˈstrʌkʃən/ n. 指令。

**译文**：MiniMax H3 是通用的全模态生成系统。它支持统一理解由文本、图像、视频和音频组成的多模态上下文，并能生成带原生立体声音频的视频，最高分辨率为 2K，最长时长为 15 秒。得益于面向任务泛化的系统设计，H3 在预训练阶段就已具备广泛的多模态上下文理解与生成能力，因此能够出色地遵循复杂多模态指令。

### P08｜输入输出规格

**词汇释义**：specification /ˌspesɪfɪˈkeɪʃən/ n. 规格；aspect ratio /ˈæspekt ˈreɪʃiəʊ/ n. phr. 画幅宽高比；shorter side /ˈʃɔːtə saɪd/ n. phr. 短边；pixel /ˈpɪksəl/ n. 像素；default /dɪˈfɔːlt/ n. 默认值；frame rate /freɪm reɪt/ n. phr. 帧率；FPS abbr. frames per second，每秒帧数；kHz abbr. kilohertz，千赫；varying degrees /ˈveəriɪŋ dɪˈɡriːz/ n. phr. 不同程度。

**译文**：H3 支持以下输入输出规格：

| 类别 | 规格 |
|---|---|
| 输出时长 | 4—15 秒 |
| 输出画幅 | 支持多种宽高比，包括但不限于 21:9、16:9、4:3、1:1、3:4、9:16 |
| 输出分辨率 | 支持多种尺寸，短边默认 768 像素；2K 生成通过 H3-Regenerate-2K 实现。原表单元格中多余的竖线是排版字符，不是另一个参数 |
| 输出帧率 | 24 FPS |
| 输出音频 | 32 kHz 立体声 |
| 对白语言 | 稳定支持阿拉伯语、中文、英语、法语、德语、意大利语、日语、韩语、葡萄牙语、俄语、西班牙语，共 11 种；也在不同程度上支持其他语言 |

### P09｜模型变体与输入规格

**词汇释义**：variant /ˈveəriənt/ n. 变体；first-and-last-frame /fɜːst ənd lɑːst freɪm/ adj. 首尾帧的；omni-reference /ˌɒmniˈrefərəns/ adj. 全参考的；clip /klɪp/ n. 片段；total duration /ˈtəʊtəl djʊəˈreɪʃən/ n. phr. 总时长；mixed /mɪkst/ adj. 混合的；maximum /ˈmæksɪməm/ n. 最大值。

**译文**：H3-Base-FL2VA 为首尾帧模式，支持零张、一张或两张输入图像。没有图像时为文生视频；一张图像时可以首帧生视频或尾帧生视频；两张图像时为首尾帧生视频。H3-Base-Ref2VA 为全参考模式，支持多模态参考输入：图像不超过 9 张；视频不超过 3 段，每段 2—15 秒，总时长不超过 15 秒；音频不超过 3 段，每段 2—15 秒，总时长不超过 15 秒；混合输入的文件总数最多 12 个。

![系统概览](assets/overview.png)

### P10｜完整系统的三个模块

**词汇释义**：consist /kənˈsɪst/ v. 由……组成；module /ˈmɒdjuːl/ n. 模块；complete /kəmˈpliːt/ adj. 完整的。

**译文**：完整 H3 系统由以下三个模块组成。

### P11｜H3-Context-IR

**词汇释义**：dedicated /ˈdedɪkeɪtɪd/ adj. 专用于某项任务的；deeply /ˈdiːpli/ adv. 深入地；refine /rɪˈfaɪn/ v. 细化、完善；convert /kənˈvɜːt/ v. 转换；readily /ˈredɪli/ adv. 容易地；intermediate representation /ˌɪntəˈmiːdiət ˌreprɪzenˈteɪʃən/ n. phr. 中间表示；critical /ˈkrɪtɪkəl/ adj. 至关重要的；incorporate /ɪnˈkɔːpəreɪt/ v. 纳入；pipeline /ˈpaɪplaɪn/ n. 处理流水线；context-processing /ˈkɒntekst ˈprəʊsesɪŋ/ n. 上下文处理。

**译文**：H3-Context-IR：随着输入日益复杂，我们构建了一个专用系统，深入理解并细化输入的多模态指令，然后将其转换成 H3 容易理解的形式——上下文中间表示（Context Intermediate Representation）——用于生成。H3-Context-IR 对最终输出质量至关重要，因此我们强烈建议将其纳入生成流水线，或遵循“提示词指导”构建自己的上下文处理系统。

### P12｜H3-Base

**词汇释义**：generate /ˈdʒenəreɪt/ v. 生成；based on /beɪst ɒn/ phr. 基于；output /ˈaʊtpʊt/ n. 输出；resolution /ˌrezəˈluːʃən/ n. 分辨率。

**译文**：H3-Base：根据 H3-Context-IR 的输出生成音频和视频，产出 768p 分辨率的结果。

### P13｜H3-Regenerate-2K

**词汇释义**：feed back /fiːd bæk/ v. phr. 回送；regenerate /ˌriːˈdʒenəreɪt/ v. 重新生成；leverage /ˈliːvərɪdʒ/ v. 利用；capability /ˌkeɪpəˈbɪləti/ n. 能力；accurate /ˈækjərət/ adj. 准确的；detail /ˈdiːteɪl/ n. 细节；visual fidelity /ˈvɪʒuəl fɪˈdeləti/ n. phr. 视觉保真度。

**译文**：H3-Regenerate-2K：把 768p 结果与原始上下文一起重新输入 H3，以 2K 分辨率再生成输出。该过程同时利用 H3 强大的生成能力和原始上下文中的丰富信息，从而产生细节更准确、视觉保真度更高的高分辨率输出。

## 05｜Model Architecture：模型架构

### P14｜H3-Context-IR 的系统性质

**词汇释义**：hosted /ˈhəʊstɪd/ adj. 托管的；preprocessing /ˌpriːˈprəʊsesɪŋ/ n. 预处理；orchestration /ˌɔːkɪˈstreɪʃən/ n. 流程编排；free-form /ˌfriːˈfɔːm/ adj. 自由形式的；multimodal /ˌmʌltiˈməʊdəl/ adj. 多模态的。

**译文**：H3-Context-IR 是为自由形式多模态输入设计的托管预处理与流程编排系统。

### P15｜关系理解与内部流程

**词汇释义**：interpret /ɪnˈtɜːprɪt/ v. 理解、解释；relationship /rɪˈleɪʃənʃɪp/ n. 关系；intended /ɪnˈtendɪd/ adj. 预期的；internal /ɪnˈtɜːnəl/ adj. 内部的；parsing /ˈpɑːsɪŋ/ n. 解析；cross-modal association /krɒs ˈməʊdəl əˌsəʊsiˈeɪʃən/ n. phr. 跨模态关联；temporal understanding /ˈtempərəl ˌʌndəˈstændɪŋ/ n. phr. 时序理解；logical reasoning /ˈlɒdʒɪkəl ˈriːzənɪŋ/ n. phr. 逻辑推理。

**译文**：它理解文本、图像、音频和参考视频之间的关系，以及这些素材与预期生成结果的关系。其内部工作流程包括指令解析、跨模态关联、时间理解和复杂逻辑推理。

### P16｜结构化表示与语义补全

**词汇释义**：serialize /ˈsɪəriəlaɪz/ v. 序列化；structured representation /ˈstrʌktʃəd ˌreprɪzenˈteɪʃən/ n. phr. 结构化表示；accept /əkˈsept/ v. 接受；deviate /ˈdiːvieɪt/ v. 偏离；intent /ɪnˈtent/ n. 意图；supplement /ˈsʌplɪment/ v. 补充；underspecified /ˌʌndəˈspesɪfaɪd/ adj. 描述或规定不充分的；semantic /sɪˈmæntɪk/ adj. 语义的；appropriate /əˈprəʊpriət/ adj. 适当的。

**译文**：H3-Context-IR 将自己对上下文的理解序列化为 H3-Base 接受的结构化表示。在不偏离用户原始意图的前提下，它也可能适度补充缺失或描述不充分的语义细节。

### P17｜开放范围与接口

**词汇释义**：rely /rɪˈlaɪ/ v. 依赖；multi-stage /ˌmʌltiˈsteɪdʒ/ adj. 多阶段的；service /ˈsɜːvɪs/ n. 服务；release /rɪˈliːs/ n. 发布版本；reproduce /ˌriːprəˈdjuːs/ v. 复现；behavior /bɪˈheɪvjə/ n. 行为；official /əˈfɪʃəl/ adj. 官方的；tutorial /tjuːˈtɔːriəl/ n. 教程；developer /dɪˈveləpə/ n. 开发者。

**译文**：H3-Context-IR 依赖多阶段流程以及多个托管模型和服务，因此未包含在此次开源发布中。我们提供 API，让用户复现官方流程的行为；也提供详细教程，开发者可遵循“提示词指导”构建自己的预处理系统。

### P18｜详细用法位置

**词汇释义**：usage /ˈjuːsɪdʒ/ n. 使用方法；recommended /ˌrekəˈmendɪd/ adj. 推荐的；workflow /ˈwɜːkfləʊ/ n. 工作流程。

**译文**：详细使用说明见“推荐工作流程——完整 2K 工作流”。

### P19｜Safety Guardrails：安全防护

**词汇释义**：guardrail /ˈɡɑːdreɪl/ n. 防护措施；submitted /səbˈmɪtɪd/ adj. 已提交的；enhanced /ɪnˈhɑːnst/ adj. 增强的；automated moderation /ˈɔːtəmeɪtɪd ˌmɒdəˈreɪʃən/ n. phr. 自动内容审核；unlawful /ʌnˈlɔːfəl/ adj. 违法的；pornographic /ˌpɔːnəˈɡræfɪk/ adj. 色情的；infringe /ɪnˈfrɪndʒ/ v. 侵犯；false positive /fɔːls ˈpɒzətɪv/ n. phr. 误报；false negative /fɔːls ˈneɡətɪv/ n. phr. 漏报；licensee /ˌlaɪsənˈsiː/ n. 被许可方；obligation /ˌɒblɪˈɡeɪʃən/ n. 义务；restriction /rɪˈstrɪkʃən/ n. 限制。

**译文**：用户提交的文本、图像和视频，以及增强后的提示词，都接受自动审核。涉嫌违法、色情或侵犯第三方权利的内容可能被拦截。我们采用行业标准过滤措施，但无法完全消除误报或漏报。这些防护措施不影响被许可方在《MiniMax H3 社区许可协议》下的义务，尤其是合法使用和使用限制方面的义务。

### H3-Base

![完整架构](assets/full-arch.png)

### P20｜编码与打包序列

**词汇释义**：encode /ɪnˈkəʊd/ v. 编码；modality /məʊˈdæləti/ n. 模态；encoder /ɪnˈkəʊdə/ n. 编码器；VAE abbr. Variational Autoencoder，变分自编码器；packed /pækt/ adj. 打包的；sequence /ˈsiːkwəns/ n. 序列；RoPE abbr. Rotary Position Embedding，旋转位置编码；spatial /ˈspeɪʃəl/ adj. 空间的；temporal /ˈtempərəl/ adj. 时间的；token /ˈtəʊkən/ n. 词元、模型处理单元。

**译文**：H3-Base 使用各模态对应的编码器或 VAE 编码不同模态，并将编码结果组织成统一的、打包后的多模态序列。整个序列送入 H3-Omni-Transformer 前，先通过 RoPE 表达词元之间必要的空间与时间关系。

### P21｜各模态的编码器

**词汇释义**：specifically /spəˈsɪfɪkli/ adv. 具体而言；visual input /ˈvɪʒuəl ˈɪnpʊt/ n. phr. 视觉输入；solely /ˈsəʊlli/ adv. 仅仅。

**译文**：具体来说，文本由 H3-Encoder 编码；视觉输入同时由 H3-Encoder 和 H3-VisualVAE 编码；音频仅由 H3-AudioVAE 编码。

### P22｜音视频联合预测

**词汇释义**：jointly /ˈdʒɔɪntli/ adv. 联合地；predict /prɪˈdɪkt/ v. 预测；latent /ˈleɪtənt/ n. 潜在表示；decode /diːˈkəʊd/ v. 解码；respectively /rɪˈspektɪvli/ adv. 分别。

**译文**：H3-Omni-Transformer 联合预测视频和音频潜在表示，再分别解码为视频与立体声音频。

### P23｜稀疏注意力的发布边界

**词汇释义**：computational cost /ˌkɒmpjuˈteɪʃənəl kɒst/ n. phr. 计算成本；natively /ˈneɪtɪvli/ adv. 原生地；sparse attention /spɑːs əˈtenʃən/ n. phr. 稀疏注意力；training /ˈtreɪnɪŋ/ n. 训练；inference /ˈɪnfərəns/ n. 推理；initial /ɪˈnɪʃəl/ adj. 初始的；implementation /ˌɪmplɪmenˈteɪʃən/ n. 实现。

**译文**：为了降低长多模态序列的计算成本，H3 原生支持稀疏注意力训练和推理。首次开源发布仅提供全注意力推理，稀疏注意力实现将在后续更新中发布。

### P24｜H3-Encoder 的权重与隐藏状态

**词汇释义**：pretrained /ˌpriːˈtreɪnd/ adj. 预训练的；weight /weɪt/ n. 权重；hidden state /ˈhɪdən steɪt/ n. phr. 隐藏状态；layer /ˈleɪə/ n. 层。

**译文**：H3-Encoder 使用 Qwen3-VL-32B 的完整预训练权重，并向 H3-Omni-Transformer 提供其第 50 层隐藏状态。

### P25｜特殊词元与分词器

**词汇释义**：special token /ˈspeʃəl ˈtəʊkən/ n. phr. 特殊词元；tokenizer /ˈtəʊkənaɪzə/ n. 分词器；configuration /kənˌfɪɡəˈreɪʃən/ n. 配置；associated /əˈsəʊsieɪtɪd/ adj. 关联的；required /rɪˈkwaɪəd/ adj. 必需的。

**译文**：我们在分词器配置中添加了若干特殊词元，如 `<d>`。使用 H3 时，必须采用 H3 仓库提供的分词器及相关配置文件。

### P26｜H3-VAE

**词汇释义**：separate /ˈsepərət/ adj. 分开的；latent /ˈleɪtənt/ n. 潜在表示；respective /rɪˈspektɪv/ adj. 各自的；represent /ˌreprɪˈzent/ v. 表示。

**译文**：H3 使用独立的视觉和音频潜在表示，分别表示各自模态。

### P27｜视觉 VAE 的压缩规格

**词汇释义**：temporally causal /ˈtempərəli ˈkɔːzəl/ adj. 时间因果的；autoencoder /ˌɔːtəʊɪnˈkəʊdə/ n. 自编码器；compression factor /kəmˈpreʃən ˈfæktə/ n. phr. 压缩因子；channel /ˈtʃænəl/ n. 通道；denote /dɪˈnəʊt/ v. 记作；optimization /ˌɒptɪmaɪˈzeɪʃən/ n. 优化；reconstruction /ˌriːkənˈstrʌkʃən/ n. 重建；learnability /ˌlɜːnəˈbɪləti/ n. 可学习性。

**译文**：H3-VisualVAE 是时间因果视频自编码器，空间压缩因子为 16 倍、时间压缩因子为 4 倍、潜在通道数为 24，记作 f16t4d24。我们采用若干潜在空间优化技术，同时提高重建质量和潜在表示的可学习性。

### P28｜分块与有效下采样

**词汇释义**：patchify /ˈpætʃɪfaɪ/ v. 划分为块；patch size /pætʃ saɪz/ n. phr. 块尺寸；dimension /daɪˈmenʃən/ n. 维度；effective /ɪˈfektɪv/ adj. 有效的；downsampling /ˌdaʊnˈsɑːmplɪŋ/ n. 下采样；remain /rɪˈmeɪn/ v. 保持。

**译文**：进入 H3-Omni-Transformer 前，视觉潜在表示沿 `(time, height, width)` 维度，以 `1 × 2 × 2` 的块尺寸进一步分块。因此进入 Transformer 的视觉词元具有 32 倍有效空间下采样率，时间下采样率仍为 4 倍。

### P29｜潜在空间与解码器优化

**词汇释义**：latent space /ˈleɪtənt speɪs/ n. phr. 潜在空间；ease /iːz/ n. 容易程度；additionally /əˈdɪʃənəli/ adv. 另外；ViT abbr. Vision Transformer，视觉 Transformer；decoder /diːˈkəʊdə/ n. 解码器；reduce /rɪˈdjuːs/ v. 降低。

**译文**：H3-VisualVAE 的潜在空间同时针对重建质量以及生成模型的学习便利性进行优化。编码器训练之后，我们另外训练基于 ViT 的解码器，以降低解码成本并进一步提高重建质量。

### P30｜音频 VAE 的左右声道

**词汇释义**：channel /ˈtʃænəl/ n. 声道；independently /ˌɪndɪˈpendəntli/ adv. 独立地；recombine /ˌriːkəmˈbaɪn/ v. 重新组合；stereo /ˈsteriəʊ/ adj. 立体声的。

**译文**：H3-AudioVAE 对左右声道使用相同的编码器和解码器，但分别独立处理两个声道。解码之后再组合声道，从而支持立体声音频输入与输出。

### P31｜音频时间压缩

**词汇释义**：compress /kəmˈpres/ v. 压缩；sequence /ˈsiːkwəns/ n. 序列；temporal rate /ˈtempərəl reɪt/ n. phr. 时间采样速率；Hz abbr. hertz，赫兹。

**译文**：对于每个声道，H3-AudioVAE 将 32 kHz 音频压缩为时间速率为 40 Hz 的潜在词元序列。

### P32｜音频潜在空间优化

**词汇释义**：inspired /ɪnˈspaɪəd/ adj. 受启发的；optimize /ˈɒptɪmaɪz/ v. 优化；preserve /prɪˈzɜːv/ v. 保持；reconstruction quality /ˌriːkənˈstrʌkʃən ˈkwɒləti/ n. phr. 重建质量。

**译文**：受 VA-VAE 启发，我们优化潜在空间，在保持音频重建质量的同时，让生成模型更容易学习。

### P33｜Omni Transformer 的参数结构

**词汇释义**：scalability /ˌskeɪləˈbɪləti/ n. 可扩展性；generalization /ˌdʒenərəlaɪˈzeɪʃən/ n. 泛化；dense /dens/ adj. 稠密的；single-stream /ˈsɪŋɡəl striːm/ adj. 单流的；parameter /pəˈræmɪtə/ n. 参数；AdaLN abbr. Adaptive Layer Normalization，自适应层归一化；branch /brɑːntʃ/ n. 分支；modulation /ˌmɒdjʊˈleɪʃən/ n. 调制；precompute /ˌpriːkəmˈpjuːt/ v. 预计算；cache /kæʃ/ v. 缓存；deployment /dɪˈplɔɪmənt/ n. 部署；fine-tuning /ˈfaɪn ˌtjuːnɪŋ/ n. 微调。

**译文**：出于可扩展性与泛化的考虑，我们采用相对简单的 Transformer 块设计。H3-Omni-Transformer 是一个 330 亿参数、稠密、单流 Transformer，其中约 130 亿参数位于 AdaLN 相关分支。AdaLN 调制输出可以预计算并缓存，因此仅作推理的部署不必加载这些参数。我们发布完整模型权重，以支持进一步开发，包括微调。

### P34｜模态专用参数的位置

**词汇释义**：attention layer /əˈtenʃən ˈleɪə/ n. phr. 注意力层；FFN abbr. Feed-Forward Network，前馈网络；modality-specific /məʊˈdæləti spəˈsɪfɪk/ adj. 模态专用的；confine /kənˈfaɪn/ v. 限定；input/output /ˈɪnpʊt ˈaʊtpʊt/ n. 输入／输出；relatively /ˈrelətɪvli/ adv. 相对地；additional /əˈdɪʃənəl/ adj. 额外的。

**译文**：注意力层和 FFN 层都不包含模态专用结构。模态专用参数仅分布在输入／输出层及 AdaLN 分支。特别是，模态专用 AdaLN 能以相对较低的额外训练和推理成本改善生成质量。

### P35｜三维位置编码

**词汇释义**：MM-RoPE abbr. Multimodal Rotary Position Embeddings，多模态旋转位置嵌入；three-dimensional /ˌθriː daɪˈmenʃənəl/ adj. 三维的；positional /pəˈzɪʃənəl/ adj. 位置的；temporal /ˈtempərəl/ adj. 时间的；spatial /ˈspeɪʃəl/ adj. 空间的。

**译文**：模型采用三维多模态旋转位置嵌入（MM-RoPE），表示一个时间维度和两个空间维度 `(t, h, w)` 上的位置关系。

### P36｜训练末期加入稀疏注意力

**词汇释义**：final stage /ˈfaɪnəl steɪdʒ/ n. phr. 最后阶段；introduce /ˌɪntrəˈdjuːs/ v. 引入；native /ˈneɪtɪv/ adj. 原生的；separately /ˈsepərətli/ adv. 单独地；future update /ˈfjuːtʃə ˈʌpdeɪt/ n. phr. 后续更新。

**译文**：训练最后阶段引入原生稀疏注意力，以降低长序列的计算成本。首次开源发布不包含稀疏注意力实现，后续更新将单独发布。

### P37｜2K 再生成方法

**词汇释义**：conventional /kənˈvenʃənəl/ adj. 传统的；dedicated /ˈdedɪkeɪtɪd/ adj. 专用的；super-resolution /ˌsuːpə ˌrezəˈluːʃən/ n. 超分辨率；in-context /ɪn ˈkɒntekst/ adj. 上下文内的；regenerate /ˌriːˈdʒenəreɪt/ v. 重新生成。

**译文**：H3 的 2K 输出没有采用传统专用超分辨率模块，而是让 H3 基础模型以上下文内处理方式重新生成自己的低分辨率结果。

### P38｜该方法的两个优点

**词汇释义**：advantage /ədˈvɑːntɪdʒ/ n. 优点；reuse /ˌriːˈjuːz/ v. 复用；extent /ɪkˈstent/ n. 程度；recover /rɪˈkʌvə/ v. 恢复；otherwise /ˈʌðəwaɪz/ adv. 否则；guess /ɡes/ v. 猜测；fine detail /faɪn ˈdiːteɪl/ n. phr. 精细细节。

**译文**：这种方法有两个优点：第一，再生成过程可以最大程度复用 H3 基础模型的生成能力；第二，上下文内格式让高分辨率生成复用原始多模态上下文，因此能恢复传统超分辨率方法原本不得不“猜测”的信息，例如小字和精细细节。

### P39｜任务泛化实例

**词汇释义**：in-context regeneration /ɪn ˈkɒntekst ˌriːdʒenəˈreɪʃən/ n. phr. 上下文内再生成；task generalization /tɑːsk ˌdʒenərəlaɪˈzeɪʃən/ n. phr. 任务泛化。

**译文**：上下文内再生成也是任务泛化的一个实例。

### P40｜2K 模块开放范围

**词汇释义**：complexity /kəmˈpleksəti/ n. 复杂度；open-sourced /ˌəʊpənˈsɔːst/ adj. 已开源的；ready /ˈredi/ adj. 准备就绪的；validate /ˈvælɪdeɪt/ v. 验证。

**译文**：由于系统复杂，该模块尚未开源，准备就绪后将发布。我们提供用于验证官方结果的 API，见下文“完整 2K 工作流”。

## 06｜Recommended Workflow：推荐工作流程

### P41｜两种验证方法

**词汇释义**：community /kəˈmjuːnəti/ n. 社区；deploy /dɪˈplɔɪ/ v. 部署；correctly /kəˈrektli/ adv. 正确地；validation /ˌvælɪˈdeɪʃən/ n. 验证；method /ˈmeθəd/ n. 方法。

**译文**：为了帮助社区正确部署 MiniMax H3，我们提供两种验证方法。

### P42｜完整 2K 与本地 768p

**词汇释义**：end-to-end /ˌend tə ˈend/ adj. 端到端的；combine /kəmˈbaɪn/ v. 结合；Open Platform /ˈəʊpən ˈplætfɔːm/ n. phr. 开放平台；locally deployed /ˈləʊkəli dɪˈplɔɪd/ adj. 本地部署的。

**译文**：完整 H3 系统包含 H3-Context-IR、H3-Base 与 H3-Regenerate-2K 三个模块。因此，“完整 2K 工作流”结合开放平台 API 与本地 H3-Base，提供面向 2K 输出的端到端验证流水线；“H3-Base 本地部署”部分则提供只使用本地 H3-Base 验证 768p 输出的方法。

### P43｜提示词系统教程

**词汇释义**：in addition /ɪn əˈdɪʃən/ phr. 此外；guidance /ˈɡaɪdəns/ n. 指导；detailed /ˈdiːteɪld/ adj. 详细的；develop /dɪˈveləp/ v. 开发。

**译文**：此外，“提示词指导”部分提供详细教程，帮助社区开发自己的提示词系统。

### P44｜两个检查点

**词汇释义**：task-specific /tɑːsk spəˈsɪfɪk/ adj. 针对特定任务的；checkpoint /ˈtʃekpɔɪnt/ n. 模型检查点；specialized /ˈspeʃəlaɪzd/ adj. 专门化的；processor /ˈprəʊsesə/ n. 处理器；standalone /ˈstændəˌləʊn/ adj. 独立的；component /kəmˈpəʊnənt/ n. 组件。

**译文**：MiniMax H3 以两个任务专用检查点发布。每个检查点都包括专门化的 Omni Transformer 模型，以及必需的 processor、tokenizer、文本编码器、视觉 VAE 和独立音频 VAE 组件。

### P45｜检查点规格表

**词汇释义**：condition /kənˈdɪʃən/ n. 条件；optional /ˈɒpʃənəl/ adj. 可选的；precision /prɪˈsɪʒən/ n. 数值精度；BF16 abbr. bfloat16，16 位浮点数格式。

**译文**：MiniMax-H3 Base FL2VA 支持 `t2va` 文生音视频和 `fl2va` 首／尾帧生音视频；输入是文本，可选首帧、尾帧或二者；输出视频与音频，精度 BF16。MiniMax-H3 Base Ref2VA 支持 `ref2va` 参考素材生音视频；输入是文本及参考图像、视频和／或音频；输出视频与音频，精度 BF16。

### P46｜CFG 蒸馏

**词汇释义**：CFG abbr. Classifier-Free Guidance，无分类器引导；distilled /dɪˈstɪld/ adj. 经蒸馏的；model weight /ˈmɒdəl weɪt/ n. phr. 模型权重。

**译文**：发布的检查点是经过 CFG 蒸馏的 Omni Transformer 模型权重。

### P47｜检查点目录

**词汇释义**：distribute /dɪˈstrɪbjuːt/ v. 分发；self-contained /ˌself kənˈteɪnd/ adj. 自包含的；component /kəmˈpəʊnənt/ n. 组件。

**译文**：每个检查点作为自包含的 Hugging Face 风格仓库分发，含以下组件；原目录标识保留：

```text
<TASK>/
├── model_index.json
├── processor/
├── tokenizer/
├── text_encoder/
├── transformer/
├── visual_vae/
└── audio_vae/
```

### P48｜按框架限定下载范围

**词汇释义**：download /ˌdaʊnˈləʊd/ v. 下载；host /həʊst/ v. 托管；side by side /saɪd baɪ saɪd/ adv. 并列地；scope /skəʊp/ v. 限定范围；framework /ˈfreɪmwɜːk/ n. 框架。

**译文**：下载模型。仓库并列提供原始检查点（`FL2VA/`、`Ref2VA/`）和 diffusers 格式，因此应按所用框架限定下载范围。

### P49｜模型入口与任务索引

**词汇释义**：repository-level /rɪˈpɒzɪtəri ˈlevəl/ adj. 仓库级的；public entry /ˈpʌblɪk ˈentri/ n. phr. 公共入口；task family /tɑːsk ˈfæməli/ n. phr. 任务族；index /ˈɪndeks/ n. 索引。

**译文**：`model_index.json` 是仓库级公共入口。任务族专用 diffusers 索引仍位于 `FL2VA/model_index.json` 和 `Ref2VA/model_index.json`。

```bash
# 原始检查点，同时下载两个任务族（SGLang、vLLM）：
hf download MiniMaxAI/MiniMax-H3 --include "model_index.json" "FL2VA/*" "Ref2VA/*" --local-dir MiniMax-H3

# 或者仅下载一个任务族：
hf download MiniMaxAI/MiniMax-H3 --include "model_index.json" "FL2VA/*" --local-dir MiniMax-H3
```

### P50｜diffusers 自动获取组件

**词汇释义**：manual /ˈmænjuəl/ adj. 手动的；fetch /fetʃ/ v. 获取；exactly /ɪɡˈzæktli/ adv. 精确地；loading recipe /ˈləʊdɪŋ ˈresəpi/ n. phr. 加载示例方案。

**译文**：diffusers 用户不必手动下载：`ModularPipeline.from_pretrained("MiniMaxAI/MiniMax-H3")` 会精确获取所需组件。加载方案见原文所链接的 [diffusers 文档](https://github.com/huggingface/diffusers/blob/minimax-h3/docs/source/en/api/pipelines/minimax_h3.md)。

### P51｜推荐推理框架

**词汇释义**：inference framework /ˈɪnfərəns ˈfreɪmwɜːk/ n. phr. 推理框架；serve /sɜːv/ v. 以服务方式运行；cookbook /ˈkʊkbʊk/ n. 实用示例教程；recipe /ˈresəpi/ n. 操作方案；template /ˈtempleɪt/ n. 模板。

**译文**：原文推荐以下推理框架提供模型服务：SGLang，参见其 [MiniMax-H3 cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3)；vLLM，参见 [recipes](https://recipes.vllm.ai/MiniMaxAI/MiniMax-H3)；diffusers，参见上述文档；ComfyUI，参见 [教程](https://docs.comfy.org/tutorials/video/minimax/minimax-h3)，并使用 [R2V 模板](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/video_minimax_h3_r2v.json) 或 [T2V 模板](https://github.com/Comfy-Org/workflow_templates/blob/main/templates/video_minimax_h3_t2v.json)。

### P52｜SGLang 部署示例

**词汇释义**：deployment /dɪˈplɔɪmənt/ n. 部署；configuration /kənˌfɪɡəˈreɪʃən/ n. 配置；model path /ˈmɒdəl pɑːθ/ n. phr. 模型路径；performance /pəˈfɔːməns/ n. 性能；host /həʊst/ n. 监听主机；port /pɔːt/ n. 端口。

**译文**：这里以 SGLang 为部署示例。其他部署配置见原文的 MiniMax-H3 部署指南。以下运行命令按源文件保留，不据此宣称已在本地执行。

FL2VA：
```bash
sglang serve \
  --model-path MiniMaxAI/MiniMax-H3 \
  --num-gpus 4 \
  --ulysses-degree 4 \
  --performance-mode speed \
  --host 0.0.0.0 \
  --port 30010 \
  --model-variant fl2va
```

Ref2VA：
```bash
sglang serve \
  --model-path MiniMaxAI/MiniMax-H3 \
  --num-gpus 4 \
  --ulysses-degree 4 \
  --performance-mode speed \
  --host 0.0.0.0 \
  --port 30011 \
  --model-variant ref2va
```

### P53｜可复现 768p 案例

**词汇释义**：reproducible /ˌriːprəˈdjuːsəbəl/ adj. 可复现的；use case /juːs keɪs/ n. phr. 使用案例；demonstrate /ˈdemənstreɪt/ v. 展示；request /rɪˈkwest/ n. 请求；result /rɪˈzʌlt/ n. 结果。

**译文**：以下 T2VA、FL2VA、Ref2VA 三种用例展示如何复现 MiniMax-H3 音视频生成：

| 用例 | 请求脚本 | 结果 |
|---|---|---|
| T2VA | [reproducible-768p-t2va-request.sh](scripts/readme/reproducible-768p-t2va-request.sh) | [t2va.mp4](assets/t2va.mp4) |
| FL2VA | [reproducible-768p-fl2va-request.sh](scripts/readme/reproducible-768p-fl2va-request.sh) | [fl2va.mp4](assets/fl2va.mp4) |
| Ref2VA | [reproducible-768p-ref2va-request.sh](scripts/readme/reproducible-768p-ref2va-request.sh) | [ref2va.mp4](assets/ref2va.mp4) |

### P54｜用本地图像／视频替换远程地址

**词汇释义**：remote /rɪˈməʊt/ adj. 远程的；URI abbr. Uniform Resource Identifier，统一资源标识符；URL abbr. Uniform Resource Locator，统一资源定位符；CDN abbr. Content Delivery Network，内容分发网络；out of the box /aʊt əv ðə bɒks/ phr. 开箱即用；point at /pɔɪnt æt/ v. phr. 指向；swap /swɒp/ v. 替换。

**译文**：上述复现脚本中的 `conditions[].uri` 使用公共 CDN 地址，便于开箱即用，但 `uri` 并不限于 `http(s)://`。本地测试可以改用 `file://` 路径。例如，把 FL2VA 的关键帧替换为自己的图像：

```json
"conditions": [
  {
    "type": "image",
    "uri": "file:///data/minimax-h3/my-keyframe.png",
    "role": "keyframe",
    "frame_index": 0
  }
]
```

### P55｜路径由服务端解析

**词汇释义**：resolve /rɪˈzɒlv/ v. 解析；server process /ˈsɜːvə ˈprəʊses/ n. phr. 服务进程；actually /ˈæktʃuəli/ adv. 实际地；readable /ˈriːdəbəl/ adj. 可读取的；absolute path /ˈæbsəluːt pɑːθ/ n. phr. 绝对路径；container /kənˈteɪnə/ n. 容器；mount /maʊnt/ v. 挂载。

**译文**：该路径由 SGLang 服务进程解析，而不是由运行 `curl` 的机器解析，因此必须指向服务端实际看得见的文件。`sglang serve` 直接运行在宿主机上时，任何该进程可读的绝对路径都可以；运行在容器中时，文件必须位于已挂载到容器的目录内，例如把宿主机目录挂载为 `/data/minimax-h3`，再引用 `file:///data/minimax-h3/...`。

### P56｜完整媒体参数

**词汇释义**：supported /səˈpɔːtɪd/ adj. 受支持的；condition /kənˈdɪʃən/ n. 条件；media /ˈmiːdiə/ n. 媒体；option /ˈɒpʃən/ n. 选项。

**译文**：支持的完整条件／媒体选项清单，参见 [MiniMax-H3 SGLang cookbook](https://docs.sglang.io/cookbook/diffusion/MiniMax/MiniMax-H3)。

## 07｜Full 2K Workflow：完整 2K 工作流

### P57｜流程目标与初始化

**词汇释义**：combine /kəmˈbaɪn/ v. 结合；locally deployed /ˈləʊkəli dɪˈplɔɪd/ adj. 本地部署的；reproduce /ˌriːprəˈdjuːs/ v. 复现；endpoint /ˈendpɔɪnt/ n. 接口端点；credential /krɪˈdenʃəl/ n. 凭据；configure /kənˈfɪɡə/ v. 配置。

**译文**：本节说明如何将本地 SGLang 服务与官方 H3-Context-IR、H3-Regenerate-2K API 结合，以复现直接调用 MiniMax API 所生成 2K 视频的质量。开始前，配置 SGLang 端点和 MiniMax API 凭据：

```bash
# SGLang 部署地址
SGLANG_DEPLOYMENT_URL="<sglang-deployment-url>"

# MiniMax API 端点（二选一）
# 中国区
MINIMAX_API_BASE="https://api.minimaxi.com"
# 全球区
# MINIMAX_API_BASE="https://api.minimax.io"

# 从 MiniMax 平台取得的 API 令牌
TOKEN="<token>"
```

### P58｜MiniMax 平台文档入口

**词汇释义**：create /kriˈeɪt/ v. 创建；regeneration /ˌriːdʒenəˈreɪʃən/ n. 再生成；documentation /ˌdɒkjʊmenˈteɪʃən/ n. 文档。

**译文**：MiniMax 平台 API 文档：创建 H3-2K 对应文档路径 `/video-generation-v2-create`；H3-Context-IR 对应 `/video-generation-v2-h3-context-ir`；H3-Regenerate-2K 对应 `/video-generation-v2-regeneration`。原文分别提供全球区英文文档与中国区中文文档入口。这些是文档路由名称，不应误当作完整 API 请求地址。

### P59｜本地文件编码与生产环境建议

**词汇释义**：encode /ɪnˈkəʊd/ v. 编码；Base64 专用编码名称，保留；Data URL n. phr. 内嵌数据地址；production /prəˈdʌkʃən/ n. 生产环境；upload /ˌʌpˈləʊd/ v. 上传；publicly accessible /ˈpʌblɪkli əkˈsesəbəl/ adj. 可公开访问的；pass /pɑːs/ v. 传入。

**译文**：以下示例把本地 H3-Base 输出文件编码为 Base64 Data URL。生产使用时，建议把视频上传到可公开访问的地址，并将该地址作为 `base_video` 传入。

### P60｜对照结果

**词汇释义**：reference output /ˈrefərəns ˈaʊtpʊt/ n. phr. 对照输出；directly /dəˈrektli/ adv. 直接地；validate /ˈvælɪdeɪt/ v. 验证。

**译文**：下列每个案例都提供直接通过开放平台 API 生成的 2K 和 768p 对照结果，以便验证。

### P61｜case-T2VA：案例参数和返回元数据

**词汇释义**：text-to-video /tekst tə ˈvɪdiəʊ/ adj. 文生视频的；stage /steɪdʒ/ n. 阶段；request /rɪˈkwest/ n. 请求；succeeded /səkˈsiːdɪd/ v./状态值 已成功；usage /ˈjuːsɪdʒ/ n. 用量；completion /kəmˈpliːʃən/ n. 输出完成内容；modality /məʊˈdæləti/ n. 模态。

**译文**：类型为文生视频，时长 10 秒，画幅 16:9。示例任务模型为 MiniMax-H3，状态 succeeded，类型 h3_context_ir，模态 text。`id`、`created_at`、`updated_at` 是占位符；返回的提示词位于 `task.content.prompt`。示例用量为 total_tokens=8565、prompt_tokens=5650、completion_tokens=2915；这只是源文示例值，不是固定收费或每次调用的预估。

### P62｜T2VA 提示词正文：[Shot 1]

**词汇释义**：cavernous /ˈkævənəs/ adj. 洞穴般宽大的；dimly lit /ˈdɪmli lɪt/ adj. 光线昏暗的；bridge /brɪdʒ/ n. 舰桥；starship /ˈstɑːʃɪp/ n. 星际飞船；console /ˈkɒnsəʊl/ n. 控制台；amber /ˈæmbə/ adj. 琥珀色的；flank /flæŋk/ v. 位于两侧；insignia /ɪnˈsɪɡniə/ n. 徽章；silhouetted /ˌsɪluˈetɪd/ adj. 呈剪影的；clasp /klɑːsp/ v. 紧握；armada /ɑːˈmɑːdə/ n. 庞大舰队；jagged /ˈdʒæɡɪd/ adj. 棱角嶙峋的；dreadnought /ˈdrednɔːt/ n. 无畏级战舰；nebula /ˈnebjʊlə/ n. 星云；thruster /ˈθrʌstə/ n. 推进器。

**译文**：integrated_multimodal_description：[Shot 1] 电影式画面，中全景，缓慢推进。一艘星际飞船的舰桥宽阔如洞穴，光线昏暗；一面巨大的弧形观察窗两侧排列着流线型金属控制台，其琥珀色显示屏发着光。一名四十多岁后段、体格健壮、黑色短发间夹有银丝的女舰长站在中景中央。她穿结构挺括的深海军蓝高领军服，胸前有银色徽章。她背对摄影机，在穿过厚玻璃洒入的冷色星光映衬下呈现剪影；她一动不动，双手紧扣在背后。窗外，庞大的深灰色棱角战舰群在深紫色星云前保持紧密编队悬浮。舰队巨大的尾部推进器开始发出越来越强烈的亮蓝色光芒。

### P63｜T2VA 提示词正文：[Shot 2]

**词汇释义**：close-up /ˈkləʊsʌp/ n. 特写；blinding /ˈblaɪndɪŋ/ adj. 刺眼的；flash /flæʃ/ n. 闪光；wash out /wɒʃ aʊt/ v. phr. 使画面过曝、淹没细节；hyperspace /ˈhaɪpəspeɪs/ n. 超空间；jolt /dʒəʊlt/ v. 猛烈震动；stagger /ˈstæɡə/ v. 踉跄；tense /tens/ v. 绷紧；brace /breɪs/ v. 绷住身体抵抗；tremor /ˈtremə/ n. 震颤；expanse /ɪkˈspæns/ n. 广阔空间；clench /klentʃ/ v. 咬紧、绷紧。

**译文**：[Shot 2] At 00:04.500，镜头切到女舰长面部特写，并强烈抖动。舰队聚能发出的耀眼蓝白色光芒鲜明映在她深色眼睛中。突然，刺眼白光涌过观察窗；舰队跃迁至超空间，背景完全被白光淹没。巨大的空间作用力猛烈震动舰桥，使 Shot 1 中的女舰长略向前踉跄；她肩膀绷紧，明显以身体抵御震颤。强烈白光骤然褪去，只剩昏暗、空旷的紫色星云映在她受硬光照亮的皮肤上；她咬紧下颌，在刚刚空下来的空间中缓缓闭眼。

### P64｜T2VA 整体声景

**词汇释义**：resonant /ˈrezənənt/ adj. 共鸣的；life support /laɪf səˈpɔːt/ n. phr. 生命维持系统；baseline /ˈbeɪslaɪn/ n. 基底；drown out /draʊn aʊt/ v. phr. 盖过；high-pitched /ˌhaɪˈpɪtʃt/ adj. 高音调的；whine /waɪn/ n. 尖啸；deafening /ˈdefənɪŋ/ adj. 震耳欲聋的；crackle /ˈkrækəl/ n. 噼啪声；bulkhead /ˈbʌlkhed/ n. 舱壁；rattle /ˈrætəl/ n. 咔嗒震响；thud /θʌd/ n. 沉闷撞击；hollow /ˈhɒləʊ/ adj. 空洞的；isolated /ˈaɪsəleɪtɪd/ adj. 孤立的。

**译文**：overall_soundscape：飞船生命维持系统低沉、带共鸣的嗡鸣构成底声，很快被窗外舰队为超空间引擎充能时不断升高的电子尖啸盖过。刺眼闪光出现时，巨大的、震耳欲聋的低频轰鸣与尖锐噼啪声爆发，同时伴随舰桥舱壁承受强烈物理应力而震动产生的响亮金属吱嘎、咔嗒震响和深沉撞击。强烈咆哮般的冲击声突然切回空洞、回响的室内底声，只留下孤独舰桥微弱而稳定的嗡鸣。

### P65｜T2VA 画外配乐

**词汇释义**：space opera /speɪs ˈɒpərə/ n. phr. 太空歌剧；orchestral score /ɔːˈkestrəl skɔː/ n. phr. 管弦配乐；solitary /ˈsɒlɪtəri/ adj. 独奏般孤立的；mournful /ˈmɔːnfəl/ adj. 哀伤的；French horn /frentʃ hɔːn/ n. phr. 圆号；dissonance /ˈdɪsənəns/ n. 不协和音；swell /swel/ v. 增强；peak /piːk/ n. 峰值。

**译文**：non_diegetic_music：电影式太空歌剧管弦配乐，慢速；一条孤独、哀伤的圆号旋律位于深沉持续的弦乐不协和音之上，音量和强度快速增长，膨胀至巨大的管弦乐峰值，跃迁之后立即骤然静音。

### P66｜T2VA 请求与结果表

**词汇释义**：reference result /ˈrefərəns rɪˈzʌlt/ n. phr. 对照结果；directly calling /dəˈrektli ˈkɔːlɪŋ/ phr. 直接调用；view script /vjuː skrɪpt/ v. phr. 查看脚本。

**译文**：原表的阶段、请求与结果对应如下：

| 阶段 | 请求脚本 | 结果 |
|---|---|---|
| H3-Context-IR | [full-2k-t2va-h3-context-ir.sh](scripts/readme/full-2k-t2va-h3-context-ir.sh) | 上述任务及增强提示词 |
| H3-Base | [full-2k-t2va-h3-base.sh](scripts/readme/full-2k-t2va-h3-base.sh) | [t2va.mp4](assets/t2va.mp4) |
| H3-Regenerate-2K | [full-2k-t2va-h3-regenerate-2k.sh](scripts/readme/full-2k-t2va-h3-regenerate-2k.sh) | [t2va_2k.mp4](assets/t2va_2k.mp4) |
| 直接调用开放平台的 2K 对照 | [脚本](scripts/readme/full-2k-t2va-reference-2k-result-by-directly-calling-open-platform-api.sh) | [h3_direct_2k.mp4](assets/h3_direct_2k.mp4) |
| 直接调用开放平台的 768p 对照 | [脚本](scripts/readme/full-2k-t2va-reference-768p-result-by-directly-calling-open-platform-api.sh) | [h3_direct_768p.mp4](assets/h3_direct_768p.mp4) |

### P67｜case-I2VA：参数与首帧指令

**词汇释义**：first-frame image-to-video /fɜːst freɪm ˈɪmɪdʒ tə ˈvɪdiəʊ/ n. phr. 首帧图生视频；adaptive /əˈdæptɪv/ adj. 自适应的；fully referenced /ˈfʊli ˈrefərənst/ phr. 完整参考。

**译文**：类型为首帧图生视频，时长 8 秒，画幅自适应。返回示例中的 ratio 为 16:9；任务状态 succeeded，模型 MiniMax-H3，类型 h3_context_ir，模态 text；用量 total_tokens=22822、prompt_tokens=12800、completion_tokens=10022。提示词首先要求：目标视频在 0.00 秒处完整参考属于 [Shot 1] 的 <Picture 1>。

### P68｜I2VA 画面开场与拉面碗

**词汇释义**：shallow depth of field /ˈʃæləʊ depθ əv fiːld/ n. phr. 浅景深；static /ˈstætɪk/ adj. 固定的；cozy /ˈkəʊzi/ adj. 温馨舒适的；intricately patterned /ˈɪntrɪkətli ˈpætənd/ adj. 图案精细复杂的；ceramic /səˈræmɪk/ adj. 陶瓷的；ramen /ˈrɑːmen/ n. 日式拉面；foreground /ˈfɔːɡraʊnd/ n. 前景；crisp /krɪsp/ adj. 清晰锐利的；broth /brɒθ/ n. 汤汁；marbling /ˈmɑːblɪŋ/ n. 脂肪大理石纹理；spiral /ˈspaɪrəl/ adj. 螺旋的；scallion /ˈskæljən/ n. 青葱；nori /ˈnɔːri/ n. 海苔。

**译文**：integrated_multimodal_description：[Shot 1] 真人实拍、电影式浅景深镜头。摄影机在整个八秒时长内完全固定，拍摄传统日式餐室中温馨的家庭聚餐。开场时，最近前景是一只大号蓝白陶瓷拉面碗，纹样精细复杂，焦点清晰锐利。碗放在光滑抛光的长木桌上。碗里浓郁、油润的金棕色汤汁围着黄色卷面，上面有两片厚圆叉烧，能看到脂肪纹理和明显的肉质螺旋花纹。中央堆着大量新切的鲜绿葱花，右边缘插着一片脆挺、深绿色的长方形海苔。

### P69｜I2VA 桌面与背景

**词汇释义**：chopsticks /ˈtʃɒpstɪks/ n. 筷子；chopstick rest /ˈtʃɒpstɪk rest/ n. phr. 筷架；cylindrical /sɪˈlɪndrɪkəl/ adj. 圆柱形的；spherical /ˈsferɪkəl/ adj. 球形的；paper lantern /ˈpeɪpə ˈlæntən/ n. phr. 纸灯笼；ribbed /rɪbd/ adj. 有肋条的；bamboo frame /bæmˈbuː freɪm/ n. phr. 竹骨架；shoji /ˈʃəʊdʒi/ n. 日式纸拉门；lattice /ˈlætɪs/ n. 格栅；lush /lʌʃ/ adj. 繁茂的。

**译文**：碗左边，一双浅棕木筷水平搁在小型深色长方形筷架上，旁边是一只绘有蓝色图案的小圆柱形陶瓷茶杯。桌子右侧，一盏带竹肋骨架的球形纸灯笼置于黑色木座上。背景中，七口之家围坐桌边，起初只是柔软模糊的形象。身后，木格框的传统日式纸拉门敞开，露出室外明亮景色与繁茂绿树。

### P70｜I2VA 蒸汽与焦点转移

**词汇释义**：intensify /ɪnˈtensɪfaɪ/ v. 增强；billow /ˈbɪləʊ/ v. 翻涌；swirling /ˈswɜːlɪŋ/ adj. 旋绕的；deliberate /dɪˈlɪbərət/ adj. 有意而从容的；focus shift /ˈfəʊkəs ʃɪft/ n. phr. 焦点转移；hazy /ˈheɪzi/ adj. 朦胧的；simultaneously /ˌsɪməlˈteɪniəsli/ adv. 同时；translucent veil /trænzˈluːsənt veɪl/ n. phr. 半透明薄幕；locked /lɒkt/ adj. 锁定的。

**译文**：片段开始不久，热拉面汤升起的浓白蒸汽立即变得更强，向上翻涌成厚重旋绕的蒸汽团，不停在碗上方舞动。进入中间几秒时，摄影机保持位置不变，焦点却有意而平顺地向室内深处转移。前景拉面碗、鲜艳配料与蒸汽逐渐软化为朦胧的失焦影像；同时，背景家人变得清晰、细节分明。浓蒸汽继续从前景升起，在摄影机和家人之间形成动态的半透明薄幕。焦点牢固锁在背景后，热闹的家庭晚餐鲜活起来。

### P71｜I2VA 家庭成员动作

**词汇释义**：lean forward /liːn ˈfɔːwəd/ v. phr. 身体前倾；animatedly /ˈænɪmeɪtɪdli/ adv. 生动活跃地；silent exchange /ˈsaɪlənt ɪksˈtʃeɪndʒ/ n. phr. 无声交流；blouse /blaʊz/ n. 女式衬衫；crinkle /ˈkrɪŋkəl/ v. 起细纹；pick up /pɪk ʌp/ v. phr. 夹取；pickled vegetable /ˈpɪkəld ˈvedʒtəbəl/ n. phr. 腌菜；clasp /klɑːsp/ v. 交握；cadence /ˈkeɪdəns/ n. 节奏；comforting /ˈkʌmfətɪŋ/ adj. 令人舒适的。

**译文**：左边穿深海军蓝长袖衬衫的男子身体前倾，在无声交流中嘴部活跃地运动。旁边穿干净白色短袖 T 恤的小女孩灿烂微笑，看向桌子中央。最左边穿柔软浅蓝色长袖衬衫的女子稍微转头，温柔微笑。桌子对面穿浅灰色纽扣衬衫的女子大笑，眼角起细纹，双手放在盘子附近。更后方穿深灰色上衣的女子用木筷从中央盛着鲜红腌菜的陶瓷盘中夹起一小块食物。后方中央穿浅灰毛衣的女子温柔微笑，双手轻轻交握在身前，观察家人的互动。片段剩余时间内，家人继续活跃地以身体交流，嘴部按连续而无声的交谈节奏运动；前景失焦拉面碗中的浓白蒸汽始终不断升起，为温暖聚餐增添舒适氛围。

### P72｜I2VA 整体声景

**词汇释义**：airy /ˈeəri/ adj. 气流般轻盈的；rustle /ˈrʌsəl/ n. 窸窣声；hissing /ˈhɪsɪŋ/ n. 嘶声；bubbling /ˈbʌbəlɪŋ/ n. 冒泡声；bustling /ˈbʌslɪŋ/ adj. 热闹忙碌的；dominant /ˈdɒmɪnənt/ adj. 占主导的；clinking /ˈklɪŋkɪŋ/ n. 清脆碰响；muffled /ˈmʌfəld/ adj. 闷响的；cotton /ˈkɒtən/ n. 棉；wool /wʊl/ n. 羊毛；gesture /ˈdʒestʃə/ v. 做手势。

**译文**：overall_soundscape：开头是安静室内底声，混有前景热拉面碗浓蒸汽翻涌产生的微弱气流窸窣声，以及浓汤细微持续的嘶声与冒泡声。视觉焦点转向室内深处时，热闹家庭晚餐的物理声音变成听觉前景。家人伸手取食时，陶瓷碗以及木筷触碰盘子的清脆碰响清晰可闻。随后是杯子放在光滑木桌上微弱闷响，以及家人前倾、做手势时棉毛衣物细微而有节奏的摩擦声，准确表现共享用餐活跃的物理氛围。

### P73｜I2VA 画外配乐

**词汇释义**：heartwarming /ˈhɑːtˌwɔːmɪŋ/ adj. 温暖人心的；acoustic guitar /əˈkuːstɪk ɡɪˈtɑː/ n. phr. 原声吉他；melody /ˈmelədi/ n. 旋律；resonant /ˈrezənənt/ adj. 共鸣的；koto /ˈkəʊtəʊ/ n. 日本筝；nostalgic /nɒˈstældʒɪk/ adj. 怀旧的；joyful /ˈdʒɔɪfəl/ adj. 欢快的。

**译文**：non_diegetic_music：温柔、温暖人心的原声吉他旋律轻轻在背景中奏响，伴以传统日本筝细微而有共鸣的乐音。音乐保持缓慢舒适的速度，加强家庭聚餐温馨、怀旧而欢乐的氛围。

### P74｜I2VA 请求与结果表

**词汇释义**：stage /steɪdʒ/ n. 阶段；reference /ˈrefərəns/ n. 对照；regenerate /ˌriːˈdʒenəreɪt/ v. 再生成。

**译文**：阶段与结果对应如下：

| 阶段 | 请求脚本 | 结果 |
|---|---|---|
| H3-Context-IR | [full-2k-i2va-h3-context-ir.sh](scripts/readme/full-2k-i2va-h3-context-ir.sh) | 上述增强提示词 |
| H3-Base | [full-2k-i2va-h3-base.sh](scripts/readme/full-2k-i2va-h3-base.sh) | [i2va.mp4](assets/i2va.mp4) |
| H3-Regenerate-2K | [full-2k-i2va-h3-regenerate-2k.sh](scripts/readme/full-2k-i2va-h3-regenerate-2k.sh) | [i2va_2k.mp4](assets/i2va_2k.mp4) |
| 直接调用开放平台的 2K 对照 | [脚本](scripts/readme/full-2k-i2va-reference-2k-result-by-directly-calling-open-platform-api.sh) | [i2va_direct_2k.mp4](assets/i2va_direct_2k.mp4) |
| 直接调用开放平台的 768p 对照 | [脚本](scripts/readme/full-2k-i2va-reference-768p-result-by-directly-calling-open-platform-api.sh) | [i2va_direct_768p.mp4](assets/i2va_direct_768p.mp4) |

### P75｜case-Ref2VA：参数与元数据

**词汇释义**：multimodal reference-to-video /ˌmʌltiˈməʊdəl ˈrefərəns tə ˈvɪdiəʊ/ n. phr. 多模态参考生视频；adaptive /əˈdæptɪv/ adj. 自适应的；usage /ˈjuːsɪdʒ/ n. 用量。

**译文**：类型为多模态参考生视频（视频＋音频），时长 5 秒，画幅自适应。返回示例 ratio 为 16:9；模型 MiniMax-H3，状态 succeeded，类型 h3_context_ir，模态 text；用量 total_tokens=39299、prompt_tokens=33323、completion_tokens=5976。任务标识和创建／更新时间仍用源文占位符表示。

### P76｜Ref2VA 的参考内容定义

**词汇释义**：wavy /ˈweɪvi/ adj. 波浪状的；blonde /blɒnd/ adj. 金发的；suit jacket /suːt ˈdʒækɪt/ n. phr. 西装上衣；matching /ˈmætʃɪŋ/ adj. 配套的；trousers /ˈtraʊzəz/ n. 长裤；unbuttoned /ʌnˈbʌtənd/ adj. 解开纽扣的；lamb /læm/ n. 羔羊；synchronized audio track /ˈsɪŋkrənaɪzd ˈɔːdiəʊ træk/ n. phr. 同步音轨；voice timbre /vɔɪs ˈtæmbə/ n. phr. 音色；voiceover /ˈvɔɪsəʊvə/ n. 画外音。

**译文**：subject_definitions：

`<Subject 1>` 是 `<Video 1>` 中的年轻男子，留金色短卷发，穿亮粉色西装上衣和配套粉色长裤、解开纽扣的白衬衫，戴银戒指，怀抱一只小黑羊。

`<Video 1>` 是编辑任务的源视频。

`<Audio 1>` 是 `<Video 1>` 的同步音轨，提供背景音乐。

`<Audio 2>` 是 `<Subject 1>` 的声音音色参考，其中包含男性口述画外音。

### P77｜Ref2VA 摘要

**词汇释义**：edited version /ˈedɪtɪd ˈvɜːʃən/ n. phr. 编辑后的版本；grassy field /ˈɡrɑːsi fiːld/ n. phr. 草地；animate /ˈænɪmeɪt/ v. 使动起来；user-provided /ˈjuːzə prəˈvaɪdɪd/ adj. 用户提供的；partially reused /ˈpɑːʃəli ˌriːˈjuːzd/ phr. 部分复用；continuous /kənˈtɪnjuəs/ adj. 连续的；spoken line /ˈspəʊkən laɪn/ n. phr. 台词。

**译文**：summary：[video editing + audio reference + audio reuse] 目标视频是 `<Video 1>` 的编辑版本。穿亮粉色西装、怀抱黑羊的 `<Subject 1>` 站在草地上，背景有其他白色羔羊。编辑使 `<Subject 1>` 的面部动起来，说出用户提供的对白。`<Audio 1>` 部分复用为持续背景音乐；目标视频则参考 `<Audio 2>` 平静的男性音色，为 `<Subject 1>` 生成台词。

### P78｜Ref2VA 保留分析

**词汇释义**：retain /rɪˈteɪn/ v. 保留；accessory /əkˈsesəri/ n. 配饰；framing /ˈfreɪmɪŋ/ n. 取景；golden hour /ˈɡəʊldən ˈaʊə/ n. phr. 黄金时刻；setting /ˈsetɪŋ/ n. 场景环境；maintain /meɪnˈteɪn/ v. 维持；atmospheric /ˌætməsˈferɪk/ adj. 营造氛围的；mix /mɪks/ v. 混音。

**译文**：retention_analysis：

`<Subject 1>`（出现在 [Shot 1]）：fully_preserved——保留男子身份、金色卷发、粉色西装、白衬衫、配饰与怀抱的黑羊，同时新增加嘴部说话动画。

`<Video 1>`（源视频编辑）：fully_preserved——编辑中央人物时，保留原有摄影机取景、温暖黄金时刻光照、草坡场景及背景白羊。

`<Audio 1>`：partially_copy——复用其中营造氛围的背景音乐，并混在新增对白下方。

`<Audio 2>`：reference——目标音频参考其中的男性音色，生成 `<Subject 1>` 的对白。

### P79｜Ref2VA 详细描述：场景与主体

**词汇释义**：photographic /ˌfəʊtəˈɡræfɪk/ adj. 摄影式的；casually /ˈkæʒuəli/ adv. 随意地；confidently /ˈkɒnfɪdəntli/ adv. 自信地；sunlit /ˈsʌnlɪt/ adj. 阳光照耀的；pasture /ˈpɑːstʃə/ n. 牧场；securely /sɪˈkjʊəli/ adv. 稳稳地；cast /kɑːst/ v. 投下；graze /ɡreɪz/ v. 吃草；rolling hill /ˈrəʊlɪŋ hɪl/ n. phr. 起伏山坡；pale /peɪl/ adj. 淡色的。

**译文**：detailed_description：目标视频采用写实摄影风格。[Shot 1] 镜头从源 `<Video 1>` 开始，展示 `<Subject 1>`：一名留金色短卷发、穿亮粉西装上衣和配套长裤、白衬衫随意解开纽扣的年轻男子。他自信地站在阳光照耀的绿色牧场中，温柔而稳当地抱着小黑羊。温暖的黄金时刻光线在他的脸上和亮粉西装面料上投下柔和阴影。身后，几只白羊在起伏草坡上站立、吃草，背景是晴朗的淡蓝天空。`<Audio 1>` 中营造氛围的背景音乐持续贯穿场景。

### P80｜Ref2VA 详细描述：对白与收尾

**词汇释义**：physically speak /ˈfɪzɪkəli spiːk/ v. phr. 实际开口说话；sync /sɪŋk/ v. 同步；thoughtfully /ˈθɔːtfəli/ adv. 若有所思地；subtly /ˈsʌtəli/ adv. 细微地；shift one's weight /ʃɪft weɪt/ v. phr. 转移重心；cradle /ˈkreɪdəl/ v. 轻柔托抱；jaw /dʒɔː/ n. 下颌；cease /siːs/ v. 停止；horizon /həˈraɪzən/ n. 地平线；stroke /strəʊk/ v. 抚摸；fleece /fliːs/ n. 羊毛；tranquil /ˈtræŋkwɪl/ adj. 宁静的。

**译文**：`<Subject 1>` 实际开口说话，嘴部动作自然同步新对白，声音音色参考 `<Audio 2>` 平静的男性表达。他若有所思地望向前方，`<Subject 1> (S1)` 轻声说：`<d>[English] Follow the wind, live free.</d>` 说话时，他细微转移重心，托抱着安静休息的黑羊，摄影机缓慢推进。`<Subject 1> (S1)` 接着说：`<d>[English] Leave worries behind, enjoy the moment.</d>` 声音停止的确切时刻，他嘴唇合拢成放松、平和的微笑，下颌停止说话动作。随后他把目光稍微移向地平线，手指温柔抚摸黑羊毛，摄影机保持这一宁静、明亮状态，直到视频结束。

台词释义：“随风而行，自由生活。”“抛开忧虑，享受当下。”原英文台词未替换。

### P81｜Ref2VA 整体声景

**词汇释义**：consist /kənˈsɪst/ v. 由……组成；continuous /kənˈtɪnjuəs/ adj. 持续的；overlay /ˌəʊvəˈleɪ/ v. 叠加；calm /kɑːm/ adj. 平静的；main character /meɪn ˈkærəktə/ n. phr. 主角。

**译文**：overall_soundscape：声景由 `<Audio 1>` 持续、营造氛围的背景音乐构成，上面叠加主角清晰、平静的男性对白，其音色参考 `<Audio 2>`。

### P82｜Ref2VA 画外配乐

**词汇释义**：sustained /səˈsteɪnd/ adj. 持续的；score /skɔː/ n. 配乐；quietly /ˈkwaɪətli/ adv. 轻声地；spoken dialogue /ˈspəʊkən ˈdaɪəlɒɡ/ n. phr. 口头对白。

**译文**：non_diegetic_music：复用 `<Audio 1>` 营造氛围、持续的背景音乐作为连续配乐，在对白下方轻轻播放。

### P83｜Ref2VA 请求与结果表

**词汇释义**：reference /ˈrefərəns/ n. 对照；direct /dəˈrekt/ adj. 直接的；platform /ˈplætfɔːm/ n. 平台。

**译文**：原表保持以下对应关系，不将名称相近的两行合并：

| 阶段 | 请求脚本 | 结果 |
|---|---|---|
| H3-Context-IR | [full-2k-ref2va-h3-context-ir.sh](scripts/readme/full-2k-ref2va-h3-context-ir.sh) | 上述增强提示词 |
| H3-Base | [full-2k-ref2va-h3-base.sh](scripts/readme/full-2k-ref2va-h3-base.sh) | [r2va.mp4](assets/r2va.mp4) |
| 直接调用开放平台的 2K 对照 | [脚本](scripts/readme/full-2k-ref2va-reference-2k-result-by-directly-calling-open-platform-api.sh) | [r2va_2k.mp4](assets/r2va_2k.mp4) |
| 开放平台 H3 API 2K 对照 | [脚本](scripts/readme/full-2k-ref2va-h3-api-2k-in-open-platform-for-reference.sh) | [r2va_direct_2k.mp4](assets/r2va_direct_2k.mp4) |
| 直接调用开放平台的 768p 对照 | [脚本](scripts/readme/full-2k-ref2va-reference-768p-result-by-directly-calling-open-platform-api.sh) | [r2va_direct_768p.mp4](assets/r2va_direct_768p.mp4) |

## 08｜Prompting Guidance：提示词指导

### P84｜指南文件的存放说明

**词汇释义**：guidance /ˈɡaɪdəns/ n. 指导；copy /ˈkɒpi/ v. 复制；layout /ˈleɪaʊt/ n. 布局；minimal /ˈmɪnɪməl/ adj. 精简的。

**译文**：为了保持 Markdown 布局精简，Hugging Face 发布包中的提示词指导文档没有复制到本仓库。

**译注**：此句按源文保留；本仓库同时存在前文介绍的 `skills/h3-prompt-writing/references/base-en.txt` 和 `ref-en.txt`，不能据本句推断仓库不存在任何提示词参考文件。

## 09｜License：许可协议

### P85｜模型许可证

**词汇释义**：release /rɪˈliːs/ v. 发布；community /kəˈmjuːnəti/ n. 社区；license agreement /ˈlaɪsəns əˈɡriːmənt/ n. phr. 许可协议。

**译文**：MiniMax H3 按照 [MiniMax H3 Community License Agreement](https://huggingface.co/MiniMaxAI/MiniMax-H3/blob/main/LICENSE) 发布。

## 10｜Contact Us：联系我们

### P86｜联系地址

**词汇释义**：contact /ˈkɒntækt/ v. 联系。

**译文**：通过 `model@minimax.io` 联系我们。

---

### 译者核对说明

本译本只翻译和注释源文，不执行安装、模型推理或 API 请求。JSON 示例的任务元数据以等值说明列出，运行时仍以原脚本与源 JSON 为准。README 的某些案例把背景音乐、对白写入 overall_soundscape，或使用抽象情绪配乐词；这与提示词指南的部分规则存在表述差异，译本保留原例，没有把修改后的案例冒充原文。I2VA 案例写有七名家人，但只逐一描写了其中六人的动作；译本没有擅自补造第七人的特征。
