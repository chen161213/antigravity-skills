# 完整实操样例演练 (End-to-End Walkthrough Example)

本文件作为执行参考样例，演示如何将一段 30 秒的财务 SaaS 口播台词，一步步转化为符合 SOP 规范的剧本、参考图 Prompt 及合并视频 Prompt。

---

## 原始输入

* **台词文本**：
  > “月末又到了，你们公司的财务还在一张张手动核对发票、手敲报销单吗？业务部门催着报销，老板催着看财务报表，加班到半夜还容易对错账。其实业财协同真没那么麻烦。试试我们这套智能财务系统，发票一键拍照识别，自动三流合一校验，凭证生成只需要点一下。现在点击左下角，立即申请免费试用。”
* **单次视频生成时长限制**：10 秒

---

## 执行步骤与输出示范

### 1. 【剧本与情绪分镜拆解】

* **人设锁定**：28岁女性资深财务专家/数字化顾问，知性干练，藏青色高定西装配白色内搭，骨相立体清秀，眼神诚恳专业。
* **场景选定**：现代科技公司总部走廊（透视感强，适合走播与痛点直击）。

| 镜头编号 | 预估时长 | 对应台词 | 情绪弧线 | 动作与景别（安全线：中景及以上） |
| :--- | :--- | :--- | :--- | :--- |
| **Shot 1** | 00:00-00:03 (3s) | 月末又到了，你们公司的财务还在一张张手动核对发票、手敲报销单吗？ | **黄金Hook**：直击痛点，反问直视 | 中近景（MCU），快步迎面走来，突然在镜头前驻足微前倾，眼神犀利直视镜头。 |
| **Shot 2** | 00:03-00:07 (4s) | 业务部门催着报销，老板催着看财务报表，加班到半夜还容易对错账。 | **共鸣反思**：感同身受，微无奈 | 中景（MS），转身沿走廊向前缓步走动，后退跟拍，单手克制地做翻动文件手势，微微皱眉后平复。 |
| **Shot 3** | 00:07-00:10 (3s) | 其实业财协同真没那么麻烦。 | **情绪转折**：豁然开朗，释怀自信 | 中近景（MCU），步伐从容稳健，眼神看向镜头，嘴角露出一丝胸有成竹的从容微笑。 |
| **Shot 4** | 00:10-00:14 (4s) | 试试我们这套智能财务系统，发票一键拍照识别，自动三流合一校验， | **方案价值**：坚定客观，数字化赋能 | 中景（MS），继续向前走播，单手抬起做逻辑递进指引手势，背景光斑自然流转。 |
| **Shot 5** | 00:14-00:17 (3s) | 凭证生成只需要点一下。 | **极简体验**：轻松肯定 | 中近景（MCU），驻足侧身微顿，右手做出轻巧轻点动作，神情笃定专业。 |
| **Shot 6** | 00:17-00:20 (3s) | 现在点击左下角，立即申请免费试用。 | **行动号召 (CTA)**：真诚引导，促转化 | 中近景（MCU），身体微微前倾靠近镜头，眼神真诚锁定观众，左手微向下做自然指引，亲和力拉满。 |

---

### 2. 【资产生成提示词 (生图)】

#### 人物参考图 (Photographic Identity Sheet)
* **Prompt (EN)**:
  ```text
  Real-world photographic identity sheet of the same person photographed across multiple angles, contact sheet presentation on neutral matte light grey studio background. Subject: Exceptionally beautiful 28-year-old East Asian female corporate executive, stunningly attractive, high visual appeal, delicate high-end bone structure, exquisite facial proportions, large expressive bright eyes, elegant nose bridge, soft feminine jawline. Complexion: Flawless fair porcelain skin, luminous translucent skin tone, smooth dewy and radiant texture, healthy glowing fair complexion with subtle pink undertones. Makeup: Sophisticated clean dewy corporate beauty makeup, soft feathered brows, subtle earth-tone eyeshadow, moisturizing soft berry-nude satin lipstick. Aura: High-class intellectual elegance, captivating yet trustworthy executive presence. Wardrobe: Bespoke tailored dark charcoal wool blazer, single-button, crisp ivory silk collared shirt. Hair: Sleek shoulder-length dark espresso hair, neatly styled with left side tucked behind ear, glossy healthy sheen. Accessories: Holding a slim black textured leather portfolio folder under right arm. Layout: Top row shows full-body turnaround (front view, three-quarter view, side profile view, back view). Bottom row shows close-up portrait views (front portrait, three-quarter portrait, profile portrait, and speaking expression with lips softly parted showing upper teeth in active dialogue cadence). Lighting: Clean commercial studio beauty lighting, soft wrap-around daylight, gentle catchlight in the eyes, 8k resolution, shot on Hasselblad H6D-100c, 85mm portrait prime lens, commercial luxury advertising grade --ar 16:9 --style raw
  ```
