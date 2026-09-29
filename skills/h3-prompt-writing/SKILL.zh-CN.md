# H3 提示词编写｜逐段注释译本

源文件：[SKILL.md](./SKILL.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源文件 Git blob：`b6d9b2839384a588763a9c24315225dd8ce19d56`。

本文件是独立的学习译本，不替换原 Skill。按源文顺序保留英文并提供词汇释义与简体中文翻译。音标采用常见英语读法；`n.` 名词，`v.` 动词，`adj.` 形容词，`adv.` 副词，`n. phr.` 名词短语，`v. phr.` 动词短语，`abbr.` 缩写。字段名、标签、路径与模式代码保持原样；缩写按字母或全称理解，不为产品标识杜撰读音。

## 01｜名称、描述与兼容性

**原文**：`name: h3-prompt-writing`

**词汇释义**：prompt /prɒmpt/ n. 提示词；writing /ˈraɪtɪŋ/ n. 编写；name /neɪm/ n. 名称。

**译文**：名称：`h3-prompt-writing`，即 H3 提示词编写。

**原文**：Write MiniMax H3 video generation prompts for T2VA, I2VA, FL2VA, L2VA, and Ref2VA. Use when rewriting multimodal requests into H3 prompt structures, composing integrated_multimodal_description, overall_soundscape, and non_diegetic_music, aligning keyframes, or defining reference labels for images, videos, and audio.

**词汇释义**：generation /ˌdʒenəˈreɪʃən/ n. 生成；rewrite /ˌriːˈraɪt/ v. 改写；multimodal /ˌmʌltiˈməʊdəl/ adj. 多模态的；request /rɪˈkwest/ n. 请求、要求；structure /ˈstrʌktʃə/ n. 结构；compose /kəmˈpəʊz/ v. 组织、编写；integrated /ˈɪntɪɡreɪtɪd/ adj. 综合的；soundscape /ˈsaʊndskeɪp/ n. 声景；non-diegetic /ˌnɒn daɪəˈdʒetɪk/ adj. 不属于故事世界内可感知声音的；align /əˈlaɪn/ v. 对齐；keyframe /ˈkiːfreɪm/ n. 关键帧；reference /ˈrefərəns/ n. 参考；label /ˈleɪbəl/ n. 标签。

**译文**：为 T2VA、I2VA、FL2VA、L2VA 和 Ref2VA 编写 MiniMax H3 视频生成提示词。当需要把多模态请求改写成 H3 提示词结构、编写 `integrated_multimodal_description`、`overall_soundscape` 与 `non_diegetic_music`，对齐关键帧，或为图片、视频和音频定义参考标签时，使用此 Skill。

**原文**：Portable to any agent that can read local files — no external API calls, MiniMax Hub tools, or proprietary runtime required. The agents/openai.yaml file only adds optional ChatGPT/Codex UI metadata; it does not restrict the skill to OpenAI agents.

**词汇释义**：portable /ˈpɔːtəbəl/ adj. 可移植的；agent /ˈeɪdʒənt/ n. 智能体；local /ˈləʊkəl/ adj. 本地的；external /ɪkˈstɜːnəl/ adj. 外部的；API abbr. Application Programming Interface，应用程序编程接口；proprietary /prəˈpraɪətəri/ adj. 专有的；runtime /ˈrʌntaɪm/ n. 运行环境；optional /ˈɒpʃənəl/ adj. 可选的；UI abbr. User Interface，用户界面；metadata /ˈmetədeɪtə/ n. 元数据；restrict /rɪˈstrɪkt/ v. 限制。

**译文**：可移植到任何能够读取本地文件的智能体；不需要外部 API 调用、MiniMax Hub 工具或专有运行环境。`agents/openai.yaml` 仅添加可选的 ChatGPT/Codex 用户界面元数据，并不把该 Skill 限定为只能由 OpenAI 智能体使用。

## 02｜Workflow：工作流程

**原文**：1. Identify the input mode: T2VA, I2VA, FL2VA, L2VA, or full-reference Ref2VA.

**词汇释义**：workflow /ˈwɜːkfləʊ/ n. 工作流程；identify /aɪˈdentɪfaɪ/ v. 识别、确定；input /ˈɪnpʊt/ n. 输入；mode /məʊd/ n. 模式；full-reference /fʊl ˈrefərəns/ adj. 全参考的。

**译文**：1. 确定输入模式：T2VA、I2VA、FL2VA、L2VA，或全参考 Ref2VA。

**原文**：2. For base text/keyframe modes, read `references/base-en.txt` and follow its final prompt structure.

**词汇释义**：base /beɪs/ adj. 基础的；text /tekst/ n. 文本；keyframe /ˈkiːfreɪm/ n. 关键帧；follow /ˈfɒləʊ/ v. 遵循；final /ˈfaɪnəl/ adj. 最终的；structure /ˈstrʌktʃə/ n. 结构。

**译文**：2. 对于基础文本／关键帧模式，读取 `references/base-en.txt`，并遵循其中规定的最终提示词结构。

**原文**：3. For full-reference mode, read `references/ref-en.txt` and follow its six-section rewrite format.

**词汇释义**：section /ˈsekʃən/ n. 分节、部分；rewrite /ˈriːraɪt/ n. 改写稿；format /ˈfɔːmæt/ n. 格式；full-reference /fʊl ˈrefərəns/ adj. 全参考的。

**译文**：3. 对于全参考模式，读取 `references/ref-en.txt`，并遵循其六部分改写格式。

**原文**：4. Preserve the exact field names, section order, labels, and timing notation from the selected guide.

**词汇释义**：preserve /prɪˈzɜːv/ v. 保留；exact /ɪɡˈzækt/ adj. 完全准确的；field /fiːld/ n. 字段；order /ˈɔːdə/ n. 顺序；timing /ˈtaɪmɪŋ/ n. 时间安排；notation /nəʊˈteɪʃən/ n. 记法；selected /sɪˈlektɪd/ adj. 已选定的；guide /ɡaɪd/ n. 指南。

**译文**：4. 精确保留所选指南中的字段名称、分节顺序、标签和时间记法。

## 03｜Base Modes：基础模式

**原文**：T2VA: build the full audiovisual timeline from text.

**词汇释义**：T2VA abbr. Text-to-Video-and-Audio，文生音视频；build /bɪld/ v. 构建；audiovisual /ˌɔːdiəʊˈvɪʒuəl/ adj. 视听的；timeline /ˈtaɪmlaɪn/ n. 时间线。

**译文**：T2VA：从文本构建完整的视听时间线。

**原文**：I2VA: start from the first frame and develop forward from it.

**词汇释义**：I2VA abbr. Image-to-Video-and-Audio，图生音视频；frame /freɪm/ n. 帧；develop /dɪˈveləp/ v. 展开、发展；forward /ˈfɔːwəd/ adv. 向前、向后续时间推进。

**译文**：I2VA：从首帧出发，并以该首帧为基础向后续时刻展开。

**原文**：FL2VA: describe the continuous path between the first and last frames.

**词汇释义**：FL2VA abbr. First-and-Last-Frame-to-Video-and-Audio，首尾帧生音视频；describe /dɪˈskraɪb/ v. 描述；continuous /kənˈtɪnjuəs/ adj. 连续的；path /pɑːθ/ n. 路径。

**译文**：FL2VA：描述从首帧到尾帧之间的连续变化路径。

**原文**：L2VA: infer a plausible opening and converge to the supplied last frame.

**词汇释义**：L2VA abbr. Last-Frame-to-Video-and-Audio，尾帧生音视频；infer /ɪnˈfɜː/ v. 推断；plausible /ˈplɔːzəbəl/ adj. 合理可信的；opening /ˈəʊpənɪŋ/ n. 开场；converge /kənˈvɜːdʒ/ v. 逐步趋近、收敛；supplied /səˈplaɪd/ adj. 已提供的。

**译文**：L2VA：推断一个合理的开场，并逐步趋近所提供的尾帧。

**原文**：Use `integrated_multimodal_description`, `overall_soundscape`, and `non_diegetic_music` in the order shown in `references/base-en.txt`.

**词汇释义**：integrated /ˈɪntɪɡreɪtɪd/ adj. 综合的；description /dɪˈskrɪpʃən/ n. 描述；overall /ˌəʊvərˈɔːl/ adj. 整体的；soundscape /ˈsaʊndskeɪp/ n. 声景；non-diegetic music /ˌnɒn daɪəˈdʒetɪk ˈmjuːzɪk/ n. phr. 画外配乐；order /ˈɔːdə/ n. 顺序。

**译文**：按照 `references/base-en.txt` 展示的顺序，使用 `integrated_multimodal_description`（综合多模态描述）、`overall_soundscape`（整体声景）和 `non_diegetic_music`（画外配乐）。

## 04｜Full-Reference Mode：全参考模式

**原文**：Ref2VA rewrites use `subject_definitions`, `summary`, `retention_analysis`, `detailed_description`, `overall_soundscape`, and `non_diegetic_music` in that order. Reference labels stay consistent across all sections.

**词汇释义**：Ref2VA abbr. Reference-to-Video-and-Audio，参考素材驱动的音视频生成；subject /ˈsʌbdʒɪkt/ n. 主体、参考内容单元；definition /ˌdefɪˈnɪʃən/ n. 定义；summary /ˈsʌməri/ n. 摘要；retention /rɪˈtenʃən/ n. 保留；analysis /əˈnæləsɪs/ n. 分析；detailed /ˈdiːteɪld/ adj. 详细的；consistent /kənˈsɪstənt/ adj. 一致的。

**译文**：Ref2VA 改写稿依次使用 `subject_definitions`（参考内容定义）、`summary`（任务摘要）、`retention_analysis`（保留分析）、`detailed_description`（详细描述）、`overall_soundscape`（整体声景）和 `non_diegetic_music`（画外配乐）。参考标签在所有部分中必须保持一致。

**原文**：Read `references/ref-en.txt` for label rules, retention analysis, and complete examples.

**词汇释义**：label /ˈleɪbəl/ n. 标签；rule /ruːl/ n. 规则；retention analysis /rɪˈtenʃən əˈnæləsɪs/ n. phr. 保留分析；complete /kəmˈpliːt/ adj. 完整的；example /ɪɡˈzɑːmpəl/ n. 示例。

**译文**：关于标签规则、保留分析和完整示例，请阅读 `references/ref-en.txt`。

## 05｜Output Rules：输出规则

**原文**：Write rewrite sections in English; preserve dialogue, lyrics, and visible scene text in their original language.

**词汇释义**：output /ˈaʊtpʊt/ n. 输出；dialogue /ˈdaɪəlɒɡ/ n. 对白；lyrics /ˈlɪrɪks/ n. 歌词；visible /ˈvɪzəbəl/ adj. 可见的；scene /siːn/ n. 场景；original /əˈrɪdʒənəl/ adj. 原始的；language /ˈlæŋɡwɪdʒ/ n. 语言。

**译文**：各个改写部分使用英文；对白、歌词以及场景中可见的文字保留原语言。

**原文**：Describe each shot by composition, subjects, environment, actions, camera, sound, and the exact point where referenced content appears.

**词汇释义**：shot /ʃɒt/ n. 镜头；composition /ˌkɒmpəˈzɪʃən/ n. 构图；subject /ˈsʌbdʒɪkt/ n. 主体；environment /ɪnˈvaɪrənmənt/ n. 环境；action /ˈækʃən/ n. 动作；camera /ˈkæmərə/ n. 摄影机；sound /saʊnd/ n. 声音；appear /əˈpɪə/ v. 出现；exact point /ɪɡˈzækt pɔɪnt/ n. phr. 确切时点或位置。

**译文**：描述每个镜头时，应写明构图、主体、环境、动作、摄影机、声音，以及参考内容出现的确切时点或位置。

**原文**：Avoid plot summaries, unresolved reference labels, and timing that does not match the requested duration.

**词汇释义**：avoid /əˈvɔɪd/ v. 避免；plot /plɒt/ n. 情节；summary /ˈsʌməri/ n. 梗概；unresolved /ˌʌnrɪˈzɒlvd/ adj. 未解析、未明确对应的；match /mætʃ/ v. 匹配；requested /rɪˈkwestɪd/ adj. 所要求的；duration /djʊəˈreɪʃən/ n. 持续时间、片长。

**译文**：避免仅写情节梗概、使用没有明确对应关系的参考标签，或给出与要求片长不一致的时间安排。

## 06｜Tips for Better Results：改善结果的提示

**原文**：Always match the total duration of the description to the requested video length (4–15 seconds).

**词汇释义**：match /mætʃ/ v. 使一致；total /ˈtəʊtəl/ adj. 总计的；duration /djʊəˈreɪʃən/ n. 时长；requested /rɪˈkwestɪd/ adj. 所要求的；length /leŋθ/ n. 长度，此处指片长。

**译文**：始终让描述覆盖的总时长与要求的视频片长一致，即 4—15 秒。

**原文**：Keep reference labels consistent (e.g. `<Picture 1>`, `<Video 1>`, `<Audio 1>`) across every section.

**词汇释义**：reference label /ˈrefərəns ˈleɪbəl/ n. phr. 参考标签；consistent /kənˈsɪstənt/ adj. 一致的；section /ˈsekʃən/ n. 部分。

**译文**：在每一部分中保持参考标签一致，例如 `<Picture 1>`、`<Video 1>` 和 `<Audio 1>`。

**原文**：Prefer concrete visual and audio details over abstract words like "cinematic" or "beautiful".

**词汇释义**：prefer /prɪˈfɜː/ v. 优先选择；concrete /ˈkɒŋkriːt/ adj. 具体的；visual /ˈvɪʒuəl/ adj. 视觉的；detail /ˈdiːteɪl/ n. 细节；abstract /ˈæbstrækt/ adj. 抽象的；cinematic /ˌsɪnəˈmætɪk/ adj. 电影式的；beautiful /ˈbjuːtɪfəl/ adj. 美丽的。

**译文**：优先提供具体的视觉和音频细节，而不是使用“cinematic（电影式的）”或“beautiful（美丽的）”这类抽象词语。

**原文**：When using keyframes (I2VA / FL2VA / L2VA), clearly state how the first and/or last frame connects to the timeline.

**词汇释义**：keyframe /ˈkiːfreɪm/ n. 关键帧；clearly /ˈklɪəli/ adv. 明确地；state /steɪt/ v. 陈述、说明；connect /kəˈnekt/ v. 关联、衔接；timeline /ˈtaɪmlaɪn/ n. 时间线。

**译文**：使用关键帧模式（I2VA／FL2VA／L2VA）时，明确说明首帧和／或尾帧如何与时间线衔接。
