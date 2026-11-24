# GPT Image 与 Codex imagegen

用自然语言写一条完整指令。双联海报先交代整张画幅，再分别描述上下区占比、原图保护范围和下区画法。把“细腻、有质感”写成可见特征，例如细线连续、弯曲集中在主体周围、离开主体后逐渐恢复平直。优先借光栅双联、室内转杂志插画、景观拼贴或材质轴测案例的操作逻辑。

局部编辑以用户原图为底，定位具体对象、边缘和边界，写清区域外的机位、光线及必要细节。多图输入按顺序编号，把几何、材质、光色的控制权给对应图。双联原照区需要像素级保真时，将模型生成用于重绘区，原照作为版面素材直接合成。

内置 imagegen 以实际工具参数为准。当前内置接口未暴露模型版本选择。素材出处里的 2.5 或 2.6 用于标记样例。明确使用 OpenAI API 时，再按接口文档核对模型 ID、画幅和其他参数，并把可设置的参数与提示词正文分开。 [OpenAI 图像提示词指南](https://developers.openai.com/api/docs/guides/image-prompting) · [Images API](https://developers.openai.com/api/reference/resources/images/methods/generate)

## 两种不同成品

- **连贯角色分镜。** 图一负责角色定稿，图二负责格子大小。把每格动作写出来，“第二格仍戴左侧有缺口的红帽，伸手扶住自行车把手”。检查车轮是否跨出格子、帽子缺口是否换边。可以从 Simon Willison 的制作记录回看他为什么退回某些修订。 [Pedalican 制作记录](https://github.com/simonw/pedalican/blob/main/notes-on-creating-a-pet.md)
- **展览封面。** 将标题逐字放入引号，把准确位置写成“落在门廊上方留白的左半边”。若输出错字，下一轮指定该行和正确文案，同时保留现有图片、字号层级与基线。 [OpenAI 提示词指南](https://developers.openai.com/api/docs/guides/image-prompting)