* **中文提示词**:
  ```text
  真实工业级人物摄影多角度身份表，8格接触印相表排版，纯净浅中性灰色影棚背景。主体人物：极其漂亮出众的28岁东亚女性企业财务高管，顶级高阶骨相美，五官极其精致优越，明亮灵动的大眼睛，高挺秀气鼻梁，比例完美，颜值出众极具视觉吸引力。肤质肤色：通透冷白皮，白皙细腻透亮如凝脂，带有健康光泽感的微光水光肌底，肤色纯净白嫩，白里透红，绝无暗沉粗糙。气质妆造：高级清冷知性气质，兼具亲和力与商界精英气场；轻透高级微光感职场妆容，水润豆沙色唇妆。身着合身剪裁的高级深炭灰羊毛西装内搭象牙白真丝衬衫。右腋下夹带超薄黑色真皮公文夹。版面布局：上排为全身三视图（正面、3/4侧面、正侧面、背面）；下排为肖像特写（正面美颜特写、3/4侧特写、正侧特写、以及微张口说话露齿的生动口型动态特写）。商业广告级通透柔光人像布光，双眼带清晰眼神光，哈苏中画幅商业人像质感，8k超清。
  ```

#### 场景参考图 (大厂高规格实景)
* **纯中文提示词**:
  ```text
  国内头部互联网大厂总部开阔办公区主走道实景拍摄，真实甲级写字楼现场取景，拒绝低端小办公室，拒绝虚假3D渲染。
  空间挑高开阔极具纵深感，拒绝廉价矿棉板吊顶，天花板为极简现代无主灯设计与嵌入式黑色轨道射灯。
  一侧为巨大的全景落地玻璃幕墙，洒进明亮通透的大面积白天自然采光，窗边摆放着高脚木质吧台椅与生机盎然的琴叶榕绿植盆栽。
  另一侧是整齐通透的高端原木色与纯白色开放式办公工位，搭配黑色高级人体工学椅，无老气遮挡隔断屏风，视野极度通透。
  地面为整洁高档的浅灰色密织静音办公地毯，空间宽敞大气，充满真实一线科技大厂的高端专业实力感，高清实拍质感。
  ```

---

### 3. 【MiniMax H3 专用视频生成提示词 (全中文 I2VA 架构)】

