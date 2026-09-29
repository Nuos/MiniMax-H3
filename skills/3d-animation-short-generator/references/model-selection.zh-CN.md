# Video Model Selection and Prompt Shaping｜视频模型选择与提示词组织：逐段注释译本

源文件：[model-selection.md](./model-selection.md)；源版本：`d21241f0a4b3acbb34c97dae47fa417b7065e438`；源 Git blob：`48730351c215e0e591ce9f2ae68838fcbf52eb94`。本译本不覆盖源文件。文中模型优劣、价格比例、分辨率与时长均为固定源版本的表述，未在本次翻译中作当前产品核验；不可当作现行报价。n. 名词；v. 动词；adj. 形容词；adv. 副词；phr. 短语；abbr. 缩写。

## STEP 7｜视频模型选择卡片与单镜头视频片段

### 01｜生成前的必需选择

**词汇释义**：selection /sɪˈlekʃən/ n. 选择；shaping /ˈʃeɪpɪŋ/ n. 组织成形；choice card /tʃɔɪs kɑːd/ n. phr. 选择卡片；mandatory /ˈmændətəri/ adj. 必需的；clip /klɪp/ n. 片段；render /ˈrendə/ v. 渲染；Project Brief /ˈprɒdʒekt briːf/ n. phr. 项目简报；reuse /ˌriːˈjuːz/ v. 复用。

**译文**：渲染任何片段之前，必须展示视频模型选择卡片。把选择存入项目简报；除非用户之后更改，否则该项目每个片段都复用这一选择。

### 02｜H3：推荐默认选项

**词汇释义**：visual packaging /ˈvɪʒuəl ˈpækɪdʒɪŋ/ n. phr. 视觉包装；motion graphics /ˈməʊʃən ˈɡræfɪks/ n. phr. 动态图形；clarity /ˈklærəti/ n. 清晰度；UI abbr. User Interface，用户界面；cost efficiency /kɒst ɪˈfɪʃənsi/ n. phr. 成本效率；comparable /ˈkɒmpərəbəl/ adj. 可比的；flagship /ˈflæɡʃɪp/ adj. 旗舰级的；dual-channel /ˈdjuːəl ˈtʃænəl/ adj. 双声道的；stylized /ˈstaɪlaɪzd/ adj. 风格化的；overlay /ˈəʊvəleɪ/ n. 叠加层；dialogue-driven /ˈdaɪəlɒɡ ˈdrɪvən/ adj. 对白驱动的；deliverable /dɪˈlɪvərəbəl/ n. 交付物。

**译文**：H3（推荐默认模型）：擅长视觉包装、动态图形、文字／界面清晰度、多模态上下文理解和成本效率；源文称，其 2K 价格约为可比旗舰模型的三分之一，768P 约为二分之一。原生双声道音频；每段最长 15 秒，分辨率 2K。最适合具有鲜明设计语言、叠加文字、动态图形段落、包装式转场的风格化三维动画短片，以及把音频作为交付组成部分的对白驱动情节节拍。

### 03｜Seedance 2.0：对动画表演要求较高时的回退

**词汇释义**：high-stakes /ˌhaɪˈsteɪks/ adj. 成败影响较大的；performance /pəˈfɔːməns/ n. 动画表演；cinematic /ˌsɪnəˈmætɪk/ adj. 电影式的；elastic /ɪˈlæstɪk/ adj. 富有弹性的；tension-driven /ˈtenʃən ˈdrɪvən/ adj. 由紧张感驱动的；chase sequence /tʃeɪs ˈsiːkwəns/ n. phr. 追逐段落；slapstick /ˈslæpstɪk/ n. 肢体闹剧；climax /ˈklaɪmæks/ n. 高潮；selling point /ˈselɪŋ pɔɪnt/ n. phr. 卖点。

**译文**：Seedance 2.0（关键动画表演的回退模型）：擅长电影式运镜、复杂镜头、富有弹性的皮克斯式表演，以及紧张感驱动的动作。最适合追逐段落、肢体喜剧节拍和高潮镜头，尤其当卖点是动画表演本身而非视觉包装时。

### 04｜逐镜头混合：高级选项

**词汇释义**：per-shot /pɜː ʃɒt/ adj. 逐镜头的；mixed /mɪkst/ adj. 混合的；advanced /ədˈvɑːnst/ adj. 高级的；mark /mɑːk/ v. 标注；column /ˈkɒləm/ n. 列；packaging-heavy /ˈpækɪdʒɪŋ ˈhevi/ adj. 包装比重大的；performance-heavy /pəˈfɔːməns ˈhevi/ adj. 表演比重大的；unmarked /ʌnˈmɑːkt/ adj. 未标注的。

