# Standardized Shot Table Specification｜标准化镜头表规范：逐段注释译本

源文件：[shot-table-spec.md](./shot-table-spec.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`417405085fd3739c105482108f655c3eee2fde75`。本译本不改写源文件，按原顺序先释义再翻译；字段与固定标记保留英文。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语；abbr. 缩写。

## STEP 5｜标准化镜头表视频提示词（六列）

### 01｜创建镜头信息表

**词汇释义**：standardized /ˈstændədaɪzd/ adj. 标准化的；specification /ˌspesɪfɪˈkeɪʃən/ n. 规范；locked /lɒkt/ adj. 已锁定的；mandatory /ˈmændətəri/ adj. 必需的；swap /swɒp/ v. 调换；storyboard /ˈstɔːribɔːd/ n. 分镜；canvas table node /ˈkænvəs ˈteɪbəl nəʊd/ n. phr. 画布表格节点。

**译文**：人物卡与场景卡锁定后，以镜头信息表的形式输出标准化视频提示词。此步骤必须执行，不能与分镜或视频生成互换。创建名为 `标准镜头信息表` 或 `standard-shot-table` 的画布表格节点或 Markdown 表格。

### 02｜固定六列与顺序

**词汇释义**：column /ˈkɒləm/ n. 列；duration /djʊəˈreɪʃən/ n. 时长；continuity handoff /ˌkɒntɪˈnjuːəti ˈhændɒf/ n. phr. 连贯性衔接；reference anchor /ˈrefərəns ˈæŋkə/ n. phr. 参考锚点；spatial /ˈspeɪʃəl/ adj. 空间的；identity /aɪˈdentəti/ n. 身份；hook /hʊk/ n. 吸引注意的叙事抓手；directive /dəˈrektɪv/ n. 指令；track /træk/ n. 音轨。

**译文**：表格必须严格包含以下六列，顺序不可改变：

| Shot ID & Duration | Continuity Handoff | Reference Anchors (Spatial + Identity) | Hook Type | Shot Description (Per-Second Directives) | Audio & Dialogue Track |
|---|---|---|---|---|---|
| 镜头编号与时长 | 连贯性衔接 | 参考锚点（空间＋身份） | 叙事抓手类型 | 镜头描述（逐秒指令） | 音频与对白轨 |

### 03｜镜头编号与时长

**词汇释义**：ID abbr. Identifier，标识符；planned /plænd/ adj. 计划的；shot number /ʃɒt ˈnʌmbə/ n. phr. 镜头编号。

**译文**：`Shot ID & Duration`：镜头编号加计划时长，例如 `S03 / 6s`。

### 04｜连贯性衔接

**词汇释义**：naturally /ˈnætʃərəli/ adv. 自然地；ending image /ˈendɪŋ ˈɪmɪdʒ/ n. phr. 结束画面；prop position /prɒp pəˈzɪʃən/ n. phr. 道具位置；eyeline /ˈaɪlaɪn/ n. 视线方向；posture /ˈpɒstʃə/ n. 姿态；sound bridge /saʊnd brɪdʒ/ n. phr. 声桥；emotional state /ɪˈməʊʃənəl steɪt/ n. phr. 情绪状态；set up /set ʌp/ v. phr. 铺垫；spine /spaɪn/ n. 主干。

**译文**：`Continuity Handoff`：说明本镜头如何自然承接上一镜头的结束画面、道具位置、视线、人物姿态、声桥或情绪状态，并说明它怎样为下一镜头开场作铺垫。这一列是跨镜头连续性的主干。

### 05｜参考锚点的四个必需子字段

**词汇释义**：sub-field /sʌb fiːld/ n. 子字段；fixed landmark /fɪkst ˈlændmɑːk/ n. phr. 固定标志物；screen-relative /skriːn ˈrelətɪv/ adj. 相对画面的；door-frame /ˈdɔːfreɪm/ n. 门框；kitchen island /ˈkɪtʃɪn ˈaɪlənd/ n. phr. 厨房中岛。

**译文**：`Reference Anchors (Spatial + Identity)` 必须包含四个子字段。第一个是 `Fixed Landmarks`：使用场景卡中标志物的准确名称，并记录其相对画面位置，例如 `door-frame: right third`（门框：画面右侧三分之一区域）、`kitchen-island: center bottom`（厨房中岛：中央下方）。

### 06｜人物位置

**词汇释义**：camera view /ˈkæmərə vjuː/ n. phr. 摄影机视角；foreground /ˈfɔːɡraʊnd/ n. 前景；midground /ˈmɪdɡraʊnd/ n. 中景空间；background /ˈbækɡraʊnd/ n. 背景；facing direction /ˈfeɪsɪŋ dəˈrekʃən/ n. phr. 面朝方向；initial pose /ɪˈnɪʃəl pəʊz/ n. phr. 初始姿态。

**译文**：`Character Positions (camera view)`：逐一记录本镜头每名人物相对画面的位置，包括左／中／右、上／中／下、前景／中景／背景，以及面朝方向和初始姿态。

### 07｜离画人物状态

**词汇释义**：exited /ˈeksɪtɪd/ adj. 已离开的；off-screen /ˌɒfˈskriːn/ adj. 画外的；reason /ˈriːzən/ n. 原因；last seen /lɑːst siːn/ phr. 最后出现时；apple basket /ˈæpəl ˈbɑːskɪt/ n. phr. 苹果筐。

**译文**：`Exited Character Status`：上一镜头出现而本镜头未出现的人物，须写明画外位置和原因。例如 `Mia — exited frame-left, last seen holding apple basket at door-frame`，即 Mia 已从画左离开，最后出现时在门框旁提着苹果筐。

### 08｜光照基准

**词汇释义**：lighting baseline /ˈlaɪtɪŋ ˈbeɪslaɪn/ n. phr. 光照基准；inherit /ɪnˈherɪt/ v. 继承；key /kiː/ n. 主光；fill /fɪl/ n. 补光；rim /rɪm/ n. 轮廓光；modifier /ˈmɒdɪfaɪə/ n. 调整项；overhead /ˌəʊvəˈhed/ adj. 顶部的；bounce /baʊns/ n. 反射光；backlit /ˈbæklɪt/ adj. 逆光的；silhouette /ˌsɪluˈet/ n. 剪影。

**译文**：`Lighting Baseline`：继承场景卡中的主光、补光、轮廓光方向，并加入逐镜头调整。例如 `key: warm overhead, fill: cool bounce right, modifier: window-backlit silhouette`，即主光为暖色顶光，补光为右侧冷色反射光，调整项为窗户逆光剪影。

### 09｜身份绑定

**词汇释义**：identity binding /aɪˈdentəti ˈbaɪndɪŋ/ n. phr. 身份绑定；exact /ɪɡˈzækt/ adj. 精确的；approved /əˈpruːvd/ adj. 已确认的。

**译文**：除四个子字段外，还须加入身份绑定：已确认人物卡的准确名称，以及已确认场景卡的准确名称。

### 10｜叙事抓手类型

**词汇释义**：controlled vocabulary /kənˈtrəʊld vəˈkæbjʊləri/ n. phr. 受控词表；visual joke /ˈvɪʒuəl dʒəʊk/ n. phr. 视觉笑料；reversal /rɪˈvɜːsəl/ n. 反转；suspense /səˈspens/ n. 悬念；tender /ˈtendə/ adj. 温情的；chase /tʃeɪs/ n. 追逐；reveal /rɪˈviːl/ n. 揭示；callback /ˈkɔːlbæk/ n. 前文呼应；expression beat /ɪkˈspreʃən biːt/ n. phr. 表情节拍；distribution /ˌdɪstrɪˈbjuːʃən/ n. 分布。

**译文**：`Hook Type`：从受控词表中选一个短标签，例如 `visual-joke`、`reversal`、`suspense`、`tender`、`chase`、`reveal`、`callback`、`expression-beat`。用于逐集检查叙事抓手分布。

### 11｜镜头描述总体内容

**词汇释义**：shot size /ʃɒt saɪz/ n. phr. 景别；Dutch angle /dʌtʃ ˈæŋɡəl/ n. phr. 荷兰角、倾斜构图；performance style /pəˈfɔːməns staɪl/ n. phr. 表演风格；negative prompt /ˈneɡətɪv prɒmpt/ n. phr. 负面提示词；packaging /ˈpækɪdʒɪŋ/ n. 视觉包装；motion graphics /ˈməʊʃən ˈɡræfɪks/ n. phr. 动态图形；elastic /ɪˈlæstɪk/ adj. 弹性的；sub-second /sʌb ˈsekənd/ adj. 不足一秒的；critical beat /ˈkrɪtɪkəl biːt/ n. phr. 关键节拍。

**译文**：`Shot Description`：写明景别、运镜、荷兰角设计、表演风格、音效、负面提示词、视频模型生成说明，以及必需的 `Per-Second Directives` 子节。步骤 7 选择的 H3 或 Seedance 2.0 接收略有区别的提示词：H3 强调视觉包装词和文字／界面／动态图形清晰度，Seedance 2.0 强调电影式运镜和弹性表演。逐秒指令应把镜头拆成 `0–1s`、`1–2s`、`2–3s` 等；不足一秒的关键节拍可用 `2.0–2.5s`。每条逐秒指令必须包含以下五项。

### 12｜逐秒指令五项

**词汇释义**：squash-and-stretch /skwɒʃ ənd stretʃ/ n. phr. 挤压拉伸；anticipation /ænˌtɪsɪˈpeɪʃən/ n. 预备动作；overshoot /ˈəʊvəʃuːt/ n. 过冲；follow-through /ˈfɒləʊ θruː/ n. 随动；push /pʊʃ/ v. 推进；pull /pʊl/ v. 拉离；pan /pæn/ v. 横摇；tilt /tɪlt/ v. 俯仰摇；orbit /ˈɔːbɪt/ v. 环绕；audio cue /ˈɔːdiəʊ kjuː/ n. phr. 声音提示点；handoff /ˈhændɒf/ n. 衔接交接。

**译文**：五项分别是：第一，动作／姿态／表情，适用时包括挤压拉伸、预备动作、过冲与随动；第二，摄影机运动，推进／拉离／横摇／俯仰摇／手持抖动／锁定／环绕；第三，空间位置，即人物在哪、拿着什么、哪个标志物在画面中；第四，声音提示，包括旁白／对白／音效／呼吸／静音，有意无声时标 `silent`；第五，衔接下一秒或下一镜头，说明本秒为下一段锁定了什么状态。

### 13｜独立完整音频脚本

**词汇释义**：full audio script /fʊl ˈɔːdiəʊ skrɪpt/ n. phr. 完整声音脚本；time order /taɪm ˈɔːdə/ n. phr. 时间顺序；narration /nəˈreɪʃən/ n. 旁白；time range /taɪm reɪndʒ/ n. phr. 时间范围；speaker /ˈspiːkə/ n. 发声者；tone /təʊn/ n. 语气；keyed /kiːd/ adj. 按明确提示点设置的；performance note /pəˈfɔːməns nəʊt/ n. phr. 表演说明；protagonist /prəˈtæɡənɪst/ n. 主角。

**译文**：`Audio & Dialogue Track`：按时间顺序写出该镜头完整声音脚本，与逐秒声音提示分开。字段包括 `Narration`（旁白文字与时间范围，无旁白时省略）、`Dialogue`（台词、发声者、语气、时间范围）、`SFX`（具有时间锚点的音效），以及 `Performance Note`。主角作画外旁白时，标 `narrator-mouth-closed: true`，描述旁白期间的表情变化；每句对白都要描述具体视线与身体动作变化。

## 整张表格的规则

### 14｜连续性链

**词汇释义**：inherit /ɪnˈherɪt/ v. 继承；image state /ˈɪmɪdʒ steɪt/ n. phr. 画面状态；set up /set ʌp/ v. phr. 为……作铺垫。

**译文**：每个镜头都须通过 `Continuity Handoff` 列自然承接上一镜头画面状态，并在同一列铺垫下一镜头。

### 15｜首帧到尾帧全覆盖

**词汇释义**：coverage /ˈkʌvərɪdʒ/ n. 覆盖；entire /ɪnˈtaɪə/ adj. 全部的；pose /pəʊz/ n. 姿态；expression /ɪkˈspreʃən/ n. 表情。

**译文**：每个镜头行都要有覆盖首帧至尾帧全部时长的逐秒指令，包含动作、姿态、表情、运镜、空间位置、声音提示和连续性衔接。

### 16｜具体到可以直接生成分镜

**词汇释义**：specific /spəˈsɪfɪk/ adj. 具体的；panel /ˈpænəl/ n. 画格；vague /veɪɡ/ adj. 含糊的；prop detail /prɒp ˈdiːteɪl/ n. phr. 道具细节。

**译文**：逐秒指令要具体到足以直接生成分镜画格。避免只有“继续移动”而没有身体、摄影机或道具细节的含糊时间描述。

### 17｜夸张弹性表演

**词汇释义**：exaggerated /ɪɡˈzædʒəreɪtɪd/ adj. 夸张的；overlap /ˈəʊvəlæp/ n. 重叠动作；arc /ɑːk/ n. 弧线路径；pose change /pəʊz tʃeɪndʒ/ n. phr. 姿态变化；comedic silhouette /kəˈmiːdɪk ˌsɪluˈet/ n. phr. 喜剧性轮廓。

**译文**：表演须夸张而有弹性，符合迪士尼式挤压拉伸、预备动作、过冲、随动、重叠动作、弧线、快速姿态变化和清晰喜剧轮廓。

### 18｜景别节奏与倾斜设计

**词汇释义**：alternate /ˈɔːltəneɪt/ v. 交替；close-up /ˈkləʊsʌp/ n. 特写；extreme close-up /ɪkˈstriːm ˈkləʊsʌp/ n. phr. 大特写；repetitive /rɪˈpetɪtɪv/ adj. 重复的；imbalance /ɪmˈbæləns/ n. 失衡；surprise /səˈpraɪz/ n. 惊讶；slapstick /ˈslæpstɪk/ n. 肢体闹剧。

**译文**：特写／大特写必须与其他必要景别交替，避免重复取景。追逐、失衡、惊讶或肢体喜剧节拍中必须设计荷兰角倾斜构图。

### 19｜对白语言与嘴部状态

**词汇释义**：explicitly requested /ɪkˈsplɪsɪtli rɪˈkwestɪd/ phr. 明确要求的；minimal /ˈmɪnɪməl/ adj. 最少量的；optional /ˈɒpʃənəl/ adj. 可选的；pending confirmation /ˈpendɪŋ ˌkɒnfəˈmeɪʃən/ phr. 等待确认；narrator /nəˈreɪtə/ n. 旁白者；on-screen /ˌɒnˈskriːn/ adj. 画面内的。

**译文**：只有用户明确要求时才指定对白语言；否则采用少量不依赖具体语言的反应声，或把对白标为可选／待确认。含旁白或对白的镜头，每个相关发声秒段必须记录人物嘴部开闭状态；画外旁白默认为闭嘴，画面内对白默认为开口。

### 20｜离画人物追踪

**词汇释义**：track /træk/ v. 追踪；off-stage /ˌɒfˈsteɪdʒ/ adj. 不在当前场面的；consecutive /kənˈsekjʊtɪv/ adj. 连续的；drop /drɒp/ v. 从记录中移除。

**译文**：离开画面的人物，仍须至少在一个后续镜头的 `Exited Character Status` 中追踪；明确连续两个镜头都已离场后，再停止记录。

### 21｜表格确认卡片

**词汇释义**：adjust /əˈdʒʌst/ v. 调整；rhythm /ˈrɪðəm/ n. 节奏；run self-check /rʌn self tʃek/ v. phr. 运行自检。

**译文**：随后展示用户选择卡片：确认表格并运行自检（推荐）；调整镜头衔接；让动画更夸张；调整特写／大特写节奏；调整荷兰角设计。

## STEP 5.5｜镜头表自检关口（必需）

### 22｜未通过则先修表

**词汇释义**：hard self-check /hɑːd self tʃek/ n. phr. 严格自检；revise /rɪˈvaɪz/ v. 修订；re-run /ˌriːˈrʌn/ v. 重跑；approve /əˈpruːv/ v. 确认通过。

**译文**：进入铅笔分镜之前，对已确认镜头表进行严格自检。任何检查失败，都应修订表格并重新检查，再询问用户是否开始分镜。

### 23｜检查一：抓手密度

**词汇释义**：density /ˈdensəti/ n. 密度；consecutive /kənˈsekjʊtɪv/ adj. 连续的；opening /ˈəʊpənɪŋ/ adj. 开场的；closing /ˈkləʊzɪŋ/ adj. 结尾的；strong hook /strɒŋ hʊk/ n. phr. 强叙事抓手。

**译文**：每个镜头都有 `Hook Type`；每三个连续镜头中，至少一个使用 `reveal`／`reversal`／`callback`；开场和结尾镜头各自具有强抓手，即 `visual-joke`、`reversal`、`reveal`、`suspense` 或 `tender`。

### 24｜检查二与三：时长和重要人物数

**词汇释义**：exceed /ɪkˈsiːd/ v. 超过；split /splɪt/ v. 拆分；important character /ɪmˈpɔːtənt ˈkærəktə/ n. phr. 重要人物；defined /dɪˈfaɪnd/ adj. 被定义为的。

**译文**：单镜头不得超过 15 秒；一个节拍需要更长时间时拆分。单镜头不得有超过三名重要人物；“重要人物”指在画面中有动作或对白的人物。

### 25｜检查四：空间锚点继承

**词汇释义**：interior /ɪnˈtɪəriə/ adj. 室内的；inheritance /ɪnˈherɪtəns/ n. 继承；match /mætʃ/ v. 一致；explicit continuity note /ɪkˈsplɪsɪt ˌkɒntɪˈnjuːəti nəʊt/ n. phr. 明确的衔接说明；orbit left /ˈɔːbɪt left/ v. phr. 向左环绕。

**译文**：每个有两个或更多镜头的室内场景，下一镜头的 `Fixed Landmarks` 与 `Lighting Baseline` 必须与上一镜头一致，或包含明确衔接说明。例如，摄影机向左环绕时，门框从画面右侧三分之一区域移到中央。

### 26｜检查五：逐秒指令覆盖

**词汇释义**：entry /ˈentri/ n. 条目；element /ˈelɪmənt/ n. 要素；time gap /taɪm ɡæp/ n. phr. 时间缺口。

**译文**：从 `0s` 到镜头结束的每一秒，都由 `Per-Second Directives` 条目覆盖；每条都有动作／姿态／表情、摄影机、空间、声音提示和衔接五项。可以用 `2.0–2.5s` 等亚秒节拍，但不得留下时间空隙。

### 27｜检查六：跨镜头连续性

**词汇释义**：row by row /rəʊ baɪ rəʊ/ adv. 逐行地；chain /tʃeɪn/ n. 链条；contradict /ˌkɒntrəˈdɪkt/ v. 矛盾；flip /flɪp/ v. 翻转；hard cut /hɑːd kʌt/ n. phr. 硬切；time skip /taɪm skɪp/ n. phr. 时间跳跃。

**译文**：逐行阅读 `Continuity Handoff` 应形成连续链条；不得有镜头从与上一镜头结束状态矛盾的状态开始。翻转视线、人物位置、道具状态或光照时，必须明确标记，例如 `HARD CUT — time skip: 2h`（硬切——时间跳跃两小时）。

### 28｜全部通过后的标记与选择

**词汇释义**：stamp /stæmp/ n. 状态戳记；passed /pɑːst/ adj. 已通过的；detail /ˈdiːteɪl/ n. 细节；failed check /feɪld tʃek/ n. phr. 失败检查项。

**译文**：六项全部通过后，在画布表格节点顶部加上 `shot-table self-check: passed`，再显示用户选择卡片：确认自检并绘制镜头分镜（推荐）；显示自检细节；修订失败项；重新运行自检。

### 29｜未通过不能进入步骤 6

**词汇释义**：enter /ˈentə/ v. 进入；list /lɪst/ v. 列出；re-show /ˌriːˈʃəʊ/ v. 再次展示；fixed /fɪkst/ adj. 已修复的。

**译文**：任何检查失败，都不能进入步骤 6。回到步骤 5，列出失败行；只有表格修复且自检通过后，才重新显示分镜确认卡片。
