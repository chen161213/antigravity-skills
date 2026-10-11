# 提示词词库（正向 / 负向，各只维护这一份）

视频提示词中，【步态】块引用正向词一次，【禁令】块引用负向词一次。不要在每个 Shot 里重复粘贴。

## 一、正向词库

**步态与节奏（中文，MiniMax H3 / 国内模型）**
- 极其缓慢地漫步、悠闲小步踱步、步伐轻缓慢节奏、闲庭信步
- 走走停停，边说边轻微位移、身体重心从容轻微左右晃动、原地小步微调慢移
- 摄影机平稳匀速直线后退，保持恒定视距（速度取自 video_prompt_spec 数值表）

**英文（Runway / Kling / Luma / Sora 等支持英文的模型）**
`extremely slow-paced stroll, leisurely small steps, relaxed pace, occasional pause while speaking, gentle weight shift, micro-stepping, steady camera backward movement at a fixed distance, medium long shot framed at the knees`

## 二、负向词库

**独立负向框（支持 Negative Prompt 的模型）**
- 英文：`fast walking, rushing, hurrying, large steps, fast movement, motion blur, running, sudden zoom, abrupt movements, close-up face distortion, foot sliding, aggressive walking`
- 中文：`快走、急促赶路、大步走、快速位移、冲刺、奔跑、面部大特写压迫、滑步、动态模糊、突兀动作`

**MiniMax H3 内嵌禁令句（无独立负向框，直接写进描述，每段一次）**
`【禁令】严禁快走、急促赶路、大跨步或快速位移；严禁人物加速逼近或贴近镜头；严禁头部大特写与腰部以上中近景；严禁头顶留白小于25%；严禁下半身滑步与穿模；严禁全程双手僵死不动，也严禁大幅甩手或手指抽搐。`

## 三、人物外观正向词（生图用）

- 肤质：通透冷白皮、细腻白皙、水光肌底、健康光泽、白里透红、纯净通透
- 骨相：精致优越的五官、明亮灵动的大眼睛、高挺秀气的鼻梁、流畅紧致的下颌线、比例完美
- 避免写入：粗糙、毛孔明显、细纹、暗沉、瑕疵等会让人物显老或变黑的词；也避免"塑料感、充气网红脸"出现在正向描述里（用"自然协调"类正向词替代）。