**译文**：逐镜头混合（高级）：允许用户在独立表格行的 `Shot Description` 列标记 `video_model: H3` 或 `video_model: Seedance2`。项目同时存在重包装镜头和重表演镜头时采用此模式。未标记的行默认使用 H3。

## 分辨率选择卡片：在模型选择之后

### 05｜模型锁定后的选项

**词汇释义**：resolution /ˌrezəˈluːʃən/ n. 分辨率；locked /lɒkt/ adj. 已锁定的；first pass /fɜːst pɑːs/ n. phr. 首轮生成；cost-efficient /kɒst ɪˈfɪʃənt/ adj. 成本高效的；sharper /ˈʃɑːpə/ adj. 更清晰锐利的；draft /drɑːft/ n. 草稿；custom /ˈkʌstəm/ adj. 自定义的。

**译文**：视频模型锁定后，展示分辨率选择卡片：768P（推荐用于 H3 首轮，成本较低）；2K（H3 默认质量，成本更高，最终画面更清晰）；1080p（推荐用于 Seedance 2.0）；720p（Seedance 2.0 草稿，成本最低）；或匹配项目／自定义分辨率。

### 06｜确认与逐片调整

**词汇释义**：confirm /kənˈfɜːm/ v. 确认；hero shot /ˈhɪərəʊ ʃɒt/ n. phr. 重点展示镜头；detail /ˈdiːteɪl/ n. 细节。

**译文**：首个片段渲染前，用户必须确认分辨率。之后用户需要某个重点镜头具备更多细节时，可以逐片段更改分辨率。

## 单镜头片段渲染

### 07｜每一表格行的输入

**词汇释义**：approved /əˈpruːvd/ adj. 已确认的；corresponding /ˌkɒrɪˈspɒndɪŋ/ adj. 对应的；independent /ˌɪndɪˈpendənt/ adj. 独立的；matching /ˈmætʃɪŋ/ adj. 匹配的；extracted /ɪkˈstræktɪd/ adj. 已提取的；standalone node /ˈstændəˌləʊn nəʊd/ n. phr. 独立节点；in-document /ɪn ˈdɒkjʊmənt/ adj. 文档内的。

**译文**：对每个已确认表格行，调用选定视频模型，生成相应的独立片段。每段必须精确使用该行所对应的文字分镜内容、人物卡和场景卡；分镜小节已提取时使用独立节点，否则使用文档中的对应小节。

### 08｜文字分镜是镜头权威参考

**词汇释义**：authoritative /ɔːˈθɒrɪtətɪv/ adj. 作为权威依据的；narrative /ˈnærətɪv/ n. 叙事；composition /ˌkɒmpəˈzɪʃən/ n. 构图；staging /ˈsteɪdʒɪŋ/ n. 动作调度；per-second /pɜː ˈsekənd/ adj. 逐秒的；silhouette /ˌsɪluˈet/ n. 轮廓剪影；pre-check /priː tʃek/ n. 预检查；override /ˌəʊvəˈraɪd/ v. 覆盖、取代。

**译文**：所有视频模型共用的逐镜头规则：以文字分镜文档作为叙事、构图、运镜、动作调度、逐秒时序及镜头编号的权威参考。已提取为独立节点的镜头改读独立节点。另有铅笔分镜图时，仅用于人工预检姿态／轮廓，不允许它取代文字分镜。

### 09｜身份与环境依据

**词汇释义**：character card /ˈkærəktə kɑːd/ n. phr. 人物卡；identity source /aɪˈdentəti sɔːs/ n. phr. 身份来源；scene card /siːn kɑːd/ n. phr. 场景卡；environment /ɪnˈvaɪrənmənt/ n. 环境。

**译文**：人物卡是人物身份的权威来源；场景卡是环境的权威来源。

### 10｜移除分镜标记

**词汇释义**：strip /strɪp/ v. 去除；double-binding label /ˈdʌbəl ˈbaɪndɪŋ ˈleɪbəl/ n. phr. 双重绑定标签；reference marker /ˈrefərəns ˈmɑːkə/ n. phr. 参考标记；additionally /əˈdɪʃənəli/ adv. 另外；icon /ˈaɪkɒn/ n. 图标；arrow /ˈærəʊ/ n. 箭头；note /nəʊt/ n. 注记。

**译文**：视频渲染前移除全部分镜双重绑定标签：`[char:…]`、`[scene:…]`、`[shot:…]`、`[dur:…]`、`[hook:…]`。它们只是分镜参考标记，绝不能出现在最终片段。铅笔图像分镜中的镜头编号、摄影机图标、箭头和注记也必须在渲染时移除。

### 11｜最终画面与禁用元素

