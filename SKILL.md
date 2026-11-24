---
name: image-prompt-optimizer
description: Optimize or translate image generation and editing prompts for Qwen Image 2.1, OpenAI GPT Image and Codex imagegen, MiniMax H3-Image, Gemini Nano Banana, or Midjourney. Select a visual recipe by style, separate the roles of reference images, and tailor the prompt to the requested model and interface.
---

# 按画面效果和模型优化生图提示词

先识别交付物、编辑对象、已有参考和用户指定的模型。提示词任务交付一段可以直接使用的提示词；只有用户需要多个模型时才给并排版本。用户要求出图时，通过可用的目标工具执行。用户指定的模型没有可用入口时交付为它写好的提示词，并说明执行条件。在 Codex 中，未指定模型的出图任务可以使用内置 imagegen。

## 选画法

从[风格选型表](references/styles.md)挑一个主案例。需要更细的建筑、室内、平面海报做法时，按交付物查[45 个小红书案例](references/vision-cases.md)。在原采集项目中还可以用当地的 `素材库/ImageGen索引.md` 核对样图和原始指令。研究原帖出处或寻找更多风格时，查看[创作者来源](references/creators.md)和[原案例模型证据](references/xiaohongshu-models.md)。

将案例里的画法迁移到用户的主体。优先选择两三个看得见的特征，例如“细线沿塔身隆起，在天空区域恢复水平”，或“粗糙陶釉呈宽高光，抛光杯沿只有一道亮边”。画幅、文字、色盘、人物和构图以本次需求为准。没有相近风格时，直接用用户的视觉描述。

## 选模型

只读本次目标对应的一页。原案例的出图模型用于追溯；同一个案例可以改写给其他模型。目标未知且只要求写词时，给可移植的自然语言稿。

| 目标入口 | 参考 |
| --- | --- |
| Qwen Image 2.1 | [Qwen Image](references/qwen-image.md) |
| OpenAI GPT Image 或 Codex imagegen | [GPT Image](references/gpt-image.md) |
| MiniMax H3-Image | [H3-Image](references/h3-image.md) |
| Google Gemini Nano Banana | [Nano Banana](references/nano-banana.md) |
| Midjourney | [Midjourney](references/midjourney.md) |

## 整理成可用输入

- 从零生成时，把主体、媒介、构图和用光组织成一幅具体画面。只有实际提供了参考图，才在提示词中按传入顺序分配角色。
- 编辑时说明选区、改动和相邻保留项。风格参考只借指定的光、色、材质或画法。系列图写清跨图保持一致的特征。
- 需要渲染的文案逐字写入，指定位置和层级。把工具能单独设置的参数放在提示词之外；将用户未指定的偏好按需列为可替换项。
- 用案例的验收项检查实际输出。若当前只写词，交付时可提供一个能对着成图检查的标准。做跨模型对照时共用一套素材、画幅、文案和验收项。[四种模型的同题示例](references/comparison.md)
