# Text and Pencil Storyboard Guidelines｜文字与铅笔分镜指南：逐段注释译本

源文件：[storyboard-guidelines.md](./storyboard-guidelines.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`a8639b854041cfb5fc95cd8e020ad5b4c0ffebc1`。本文件与源文件并列，不覆盖源文件。按原文章节、段落和列表次序先释义再翻译。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语；abbr. 缩写。代码标记、节点名模板和字段标识保留英文；本译文不执行生成指令。

## STEP 6｜文字分镜文档（默认）与铅笔图像分镜（主动选用）

### 01｜先选择模式

**词汇释义**：self-check /self tʃek/ n. 自检；storyboard /ˈstɔːribɔːd/ n. 分镜；opt-in /ˈɒptɪn/ adj. 主动选用的；artifact /ˈɑːtɪfækt/ n. 产物；choice card /tʃɔɪs kɑːd/ n. phr. 选择卡片。

**译文**：步骤 5.5 自检通过后，在制作任何分镜产物前，展示分镜模式选择卡片。

### 02｜仅文字分镜文档：默认推荐

**词汇释义**：in-document section /ɪn ˈdɒkjʊmənt ˈsekʃən/ n. phr. 文档内小节；mirror /ˈmɪrə/ v. 沿用对应结构；half-narrated drama /hɑːf nəˈreɪtɪd ˈdrɑːmə/ n. phr. 半旁白式剧情；spatial anchor /ˈspeɪʃəl ˈæŋkə/ n. phr. 空间锚点；per-panel /pɜː ˈpænəl/ adj. 每画格的；four-quadrant /fɔː ˈkwɒdrənt/ adj. 四象限的；ASCII abbr. American Standard Code for Information Interchange，美国信息交换标准代码，此处指字符示意图；payload /ˈpeɪləʊd/ n. 有效信息载荷；near-zero cost /nɪə ˈzɪərəʊ kɒst/ n. phr. 接近零成本。

**译文**：仅文字分镜文档（默认、推荐）：一个画布文本节点，以文档小节包含全部镜头分镜。沿用半旁白式剧情的分镜结构：逐镜头字段（标题／抓手／场景／人物／空间锚点／连续性／表演），再加皮克斯式逐画格四象限内容和可选字符布局。以接近零成本承载完整质量控制信息。步骤 7 选择的视频模型直接读取它，作为逐镜头渲染参考。

### 03｜文字加多格铅笔图：可视化模式

**词汇释义**：authoritative /ɔːˈθɒrɪtətɪv/ adj. 作为权威依据的；visualization /ˌvɪʒuəlaɪˈzeɪʃən/ n. 可视化；human review /ˈhjuːmən rɪˈvjuː/ n. phr. 人工审阅；commit to /kəˈmɪt tə/ v. phr. 决定投入；squash-and-stretch /skwɒʃ ənd stretʃ/ n. phr. 挤压拉伸；pose silhouette /pəʊz ˌsɪluˈet/ n. phr. 姿态轮廓；pre-check /priː tʃek/ v. 预检查。

**译文**：文字分镜文档加多画格铅笔图（可视化模式，主动选用）：仍制作作为权威依据的文字文档，同时每镜头生成一张多格铅笔图供人工审阅。成本更高，适合用户想在投入视频生成前预览，或挤压拉伸／姿态轮廓是主要风险、希望提前目视检查的情况。

### 04｜保存模式选择

**词汇释义**：store /stɔː/ v. 保存；Project Brief /ˈprɒdʒekt briːf/ n. phr. 项目简报；reuse /ˌriːˈjuːz/ v. 复用；regeneration discipline /ˌriːdʒenəˈreɪʃən ˈdɪsəplɪn/ n. phr. 重新生成规范。

**译文**：将选定分镜模式写入项目简报，并在步骤 7、步骤 9 以及重新生成管理中复用。

## 默认路径：单份文字分镜文档

### 05｜单文档与权威参考

**词汇释义**：rendering reference /ˈrendərɪŋ ˈrefərəns/ n. phr. 渲染参考；cross-shot continuity /krɒs ʃɒt ˌkɒntɪˈnjuːəti/ n. phr. 跨镜头连贯性；node-hopping /nəʊd ˈhɒpɪŋ/ n. 在节点间反复跳转。

**译文**：为整部短片创建一个名为 `<title> text storyboards` 的画布文本节点。即使同时生成铅笔图，这个文档仍是步骤 7 的权威渲染参考。它沿用半旁白式剧情分镜结构，每个镜头是同一文档中的一个小节，因此用户无需在节点间跳转就能阅读跨镜头衔接。

### 06｜文档顶部信息

**词汇释义**：top matter /tɒp ˈmætə/ n. phr. 文首信息；header block /ˈhedə blɒk/ n. phr. 头部内容块；approved /əˈpruːvd/ adj. 已确认的；resolution /ˌrezəˈluːʃən/ n. 分辨率；timestamp /ˈtaɪmstæmp/ n. 时间戳；table of contents /ˈteɪbəl əv ˈkɒntents/ n. phr. 目录；section anchor /ˈsekʃən ˈæŋkə/ n. phr. 小节锚点。

**译文**：文档顶部头部块包括项目标题、已确认视频模型、已确认分辨率、分镜模式和自检状态，例如 `shot-table self-check: passed at <timestamp>`。再提供一个简短目录，列出每个镜头、抓手及小节锚点（`S01`、`S02` 等），便于跳转。

### 07｜逐镜头字段与顺序

**词汇释义**：heading /ˈhedɪŋ/ n. 标题；adaptation /ˌædæpˈteɪʃən/ n. 改编、适配；mandatory /ˈmændətəri/ adj. 必需的；human-readable /ˈhjuːmən ˈriːdəbəl/ adj. 易于人阅读的；duration /djʊəˈreɪʃən/ n. 时长。

**译文**：每镜头以一个 `##` 标题起节，按镜头顺序排列。各节必须按以下顺序包含字段，这是对半旁白式剧情分镜结构的直接适配。首先是 `Shot title & duration`：简短易读的镜头标题，加 `S<N> / <duration>s`，例如 `S03 / 6s`。

### 08｜抓手类型

**词汇释义**：controlled vocabulary /kənˈtrəʊld vəˈkæbjʊləri/ n. phr. 受控词表；setup /ˈsetʌp/ n. 铺垫；visual joke /ˈvɪʒuəl dʒəʊk/ n. phr. 视觉笑料；reversal /rɪˈvɜːsəl/ n. 反转；reveal /rɪˈviːl/ n. 揭示；callback /ˈkɔːlbæk/ n. 呼应；suspense /səˈspens/ n. 悬念；tender /ˈtendə/ adj. 温情的；chase /tʃeɪs/ n. 追逐；expression beat /ɪkˈspreʃən biːt/ n. phr. 表情节拍；climax /ˈklaɪmæks/ n. 高潮。

**译文**：`Hook type`：从受控词表 `setup`／`visual-joke`／`reversal`／`reveal`／`callback`／`suspense`／`tender`／`chase`／`expression-beat`／`climax` 选择一项，用于逐集抓手分布自检。

### 09｜场景与人物

**词汇释义**：exact /ɪɡˈzækt/ adj. 精确的；on-screen /ˌɒnˈskriːn/ adj. 画面内的；bind /baɪnd/ v. 绑定；character card /ˈkærəktə kɑːd/ n. phr. 人物卡。

**译文**：`Scene & characters`：准确场景卡名称，以及画面内人物的准确名称，并绑定相应人物卡。

### 10｜空间锚点卡：固定标志物

**词汇释义**：fixed landmark /fɪkst ˈlændmɑːk/ n. phr. 固定标志物；screen-relative position /skriːn ˈrelətɪv pəˈzɪʃən/ n. phr. 相对画面的位置；door-frame /ˈdɔːfreɪm/ n. 门框；kitchen island /ˈkɪtʃɪn ˈaɪlənd/ n. phr. 厨房中岛。

**译文**：`Spatial anchor card` 必须有四个子字段，直接沿用半旁白式结构。`Fixed landmarks` 记录标志物名称和相对画面位置，例如门框在右侧三分之一区域，厨房中岛在中央下方。

### 11｜空间锚点卡：人物、离场与光照

**词汇释义**：facing direction /ˈfeɪsɪŋ dəˈrekʃən/ n. phr. 面朝方向；initial pose /ɪˈnɪʃəl pəʊz/ n. phr. 初始姿态；exited /ˈeksɪtɪd/ adj. 已离画的；off-screen /ˌɒfˈskriːn/ adj. 画外的；lighting baseline /ˈlaɪtɪŋ ˈbeɪslaɪn/ n. phr. 光照基准；key/fill/rim /kiː fɪl rɪm/ n. 主光／补光／轮廓光；modifier /ˈmɒdɪfaɪə/ n. 调整项。

**译文**：`Character positions (camera view)` 逐一记录画内人物相对画面的位置、朝向、初始姿态；`Exited character status` 记录上一镜头在画内、本镜头不在的人物及其画外位置和原因；`Lighting baseline` 继承场景卡的主光／补光／轮廓光方向，加上逐镜头调整。

### 12｜前后镜头衔接

**词汇释义**：handoff /ˈhændɒf/ n. 衔接；ending state /ˈendɪŋ steɪt/ n. phr. 结束状态；set up /set ʌp/ v. phr. 铺垫。

**译文**：`Continuity` 沿用衔接字段：`Continuity from S(N-1)` 用一至两句引用上一镜头结束状态；`Continuity to S(N+1)` 用一句铺垫下一镜头开场。

### 13｜双重绑定标签

**词汇释义**：double-binding /ˈdʌbəl ˈbaɪndɪŋ/ n. 双重绑定；marker /ˈmɑːkə/ n. 标记；strip /strɪp/ v. 移除；render time /ˈrendə taɪm/ n. phr. 渲染阶段。

**译文**：`Double-binding` 使用 `[char:角色名-01] [char:角色名-02] ... [scene:场景名] [hook: visual-joke]`，记录准确人物卡名、场景卡名和抓手类型。这些只用于分镜参考，视频模型在渲染阶段移除它们。

### 14｜逐画格四象限内容

**词汇释义**：verbatim /vɜːˈbeɪtɪm/ adv. 原样地；timecode /ˈtaɪmkəʊd/ n. 时间码；body posture /ˈbɒdi ˈpɒstʃə/ n. phr. 身体姿态；prop grip /prɒp ɡrɪp/ n. phr. 道具握持；eyeline /ˈaɪlaɪn/ n. 视线；expression path /ɪkˈspreʃən pɑːθ/ n. phr. 表情变化路径；anticipation /ænˌtɪsɪˈpeɪʃən/ n. 预备动作；overshoot /ˈəʊvəʃuːt/ n. 过冲。

**译文**：`Per-panel four-quadrant content` 按时间顺序每格一个内容块，原样保留表格行中的皮克斯式逐秒指令。`Timecode` 例如 `0–1s`。`Pose + Expression` 写具体身体姿态、轮廓、关键道具握持、视线和面部表情路径；弹性动作明确写出挤压／拉伸／预备动作／过冲。这是每格最大部分，也是视频模型读取的视觉节拍。

### 15｜摄影机、声音与表演

**词汇释义**：shot size /ʃɒt saɪz/ n. phr. 景别；push/pull/pan/tilt /pʊʃ pʊl pæn tɪlt/ v. 推进／拉离／横摇／俯仰摇；handheld shake /ˈhændheld ʃeɪk/ n. phr. 手持抖动；locked /lɒkt/ adj. 固定的；orbit /ˈɔːbɪt/ v. 环绕；Dutch angle /dʌtʃ ˈæŋɡəl/ n. phr. 倾斜机位；audio cue /ˈɔːdiəʊ kjuː/ n. phr. 声音提示；narration /nəˈreɪʃən/ n. 旁白。

**译文**：`Camera` 记录景别、运镜（推进／拉离／横摇／俯仰摇／手持抖动／固定／环绕），适用时注明荷兰角。`Audio + Anchor` 记录声音提示（`♪ narration: ...`／`dialogue: ...`／`SFX: ...`／`silent`）和空间锚点，例如门框在右侧三分之一区域，Mia 位于中景中央、面朝摄影机。表演说明沿用半旁白式规则：旁白秒段标 `narrator-mouth-closed: true`；画内对白标 `mouth-open: speaker`，描述表情路径、视线和身体动作变化。

### 16｜画格数量与覆盖

**词汇释义**：layout rule /ˈleɪaʊt ruːl/ n. phr. 布局规则；sub-second /sʌb ˈsekənd/ adj. 亚秒级的；mini-panel /ˈmɪni ˈpænəl/ n. 小画格；time gap /taɪm ɡæp/ n. phr. 时间缺口。

**译文**：每镜头布局规则：3 秒镜头 3 格、4 秒 4 格、5 秒 5 格、6 秒 6 格；7 秒以上每秒一格。不足一秒的关键节拍，只有它构成该镜头抓手时，才加例如 `2.0–2.5s` 的小画格。所有格必须无时间缺口地覆盖首帧至尾帧完整时长。

### 17｜每格绑定

**词汇释义**：appearance /əˈpɪərəns/ n. 外观；hairstyle /ˈheəstaɪl/ n. 发型；proportion /prəˈpɔːʃən/ n. 比例；costume /ˈkɒstjuːm/ n. 服装；signature prop /ˈsɪɡnətʃə prɒp/ n. phr. 标志性道具；movement path /ˈmuːvmənt pɑːθ/ n. phr. 运动路径；spatial logic /ˈspeɪʃəl ˈlɒdʒɪk/ n. phr. 空间逻辑。

**译文**：每个画格绑定该表格行列出的准确人物卡，锁定外观、面孔、发型、身体比例、服装、标志性道具与角色身份，人物名称与表格一致。绑定该行准确场景卡，以保留环境、道具、标志物、运动路径和空间逻辑。

### 18｜可选字符布局块

**词汇释义**：append /əˈpend/ v. 附加；combined sketch /kəmˈbaɪnd sketʃ/ n. phr. 合并示意图；scan /skæn/ v. 快速浏览；informational /ˌɪnfəˈmeɪʃənəl/ adj. 提供信息的；kneel /niːl/ v. 跪下；low push-in /ləʊ ˈpʊʃɪn/ n. phr. 低位推进。

**译文**：可选 ASCII 布局块（强烈推荐，不增加图像生成费用）：每格附一个小字符示意，或为整镜头附一个合并示意，让用户几秒钟内看清空间布局，无需渲染图像。原示例的含义为：`0–1s` 时 Mia 在左侧中景，门框在右侧；她跪下，手放在苹果筐上；摄影机低位推进、锁定；声音为静音，筐的锚点在中央下方；`1–2s` 继续。字符块只供阅读，视频模型读取上方结构化四象限内容，不读取 ASCII。

### 19｜分镜专用标记

**词汇释义**：critical /ˈkrɪtɪkəl/ adj. 关键的；append /əˈpend/ v. 追加；specific state /spəˈsɪfɪk steɪt/ n. phr. 特定状态；opening /ˈəʊpənɪŋ/ n. 开场。

**译文**：关键节拍在画格时间码后加 `[BEAT]`。某格必须把特定状态交给下一格或下一镜头时，加 `[HANDOFF → ...]` 和简短标签，例如 `[HANDOFF → S04 opening]`。

### 20｜每镜头模板：字段、故事内容与固定标签

**词汇释义**：copy-paste skeleton /ˈkɒpi peɪst ˈskelɪtən/ n. phr. 可复制粘贴的骨架模板；midground /ˈmɪdɡraʊnd/ n. 中景空间；foreground /ˈfɔːɡraʊnd/ n. 前景；warm overhead key /wɔːm ˌəʊvəˈhed kiː/ n. phr. 暖色顶主光；cool bounce right /kuːl baʊns raɪt/ n. phr. 右侧冷色反射光；eye-level /ˈaɪlevəl/ adj. 平视的；rustle /ˈrʌsəl/ n. 窸窣声；lift /lɪft/ v. 提起。

**译文**：原文提供适用于任意镜头的可复制模板。下面保留字段标识、标签、时间码和原有中文故事内容，将人类可读英文值译为中文。省略号本来就在源模板中，不代表遗漏源文已有内容。

```markdown
## S03 / 6s — Title: 奶奶把苹果筐递给 Mia

- **Hook type**: reveal
- **Scene & characters**: scene:kitchen | char:Mia, char:Grandma
- **Spatial anchor card**:
  - Fixed landmarks: door-frame（右侧三分之一区域）, kitchen-island（中央下方）
  - Character positions: Mia（左侧中景，面朝摄影机）| Grandma（右侧前景，面朝 Mia）
  - Exited character status: —
  - Lighting baseline: 暖色顶主光＋右侧冷色反射光
- **Continuity from S02**: 奶奶弯下腰从中岛拿起苹果筐
- **Continuity to S04**: Mia 接住筐转身，门铃响起
- **Double-binding**: [char:Mia] [char:Grandma] [scene:kitchen] [hook:reveal]

### Per-panel four-quadrant content

#### 0–1s
- Pose + Expression: 奶奶弯腰双手持筐；Mia 左侧站姿，眼神好奇
- Camera: 固定中景，平视
- Audio + Anchor: silent | Mia: 左侧中景 | basket: 中央下方
- Performance: [BEAT]

#### 1–2s
- Pose + Expression: 奶奶手臂伸向 Mia，筐倾斜；Mia 双手前伸准备接
- Camera: 固定中景，平视
- Audio + Anchor: ♪ SFX: 筐的窸窣声 | anchor: door-frame: 右侧三分之一区域
- Performance: [HANDOFF → S04 opening]

#### 2–3s
...

### ASCII layout (optional)
[0-1s]  Grandma（右侧前景）        door-frame（右侧背景）
        ──提起筐──                Mia（左侧中景）
        cam: locked | silent
[1-2s]  ...
```

### 21｜默认模式不调用图像模型

**词汇释义**：directly /dəˈrektli/ adv. 直接地；image generation /ˈɪmɪdʒ ˌdʒenəˈreɪʃən/ n. phr. 图像生成；default /dɪˈfɔːlt/ adj. 默认的。

**译文**：所有小节写完后，把文档放到画布，直接进入步骤 7。默认模式不调用任何图像生成模型。

## 镜头级提取：密集迭代模式

### 22｜何时提取独立节点

**词汇释义**：optimize /ˈɒptɪmaɪz/ v. 优化；flag /flæɡ/ v. 标出；heavy iteration /ˈhevi ˌɪtəˈreɪʃən/ n. phr. 密集迭代；slapstick /ˈslæpstɪk/ n. 肢体闹剧；revision /rɪˈvɪʒən/ n. 修订；extract /ɪkˈstrækt/ v. 提取；localize /ˈləʊkəlaɪz/ v. 局部化。

**译文**：默认单文档形式针对阅读和跨镜头连贯性优化。用户把特定镜头标为需要密集迭代时，通常是逐格内容要改很多轮的高潮／追逐／肢体喜剧镜头，将该节提取为独立文本节点，使迭代局部化。

### 23｜用户信号

**词汇释义**：signal /ˈsɪɡnəl/ n. 信号；focus on /ˈfəʊkəs ɒn/ v. phr. 专注于；rework /ˌriːˈwɜːk/ n./v. 重做；select /sɪˈlekt/ v. 选择。

**译文**：步骤 6 之后任意时刻，用户说“让我专门看 S05”“S05 需要重做”“提取 S05”等，或在分镜确认卡中选定某镜头，都可作为提取信号。

### 24｜提取机制

**词汇释义**：mechanics /mɪˈkænɪks/ n. 具体机制；move /muːv/ v. 移动；placeholder /ˈpleɪshəʊldə/ n. 占位符；standalone /ˈstændəˌləʊn/ adj. 独立的。

**译文**：第一，创建 `<title> S05 text storyboard (extracted)` 画布文本节点。第二，把文档中 `## S05` 小节的全部内容移入新节点。第三，原文档的该节替换为一行占位提示，说明 S05 已提取到独立节点，并指向上述节点名。第四，步骤 7 对 S05 读取提取节点，其他镜头仍读取主文档。

### 25｜重新整合和多镜头提取

**词汇释义**：re-integration /ˌriːɪntɪˈɡreɪʃən/ n. 重新整合；fold back /fəʊld bæk/ v. phr. 合并回去；archive /ˈɑːkaɪv/ v. 归档；track /træk/ v. 跟踪；iteration pressure /ˌɪtəˈreɪʃən ˈpreʃə/ n. phr. 迭代压力。

**译文**：用户满意后，将独立节点重新并回文档，用最新内容替换占位提示，并归档独立节点。提取多个镜头时，每镜头单独一个节点，主文档用占位提示跟踪。该机制存在，是因为独立节点应按需要使用，而非默认遍布所有镜头；但任何镜头迭代压力较高时，都可以启用。

## 主动选用路径：多格铅笔图像分镜

### 26｜文字文档仍是权威依据

**词汇释义**：on top of /ɒn tɒp əv/ phr. 在……之外另加；per table row /pɜː ˈteɪbəl rəʊ/ phr. 每表格行；human-review-only /ˈhjuːmən rɪˈvjuː ˈəʊnli/ adj. 仅供人工审阅的。

**译文**：用户在分镜模式卡中选了可视化时，除文字分镜文档外，再为每个表格行生成一张多格铅笔分镜图。文字文档继续作为权威渲染参考，铅笔图仅用于人工审阅。

### 27｜图上必需的双重绑定标签

**词汇释义**：top-right corner /tɒp raɪt ˈkɔːnə/ n. phr. 右上角；mandatory /ˈmændətəri/ adj. 必需的；duration /djʊəˈreɪʃən/ n. 时长；strip /strɪp/ v. 去除。

**译文**：每张铅笔分镜图右上角必须标记：`[char:角色名-01] [char:角色名-02] ...`，即该行准确人物卡名；`[scene:场景名]`，即准确场景卡名；`[shot: S03] [dur: 6s] [hook: visual-joke]`，即镜头编号、时长和抓手。这些只用于分镜参考，视频渲染时必须移除。

### 28｜绑定人物与场景

**词汇释义**：signature prop /ˈsɪɡnətʃə prɒp/ n. phr. 标志性道具；role identity /rəʊl aɪˈdentəti/ n. phr. 角色身份；preserve /prɪˈzɜːv/ v. 保留；landmark /ˈlændmɑːk/ n. 标志物。

**译文**：绑定该行准确人物卡，以锁定外观、面孔、发型、身体比例、服装、标志性道具与角色身份；绑定准确场景卡，以保留环境、道具、标志物、运动路径与空间逻辑。

### 29｜逐秒指令变为画格

**词汇释义**：convert /kənˈvɜːt/ v. 转换；clearly labeled /ˈklɪəli ˈleɪbəld/ adj. 明确标记的；beat panel /biːt ˈpænəl/ n. phr. 节拍画格；extra /ˈekstrə/ adj. 额外的。

**译文**：该行每条逐秒指令转换成一个分镜画格，或一个清楚标记的节拍画格。4 秒镜头通常 4 格，6 秒通常 6 格；仅在确有需要时为亚秒关键节拍添加额外小格。

### 30｜画格物理布局

**词汇释义**：strip /strɪp/ n. 条带；grid /ɡrɪd/ n. 网格；balanced /ˈbælənst/ adj. 均衡的；occupy /ˈɒkjʊpaɪ/ v. 占据；dominate /ˈdɒmɪneɪt/ v. 占主导。

**译文**：必需布局：3 秒用 1×3 条带；4 秒用 2×2 网格；5 秒上排 3 格、下排 2 格；6 秒用 2×3 网格；7 秒以上用三排，画格均衡分配。每格占同样画布面积，不能让某格过大。

### 31｜每格四象限

**词汇释义**：timecode /ˈtaɪmkəʊd/ n. 时间码；sketch /sketʃ/ n. 草图；movement arrow /ˈmuːvmənt ˈærəʊ/ n. phr. 运动箭头；door creak /dɔː kriːk/ n. phr. 门吱嘎声；anchor note /ˈæŋkə nəʊt/ n. phr. 锚点注记。

**译文**：左上写时间码，如 `0–1s`；右上放姿态与表情草图，是最大区域和实际视觉节拍；左下放摄影机图标与运动箭头（推进／拉离／横摇／环绕／固定），有荷兰角时写简注；右下写声音提示，例如 `♪ narration: "I knew it."`（旁白：“我就知道。”）、`SFX: door creak`（门吱嘎声）、`silent`，以及锚点说明，例如门框在画面右侧三分之一区域。

### 32｜读取顺序和完整内容

**词汇释义**：reading order /ˈriːdɪŋ ˈɔːdə/ n. phr. 阅读顺序；merge /mɜːdʒ/ v. 合并；corresponding /ˌkɒrɪˈspɒndɪŋ/ adj. 对应的；continuity handoff /ˌkɒntɪˈnjuːəti ˈhændɒf/ n. phr. 连贯性衔接。

**译文**：同一单镜头分镜图内，各格按阅读顺序排列；不同镜头不可合成一张图。每格注明 `0–1s`、`1–2s` 等时间码，并展示对应姿态、表情、动作、运镜、道具位置、音效提示和连续性衔接。

### 33｜铅笔图的视觉边界

**词汇释义**：black-and-white /blæk ənd waɪt/ adj. 黑白的；pencil line-art /ˈpensəl laɪn ɑːt/ n. phr. 铅笔线稿；final-render lighting /ˈfaɪnəl ˈrendə ˈlaɪtɪŋ/ n. phr. 成片渲染光照；polished /ˈpɒlɪʃt/ adj. 精修的；construction line /kənˈstrʌkʃən laɪn/ n. phr. 构造辅助线；camera-path icon /ˈkæmərə pɑːθ ˈaɪkɒn/ n. phr. 摄影机路径图标；final art /ˈfaɪnəl ɑːt/ n. phr. 最终美术成品。

**译文**：只输出纯黑白铅笔线稿，不加颜色、成片光照或精修三维渲染。图上标镜头编号，必要时每格加运镜图标。需要时可加入分镜专用铅笔构造线、动作箭头、摄影机路径图标、时间标记和小注。草稿只作为视频渲染参考素材，不是最终美术成品。

## 两种模式共用的分镜确认

### 34｜放置与分组

**词汇释义**：group /ɡruːp/ v. 分组；separately /ˈsepərətli/ adv. 分开地；shot order /ʃɒt ˈɔːdə/ n. phr. 镜头顺序。

**译文**：全部文字分镜小节以及可视化模式下的铅笔图生成后，按镜头顺序放到画布。默认单文档模式分组为 `<title> text storyboards`；可视化模式使用 `<title> text storyboards + multi-panel pencil storyboards`。文字文档和铅笔图要分别分组；源文解释为铅笔图包含双重绑定标签、ASCII 标签及镜头编号，而文字文档没有这些内容。

**译注**：源文前面的文字文档模板实际上也含双重绑定标签、镜头编号和可选字符图。此处按原句翻译，不将这一内部不一致暗中改写为新规则。

### 35｜分镜确认选项

**词汇释义**：approve /əˈpruːv/ v. 确认；re-integrate /ˌriːˈɪntɪɡreɪt/ v. 重新整合；redraw /ˌriːˈdrɔː/ v. 重绘；consistency /kənˈsɪstənsi/ n. 一致性；marker /ˈmɑːkə/ n. 标记。

**译文**：展示选择卡片：确认分镜并渲染镜头视频（推荐）；提取／重新整合一个镜头，在文档与独立节点之间移动；重绘选定铅笔分镜（可视化模式）；修复人物一致性；修复场景逻辑；修复摄影机标记；修复声音／锚点标记。

## 分镜生成失败回退：仅可视化模式

### 36｜触发条件

**词汇释义**：fallback /ˈfɔːlbæk/ n. 回退；layout collapse /ˈleɪaʊt kəˈlæps/ n. phr. 布局崩坏；illegible /ɪˈledʒəbəl/ adj. 不可辨认的；merged panel /mɜːdʒd ˈpænəl/ n. phr. 被合并的画格；escalation /ˌeskəˈleɪʃən/ n. 逐级处理。

**译文**：铅笔图像分镜达不到质量要求，例如布局崩坏、标签不可读、画格合并或人物不一致时，在询问用户之前，先按以下阶梯处理。

### 37｜第一次重试

**词汇释义**：tightened prompt /ˈtaɪtənd prɒmpt/ n. phr. 约束强化的提示词；explicitly /ɪkˈsplɪsɪtli/ adv. 明确地；per-panel content /pɜː ˈpænəl ˈkɒntent/ n. phr. 每画格内容。

**译文**：重新生成同一镜头分镜，在强化提示词中明确说明四象限布局、`[char:…] [scene:…] [shot:…]` 标签，以及每格内容规则。

### 38｜第二次重试

**词汇释义**：drop /drɒp/ v. 去掉；blank cell /blæŋk sel/ n. phr. 空白单元格；text load /tekst ləʊd/ n. phr. 文字负荷；visual beat /ˈvɪʒuəl biːt/ n. phr. 视觉节拍。

**译文**：移除右下音频／锚点象限文字，只留空格及小 `♪`，减少文字负荷。源文称这通常能修复标签不可读，而不丢失视觉节拍。

### 39｜第三次重试

**词汇释义**：reduce /rɪˈdjuːs/ v. 减少；least-actionable /liːst ˈækʃənəbəl/ adj. 可执行动作内容最少的；simplify /ˈsɪmplɪfaɪ/ v. 简化；single arrow /ˈsɪŋɡəl ˈærəʊ/ n. phr. 单箭头。

**译文**：减少一格，例如合并动作信息最少的两个秒段，把 6 格改为 5 格；摄影机图标简化为单箭头。

### 40｜三次失败之后的选择

**词汇释义**：block-color /blɒk ˈkʌlə/ adj. 色块式的；gray box /ɡreɪ bɒks/ n. phr. 灰框；rely on /rɪˈlaɪ ɒn/ v. phr. 依靠；split /splɪt/ v. 拆分；manually supply /ˈmænjuəli səˈplaɪ/ v. phr. 手动提供。

**译文**：同一镜头三次尝试失败后暂停，用选择卡片询问：仅该镜头改为色块分镜，以灰框表示姿态，不用铅笔线；去掉失败镜头的铅笔图，该行只依赖文字分镜；在步骤 5 拆成两个更短镜头并重跑步骤 5.5；或由用户手动提供参考图，绑定而非生成。

### 41｜默认文字模式的失败处理

**词汇释义**：unnecessary /ʌnˈnesəsəri/ adj. 不必要的；coherent /kəʊˈhɪərənt/ adj. 连贯的；structured text /ˈstrʌktʃəd tekst/ n. phr. 结构化文本；revise /rɪˈvaɪz/ v. 修订。

**译文**：默认文字模式不需要这整套回退。只有模型不能产生连贯结构化文本时，文字分镜才会失败；此时返回步骤 5 修订表格行。
