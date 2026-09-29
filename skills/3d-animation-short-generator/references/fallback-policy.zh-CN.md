# Generation Failure and Drift Fallback Policy｜生成失败与漂移回退策略：逐段注释译本

源文件：[fallback-policy.md](./fallback-policy.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`ec8753c963f1b9c305549512c8a30f1ee03d868b`。本文件按源文顺序先释义、再翻译，不替换源文件。以下命令式句子是被翻译的工作流规则，不表示本次执行视频或图像生成。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语。

## 一、Failure fallback per video model：各视频模型的失败回退

### 01｜H3 回退阶梯

**词汇释义**：failure /ˈfeɪljə/ n. 失败；drift /drɪft/ v./n. 偏移、漂移；fallback /ˈfɔːlbæk/ n. 回退方案；ladder /ˈlædə/ n. 阶梯；clip /klɪp/ n. 视频片段。

**译文**：片段失败或发生漂移时，H3 按以下阶梯回退。

### 02｜第一次重试

**词汇释义**：retry /ˌriːˈtraɪ/ n. 重试；regenerate /ˌriːˈdʒenəreɪt/ v. 再生成；prefix /ˈpriːfɪks/ n. 前缀；strengthen /ˈstreŋθən/ v. 加强；quote /kwəʊt/ v. 引用；exact /ɪɡˈzækt/ adj. 原样准确的；reference anchor /ˈrefərəns ˈæŋkə/ n. phr. 参考锚点。

**译文**：第一次重试：重新生成同一片段，在 H3 提示词前缀中原样引用表格里的 `Reference Anchors` 块，以加强约束。

### 03｜第二次重试

**词汇释义**：shorten /ˈʃɔːtən/ v. 缩短；shot /ʃɒt/ n. 镜头；split /splɪt/ v. 拆分；dropped /drɒpt/ adj. 被移出的；adjacent /əˈdʒeɪsənt/ adj. 相邻的；row /rəʊ/ n. 表格行；self-check /self tʃek/ n. 自检；render /ˈrendə/ v. 渲染。

**译文**：第二次重试：将镜头缩短至不超过 6 秒，把移出的秒数分配到步骤 5 中一个新增的相邻行；重新运行步骤 5.5 自检，再渲染。

### 04｜第三次重试

**词汇释义**：switch /swɪtʃ/ v. 切换；mixed mode /mɪkst məʊd/ n. phr. 混合模式；performance fallback /pəˈfɔːməns ˈfɔːlbæk/ n. phr. 性能回退；one click /wʌn klɪk/ n. phr. 一次点击；re-architecture /ˌriːˈɑːkɪtektʃə/ n. 重新设计架构。

**译文**：第三次重试：将失败镜头改用 Seedance 2.0。这正是混合模式存在的原因——性能回退只需一次切换，不需要重新设计整套架构。

### 05｜同一镜头三次失败之后

**词汇释义**：attempt /əˈtempt/ n. 尝试；pause /pɔːz/ v. 暂停；choice card /tʃɔɪs kɑːd/ n. phr. 选择卡片；loosen /ˈluːsən/ v. 放宽；prop /prɒp/ n. 道具；simplify /ˈsɪmplɪfaɪ/ v. 简化；hook /hʊk/ n. 吸引注意的情节抓手；skip /skɪp/ v. 跳过；placeholder /ˈpleɪshəʊldə/ n. 占位项；downstream /ˌdaʊnˈstriːm/ adj. 后续流程的；manually /ˈmænjuəli/ adv. 手动地；bind /baɪnd/ v. 绑定。

**译文**：同一镜头连续三次尝试失败后，暂停并用选择卡片询问用户，选项为：仅把该镜头切换至 Seedance 2.0；放宽要求，例如减少一道具、简化动作或降低情节抓手强度；跳过该镜头，添加 `placeholder: missing clip` 注记，供后续审阅；或手动提供参考视频，以绑定素材代替生成。

### 06｜Seedance 2.0 回退阶梯的适用条件

**词汇释义**：explicitly /ɪkˈsplɪsɪtli/ adv. 明确地；chosen /ˈtʃəʊzən/ v./adj. 已选择的；global model /ˈɡləʊbəl ˈmɒdəl/ n. phr. 全局模型。

**译文**：用户已明确选择 Seedance 作为全局模型，或 H3 已经失败三次后，使用以下 Seedance 2.0 回退阶梯。

### 07｜第一次重试

**词汇释义**：strengthened prompt /ˈstreŋθənd prɒmpt/ n. phr. 强化后的提示词；quote /kwəʊt/ v. 引用；block /blɒk/ n. 内容块。

**译文**：第一次重试：重新生成，使用引用了 `Reference Anchors` 块的强化提示词。

### 08｜第二次重试

**词汇释义**：drop /drɒp/ v. 去掉；reference image /ˈrefərəns ˈɪmɪdʒ/ n. phr. 参考图像；text-only /tekst ˈəʊnli/ adj. 仅文本的。

**译文**：第二次重试：去掉参考图像，改用纯文本生成。

### 09｜第三次重试

**词汇释义**：shorten /ˈʃɔːtən/ v. 缩短；split /splɪt/ v. 拆分；new row /njuː rəʊ/ n. phr. 新行。

**译文**：第三次重试：将镜头缩短至不超过 6 秒，并把移出的秒数拆分到新行中。

### 10｜三次失败后询问

**词汇释义**：failed attempt /feɪld əˈtempt/ n. phr. 失败尝试；switch /swɪtʃ/ v. 切换；loosen /ˈluːsən/ v. 放宽；supply /səˈplaɪ/ v. 提供。

**译文**：三次尝试失败之后，询问用户：该镜头切换到 H3、放宽要求、跳过镜头，或提供参考视频。

## 二、After all clips are rendered：全部片段渲染之后

### 11｜画布排列与分组

**词汇释义**：canvas /ˈkænvəs/ n. 画布；shot order /ʃɒt ˈɔːdə/ n. phr. 镜头顺序；group /ɡruːp/ v. 分组；hard-coded /hɑːd ˈkəʊdɪd/ adj. 硬编码的；single /ˈsɪŋɡəl/ adj. 单一的。

**译文**：把渲染片段按镜头顺序放到画布上，分组命名为 `<title> shot clips`，不再硬编码为单一模型名，然后向用户展示选择卡片。

### 12｜选择卡片的选项

**词汇释义**：approve /əˈpruːv/ v. 确认通过；composite /ˈkɒmpəzɪt/ v. 合成；selected /sɪˈlektɪd/ adj. 选定的；mismatch /ˌmɪsˈmætʃ/ n. 不一致；storyboard cleanup /ˈstɔːribɔːd ˈkliːnʌp/ n. phr. 分镜整理修正；spatial anchor /ˈspeɪʃəl ˈæŋkə/ n. phr. 空间锚点。

**译文**：选项依次为：确认片段并合成完整影片（推荐）；重新渲染所选片段（使用同一模型或其他视频模型）；修复人物不一致；修复场景不一致；加强分镜整理修正；修复跨片段的空间锚点漂移。

### 13｜已渲染片段偏离参考时

**词汇释义**：approved /əˈpruːvd/ adj. 已确认的；door-frame /ˈdɔːfreɪm/ n. 门框；edge /edʒ/ n. 画面边缘；flipped /flɪpt/ adj. 翻转的；persist /pəˈsɪst/ v. 持续存在；silently /ˈsaɪləntli/ adv. 未告知地；corrected /kəˈrektɪd/ adj. 已修正的；assembly /əˈsembli/ n. 组接。

**译文**：渲染片段偏离已确认的 `Reference Anchors` 时，例如门框落在错误一侧、人物从错误画边离开、光照方向翻转，应使用原样引用表中 `Reference Anchors` 块的强化提示词重新渲染。漂移仍存在时，通过混合模式将该单个镜头切换至另一视频模型；不得悄悄把已修正与未修正的片段混入组接。

## 三、Storyboard Visualization Fallback：分镜可视化回退

### 14｜适用范围和触发条件

**词汇释义**：visualization /ˌvɪʒuəlaɪˈzeɪʃən/ n. 可视化；pencil storyboard /ˈpensəl ˈstɔːribɔːd/ n. phr. 铅笔分镜；required quality /rɪˈkwaɪəd ˈkwɒləti/ n. phr. 要求的质量；layout /ˈleɪaʊt/ n. 布局；collapse /kəˈlæps/ v. 崩坏；illegible /ɪˈledʒəbəl/ adj. 难以辨认的；merged /mɜːdʒd/ adj. 被合并的；inconsistency /ˌɪnkənˈsɪstənsi/ n. 不一致；escalation /ˌeskəˈleɪʃən/ n. 逐级升级。

**译文**：以下分镜生成失败回退只用于可视化模式。铅笔图像分镜无法达到所需质量时，例如布局崩坏、标签不可读、画格合并或人物不一致，应先按以下步骤逐级处理，再询问用户。

### 15｜第一次重试

**词汇释义**：tightened prompt /ˈtaɪtənd prɒmpt/ n. phr. 约束更明确的提示词；four-quadrant /fɔː ˈkwɒdrənt/ adj. 四象限的；label /ˈleɪbəl/ n. 标签；per-panel /pɜː ˈpænəl/ adj. 每画格的；content rule /ˈkɒntent ruːl/ n. phr. 内容规则。

**译文**：第一次重试：重新生成同一镜头的分镜图，强化提示词，明确提到四象限布局、`[char:…] [scene:…] [shot:…]` 标签及每画格内容规则。

### 16｜第二次重试

**词汇释义**：bottom-right /ˌbɒtəm ˈraɪt/ adj. 右下方的；quadrant /ˈkwɒdrənt/ n. 象限；blank cell /blæŋk sel/ n. phr. 空白单元格；text load /tekst ləʊd/ n. phr. 文字负荷；visual beat /ˈvɪʒuəl biːt/ n. phr. 视觉节拍。

**译文**：第二次重试：去掉右下方音频／锚点象限的文字，保留空格，仅标一个小 `♪`，降低文字负荷。这通常能在不损失视觉节拍的情况下修复标签不可读问题。

### 17｜第三次重试

**词汇释义**：panel count /ˈpænəl kaʊnt/ n. phr. 画格数量；reduce /rɪˈdjuːs/ v. 减少；merge /mɜːdʒ/ v. 合并；actionable /ˈækʃənəbəl/ adj. 有可执行动作内容的；icon /ˈaɪkɒn/ n. 图标；arrow /ˈærəʊ/ n. 箭头。

**译文**：第三次重试：减少一个画格，例如把动作信息最少的两个秒段合并，将 6 格减至 5 格；并把摄影机图标简化为单箭头。

### 18｜同一镜头三次失败之后

**词汇释义**：block-color /blɒk ˈkʌlə/ adj. 色块式的；gray box /ɡreɪ bɒks/ n. phr. 灰色方框；pose /pəʊz/ n. 姿态；rely /rɪˈlaɪ/ v. 依赖；text storyboard /tekst ˈstɔːribɔːd/ n. phr. 文字分镜；split /splɪt/ v. 拆分；reference image /ˈrefərəns ˈɪmɪdʒ/ n. phr. 参考图像。

**译文**：同一镜头三次尝试失败后，暂停并展示选择卡片，让用户选择：仅把失败镜头切换为色块分镜，以灰框表示姿态、不用铅笔线；去掉该镜头的铅笔图，该行只依靠文字分镜文档；在步骤 5 把该镜头拆成两个短镜头，并重新运行步骤 5.5；或手动提供参考图，以绑定替代生成。

### 19｜默认文字模式

**词汇释义**：default /dɪˈfɔːlt/ adj. 默认的；unnecessary /ʌnˈnesəsəri/ adj. 不需要的；coherent /kəʊˈhɪərənt/ adj. 连贯的；structured text /ˈstrʌktʃəd tekst/ n. phr. 结构化文本；revise /rɪˈvaɪz/ v. 修订。

**译文**：默认文字模式不需要整套可视化回退。文字分镜只会在模型无法生成连贯的结构化文本时失败；这种情况下，回到步骤 5 修订对应表格行。
