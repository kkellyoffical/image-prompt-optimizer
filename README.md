# Image Prompt Optimizer

一个按**画面风格 × 目标模型**组织的生图提示词技能。用它把简短需求、底图和风格参考整理成可直接交给模型的提示词，也可以为同一任务生成多种模型写法。

重点维护 Qwen Image 2.1、OpenAI GPT Image 系列、MiniMax H3-Image 和 Google Gemini Nano Banana，另含 Midjourney 的风格参考用法。技能包自带公开来源和案例索引，可独立使用。

## 使用

将仓库克隆到个人 Codex 技能目录。

```sh
git clone https://github.com/kkellyoffical/image-prompt-optimizer.git ~/.codex/skills/image-prompt-optimizer
```

在支持读取 `SKILL.md` 的客户端中，也可以将仓库作为技能目录加载。可以这样调用。

> 用 $image-prompt-optimizer 为这两张图写 Qwen Image 2.1 和 Nano Banana 提示词。图一是客厅模型，图二只借午后百叶窗的光。保留机位和家具布局。

> 我要一张无字的海岛旅行明信片。把原照上方的蓝色海面延伸成下方的三色版画，最后用 imagegen 出图。

## 从哪里开始读

- [技能入口](SKILL.md) · [按风格查画法和验收项](references/styles.md)
- [同一组参考图在四种模型上的写法](references/comparison.md)
- [创作者与可追溯的案例](references/creators.md) · [AI构筑师Vision 的 45 个案例](references/vision-cases.md)

比如“让台灯更有质感”，可以具体化为“只在陶瓷灯座上使用色样中的青釉，让窗光沿弧面形成一条亮带，保留金属接环、亚麻灯罩和电线投影”。模型页进一步说明怎样引用图片、交付画幅和处理版本差异。

## 维护与贡献

新风格请提供代表案例、输入条件、可观察的画法和一个可对照成图的验收项。记录作者账号、原帖链接、作者标注的模型及证据位置；读者复现、策展收录与作者演示分别注明。若验证过出图，请附使用的入口、版本与结果。更新某个模型时只需修改其参考页和受影响的示例。

## 致谢与许可

特别感谢小红书创作者 **AI构筑师Vision** 分享作品、操作截图和提示词，尤其是平行光栅海报、分色景观模型和室内编辑案例，为本技能最初的风格索引提供了实例。也感谢在[创作者索引](references/creators.md)中列出的作者与整理者。 [AI构筑师Vision 的小红书主页](https://xhslink.cn/o/975ccPviWhI) · [平行光栅原帖](https://www.xiaohongshu.com/explore/6afab6ef000000002a02cf01) · [分色景观原帖](https://www.xiaohongshu.com/explore/6afd5cf4000000002a02c256)

本仓库的原创技能说明、索引编排与自拟示例按 [Apache License 2.0](LICENSE) 发布。链接所指的作品、原帖及其配图由相应权利人保有权利，引用时请沿用原作署名和许可。