**词汇释义**：full-color /fʊl ˈkʌlə/ adj. 全彩的；inspired /ɪnˈspaɪəd/ adj. 受启发的；line art /laɪn ɑːt/ n. phr. 线稿；hand-drawn /ˌhændˈdrɔːn/ adj. 手绘的；sketch texture /sketʃ ˈtekstʃə/ n. phr. 草图纹理；subtitle /ˈsʌbtaɪtəl/ n. 字幕；watermark /ˈwɔːtəmɑːk/ n. 水印。

**译文**：渲染片段只能包含干净、全彩、受皮克斯启发的三维动画。不得有分镜线稿、手绘草图质感、标签或水印；用户未要求时不得有字幕。

### 12｜保持尺寸和分辨率

**词汇释义**：maintain /meɪnˈteɪn/ v. 保持；screen size /skriːn saɪz/ n. phr. 画面尺寸；aspect ratio /ˈæspekt ˈreɪʃiəʊ/ n. phr. 宽高比；approved /əˈpruːvd/ adj. 已确认的。

**译文**：保持已确认的画面尺寸／宽高比，以及分辨率选择卡片中已确认的视频分辨率。

## 模型特定提示词组织

### 13｜共同分镜，不同前缀

**词汇释义**：model-specific /ˈmɒdəl spəˈsɪfɪk/ adj. 模型特定的；feed /fiːd/ v. 提供输入；prefix /ˈpriːfɪks/ n. 前缀；differ /ˈdɪfə/ v. 不同。

**译文**：两个模型都接收文字分镜文档，或该镜头已提取的独立节点，但分镜外层的提示词前缀不同。

### 14｜H3 前缀

**词汇释义**：emphasize /ˈemfəsaɪz/ v. 强调；design language /dɪˈzaɪn ˈlæŋɡwɪdʒ/ n. phr. 设计语言；instruction following /ɪnˈstrʌkʃən ˈfɒləʊɪŋ/ n. phr. 指令遵循；directive /dəˈrektɪv/ n. 指令；verbatim /vɜːˈbeɪtɪm/ adv. 逐字地；cartoon rendering /kɑːˈtuːn ˈrendərɪŋ/ n. phr. 卡通渲染；proportion /prəˈpɔːʃən/ n. 比例；SSS abbr. Subsurface Scattering，次表面散射；on-brand /ɒn brænd/ adj. 符合品牌风格的；palette /ˈpælət/ n. 配色。

**译文**：H3 提示词前缀（默认）：强调视觉包装关键词、设计语言、运动清晰度，相关时说明文字／界面，以及双声道音频意图。源文认为 H3 擅长遵循指令，因此逐秒指令几乎可以逐字传入。添加以下英文内容：

`Pixar-inspired 3D cartoon rendering, C4D + Octane look, stylized Q-version proportions, warm SSS skin, designed-with-detail hair, strong character design language, clean motion, on-brand color palette`

**中文含义**：受皮克斯启发的三维卡通渲染；C4D 与 Octane 观感；风格化 Q 版比例；温暖、带次表面散射的皮肤；细节经过设计的头发；鲜明的人物设计语言；干净的运动；符合品牌风格的配色。C4D 指 Cinema 4D，Octane 为渲染器名称。

### 15｜Seedance 2.0 前缀

**词汇释义**：squash-and-stretch /skwɒʃ ənd stretʃ/ n. phr. 挤压与拉伸；anticipation /ænˌtɪsɪˈpeɪʃən/ n. 预备动作；follow-through /ˈfɒləʊ θruː/ n. 随动；overshoot /ˈəʊvəʃuːt/ n. 超越目标后回摆的动作；dramatic /drəˈmætɪk/ adj. 戏剧性的；key lighting /kiː ˈlaɪtɪŋ/ n. phr. 主光照明；lens-specific /lenz spəˈsɪfɪk/ adj. 对应特定镜头焦段的；depth of field /depθ əv fiːld/ n. phr. 景深。

**译文**：Seedance 2.0 提示词前缀（表演回退）：强调电影式运镜语言、富有弹性的挤压拉伸、预备动作、随动、戏剧性光照与镜头选择。添加：

`cinematic Pixar-quality 3D animation, elastic squash-and-stretch performance, Disney-style anticipation and overshoot, dramatic key lighting, lens-specific depth of field`

**中文含义**：电影式、皮克斯品质的三维动画；富有弹性的挤压拉伸表演；迪士尼式预备动作与过冲；戏剧性主光；与具体镜头相符的景深。

### 16｜混合模式的选择规则

**词汇释义**：apply /əˈplaɪ/ v. 应用；match /mætʃ/ v. 匹配；field /fiːld/ n. 字段。

**译文**：用户选择 `per-shot mixed` 时，采用与当前行 `video_model` 字段对应的前缀。
