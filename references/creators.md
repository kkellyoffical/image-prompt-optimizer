# 创作者与风格出处

按任务选案例。每条说明了公开材料能确认的模型或角色，右栏是本项目按该方法重新提炼的写法。模型名记录来源中的实际用法或作者标注的适配范围。迁移到其他模型时，沿用画面约束，在目标模型上另做样图验证。

| 创作者与来源 | 原案例和模型证据 | 可以带进新任务的画法与验收重点 |
| --- | --- | --- |
| [AI构筑师Vision · 平行光栅海报](https://www.xiaohongshu.com/explore/6afab6ef000000002a02cf01) | 小红书。该帖的两条作者评论给出画法，图 5 操作截图标有 GPT Image 2.6 Sunburst。 | 摄影与线描双联。先选底片中一个可辨轮廓，让连续线条在其两侧逐步弯曲；远离轮廓后恢复平行。检查上半幅底片和下半幅线条各自的边界。 |
| [宝玉 · 小红书视觉内容策划师提示词](https://www.baoyu.io/blog/red-book-visual-content-prompts) | 作者博客。将内容拆成逐页图像指令，再交给 Nano Banana Pro 生成系列信息图。 | 在每页重复纸色、标题位置和插画笔触，给每页选一个能画出来的动词。先检查单张独立阅读是否完整，再检查整组标题与插画的节奏。 |
| [歸藏 · 天气移轴 Q 版模型](https://github.com/op7418/guizang-s-prompt/blob/main/image/%E5%A4%A9%E6%B0%94%E7%A7%BB%E8%BD%B4%20Q%20%E7%89%88%E6%A8%A1%E5%9E%8B.md) | 作者 GitHub。歸藏注明灵感来自宝玉，列出 Nano Banana Pro 与 Seedream 作为适配模型。 | 用当地一组可辨地标组成微缩底座，天气用立体物件表现，地名与时间放在单独文字区。日期、天气和地点取自当前任务提供或已核实的信息。 |
| [konmari · 杂志封面](https://note.com/konmari/n/n49acac1e6442) | 创作者在 note 发布的 Nano Banana Pro 封面提示词与读者实践。 | 从参考照里找出主角轮廓、视线方向和可排字空间，再确定刊名与主副标题。验收时把图缩小，确认刊名和人物仍能分别辨认。 |
| [おぱし · 新年贺卡制作记录](https://note.com/ohhpasy/n/n23d639713d34) | 作者实作的 Nano Banana Pro 贺卡，文章明确致谢 konmari 的杂志提示词。服饰三视图是此前在 Gemini 中制作的输入素材。 | 先用服装参考锁住纹样与轮廓，再改变姿态、安排祝词。为寄件人后填文字留连续空白，以打印画幅查看边缘和留白是否够用。 |
| [神屋伸行 · 活动海报与角色换姿](https://note.com/nkamiya/n/n0af324bbc781) | note 作者教程。Nano Banana Pro 的活动公告和同角色换姿两类提示示范。 | 有日期地点的海报把准确文案独立提供，规定信息区与背景的对比。角色连作以同一张定妆图为参照，只改变这一幅的动作与环境。 |
| [Charlie Hills · 摄影提示词拆解](https://charliehills.substack.com/p/how-to-prompt-gpt-image-15) | Substack 作者公开段落逐项解释自己的 GPT Image 1.5 动作人像提示词。 | 把身份参考、快门截取的动作瞬间、人物在画面中的占比写成独立要求。与参考图比对脸部特征，在全身构图中检查手脚是否按任务完整入画。 |
| [Simon Willison · Pedalican 制作记录](https://github.com/simonw/pedalican/blob/main/notes-on-creating-a-pet.md) | 作者 GitHub 项目公开了 GPT Image 2 的生成与编辑记录，包括参考顺序、被退回的修订及原因。 | 制作同角色成组画面时，分别提供版面示意和角色定稿。每组沿用相同道具与轮廓，输出后对齐角色比例，检查相邻格边界。 |
| [Wiro ML Team · 六组摄影与编辑实验](https://wiro.ai/blog/gpt-image-1-5-6-prompt-tests-for-text-and-edits/) | 团队的一手 GPT Image 1.5 对照记录，每种任务展示一次生成结果，包含微距摄影、包装、反射和手表编辑。 | 产品材质分开描述。哑光外壳写漫反射，透明边缘写亮线，投影注明光向；印有字的包装逐字核对，并检查实物边缘透视。 |

## Qwen Image 与 H3-Image 的实践者

| 看什么 | 直接来源与可复用的检验方法 |
| --- | --- |
| Qwen 商品摄影与室内多参考图 | cocktailpeanut 的包装样例可检查标签多处排字；junwatu 的空间布置可检查各张参考是否落在正确位置。[包装示例](https://x.com/cocktailpeanut/status/2102141381036875871) · [多件家具示例](https://x.com/junwatu/status/2101614052514627935) |
| Qwen 叙事分镜与编辑 | 烁皓的分镜展示同一叙事的跨格衔接；listopalafoto 发布了光色编辑指令及对照；Wild_Artichoke7648 展示了拼合和排版的失误。逐格检查动作顺序，逐项核对产品是否遗漏。 [分镜原帖](https://x.com/eternityspring/status/2102241587724206543) · [光色编辑](https://www.reddit.com/r/StableDiffusion/comments/1wlgv0l/i_tested_qwenimage21_its_amazing/) · [五项编辑测试](https://www.reddit.com/r/StableDiffusion/comments/1wp38sw/qwenimage21_vs_sensenova_u15_lite_5_edit_tests/) |
| H3 多参考编辑 | Subushie 公开了分配主体和环境的编辑提示词。可将该方法迁移到产品换材质，分别核对底图结构与样片颜色。 [作者实验](https://www.reddit.com/r/comfyui/comments/1xz07b3/h3_image_edit_model_is_wild_tips_on_usage_based/) |

## 继续查找创作者

- Replicate 的 Nano Banana Pro 专文嵌入了创作者发布的案例，能从整理页下钻到原帖。Pietro Schirano 演示了长文转白板，fofr 演示了文章转桌上的光面杂志。后续收录时分别记录演示者、是否公开完整提示词、以及可核对的成图。 [Replicate 专文及原帖索引](https://replicate.com/blog/how-to-prompt-nano-banana-pro/)
- jamez-bondos 维护的 GPT-4o / GPT Image 1 案例集分别注明提示词署名和图片署名，可用它寻找扁平城市海报、像素图标、云形摄影等一手案例。保留每个条目的归属与原链接；合集中覆盖多个模型，具体版本以单例证据为准。 [作者维护的案例目录](https://github.com/jamez-bondos/awesome-gpt4o-images/blob/main/README_en.md)