#### 大镜头 A (时长 10s，对应 Shot 1 ~ Shot 3)
* **包含台词**：“月末又到了...加班到半夜还容易对错账。其实业财协同真没那么麻烦。”
* **MiniMax H3 全中文提示词**：
  ```text
  对于目标视频，在目标视频的 0.00 秒处，完全参考 <Picture 1>（仅提取人物五官神态与服饰，严禁生成多格排版，下半身裁切至膝盖处），并融合 <Picture 2> 的大厂长廊透视背景。

  综合多模态描述:
  [Shot 1] 镜头开篇呈现居中标准【开阔中全景 / 膝盖景 (MLS)】，画面顶部严格保留 28% 的大面积开阔背景留白（Headroom），人物发顶严禁靠近上边缘，双眼严格位于画面垂直方向上三分之一黄金分割线。画面下边缘严格切在膝盖处（露出套裙与双腿至膝盖上方，脚踝与脚掌不入镜），绝美28岁东亚女性企业财务总监 (S1)，极度白皙通透冷白皮，身着高定深炭灰修身羊毛西服。她呈现出【极其缓慢地漫步、悠闲小步踱步】的极低步频状态，严格遵循【步伐轻缓慢节奏，走走停停，边说边轻微位移】，身体重心随讲话从容呈现极轻微左右晃动（Weight Shift），每 3 秒仅极其轻微迈出半步微调，整体闲庭信步。起步双手自然搭在腹前，在 00:01.80，右手优雅脱离腹部微抬至胸前，做从容的单手食指轻点与微摊手势以加强反问语气。摄像机在视平线高度保持 3.5 米开外恒定视距平稳匀速直线后退（0.3m/s），主体大小在画面中保持恒定，严禁逼近或贴近镜头。嘴唇与下颌伴随普通话发音清晰开合，(S1) 带着关切反问说道：<d>[普通话] 月末又到了，你们公司的财务还在一张张手动核对发票、手敲报销单吗？</d>
  [Shot 2] 在 00:03.00，右手顺势自然落回腹前轻搭；继续保持【步伐轻缓慢节奏，走走停停，边说边轻微位移】。在 00:04.50，伴随讲述痛点，右手再次轻抬在胸前做克制有节奏的递进指引手势，眼神流露出一丝无奈感慨，在 00:06.00 手势自然放回腹前，摄像机保持 3.5 米恒定距离同步平滑慢速后退，景别稳定锁定膝盖景与 28% 头顶留白，(S1) 语调带有一丝无奈感慨：<d>[普通话] 业务部门催着报销，老板催着看财务报表，加班到半夜还容易对错账。</d>
  [Shot 3] 在 00:07.00，依然保持【悠闲小步踱步、边说边轻微位移】的从容节奏，(S1) 表情豁然开朗，在 00:07.50 双手从腹前从容向两侧微微自然对称摊开（如对标视频般大方舒展，掌心微侧向镜头），嘴角露出一丝从容舒展的自信微笑，眼神直视镜头，在 00:09.20 双手平缓归位合拢于腹前，(S1) 语气坚定自信地说道：<d>[普通话] 其实业财协同真没那么麻烦。</d>

  【动态禁令约束】:
  严禁正常步速、严禁连续快步迈进、严禁大步流星与快速位移，必须严格保持极慢步频与走走停停；严禁人物逼近镜头；严禁全程双手僵死不动；严禁大幅度甩手或动作抽搐；严禁腰部以上中近景或特写；严禁头顶留白小于 25%；严禁下半身出现滑步、穿模或动态模糊。

  整体音景:
  高端科技公司大平层通透走廊自然安静的声学空间混响，说话人清晰自然饱满的语音投影与呼吸感。

  非剧情音乐:
  无
  ```

#### 大镜头 B (时长 10s，对应 Shot 4 ~ Shot 6)
* **包含台词**：“试试我们这套智能财务系统...凭证生成只需要点一下。现在点击左下角，立即申请免费试用。”
* **MiniMax H3 全中文提示词**：
  ```text
  对于目标视频，在目标视频的 0.00 秒处，完全参考 <Picture 1>（来自上一镜头最后一秒尾帧，严禁发生跳切变形）。

  综合多模态描述:
  [Shot 1] 顺畅接续 <Picture 1> 的运镜动线，景别稳定保持【中全景 / 膝盖景 (MLS)】，画面下边缘稳定卡在膝盖处。(S1) 保持极缓步从容漫步向前，双手微叠腹前，右手在 00:02 做轻微从容的单手递进指引手势，眼神充满专业信服力，(S1) 清晰讲解道：<d>[普通话] 试试我们这套智能财务系统，发票一键拍照识别，自动三流合一校验，</d> 摄像机以极慢速（0.5m/s）保持 2.5 米恒定视距平稳后退。
  [Shot 2] 在 00:04.00，(S1) 在开阔玻璃窗前优雅从容缓步停驻，侧身微正面向镜头，双手自然交叠腹前，右手食指在胸前轻巧做出一次克制单点手势，露出自信从容微笑，(S1) 轻松说道：<d>[普通话] 凭证生成只需要点一下。</d> 摄像机平滑缓冲停稳为固定中全景。
  [Shot 3] 在 00:07.00，保持原地优雅站立，身姿挺拔，仪态高贵知性，双手自然轻叠于腰前，眼神真诚饱满锁定观众发出号召：<d>[普通话] 现在点击左下角，立即申请免费试用。</d>

  整体音景:
  连续的现代办公走廊安静环境底噪，环境脚步声平稳安静，转为清澈饱满的真人广告配音质感。

  非剧情音乐:
  无
  ```
