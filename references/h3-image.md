# MiniMax H3-Image

当目标是 H3-Image 或海螺中的 H3 图片模型时，使用本页。MiniMax 官方同时提供文生图和参考图编辑，参考上限为 16 张。只选择负责主体、机位、色材或布局的必要图片。 [MiniMax 发布说明](https://www.minimax.io/blog/minimax-h3-image)

## 改写方式

- 默认用英文描述最终画面，画面里实际印出的文字保留原语言、标点和大小写。将宽高比单列为交付设置。编辑时，按实际上传顺序将参考图称作 `<Picture 1>`、`<Picture 2>`。这些是官方示例采用的写法。 [MiniMax 官方提示词指南](https://github.com/MiniMax-AI/MiniMax-H3-Image/blob/main/skills/h3-image-prompt-writing/SKILL.md)
- 拆开描述不同图片的控制范围。例如织物样片只决定纤维和颜色，沙发的轮廓、机位和尺寸仍来自空间底图。多格画面明确写几行、几列，按行列坐标指定文字或局部变化。 [MiniMax 官方编辑样例](https://github.com/MiniMax-AI/MiniMax-H3-Image/blob/main/skills/h3-image-prompt-writing/references/edit-en.txt)
- 对照两个写法的效果时，使用同一入口并记录扩写状态。MiniMax 官方脚本能控制文生图扩写，官方 API 在编辑时会进行扩写。可取得改写文本时一并记录。 [官方工作流说明](https://github.com/MiniMax-AI/MiniMax-H3-Image/blob/main/skills/README.md)

## 原创适配示例

**产品材质样照 · 两图编辑。** 图一是现有台灯的产品照，图二是釉面色样。将参考的“保留什么、借用什么”具体到部件。此法也可对照 Subushie 公开的多参考编辑实验，作者分别声明了各主体和环境的保留程度。 [Subushie 的公开提示词实验](https://www.reddit.com/r/comfyui/comments/1xz07b3/h3_image_edit_model_is_wild_tips_on_usage_based/)

```text
Use the product photograph in <Picture 1> as the base. Refinish only the lamp’s ceramic foot in the mottled sea-green glaze visible in <Picture 2>. Follow the original foot’s curvature with a narrow highlight facing the window. Preserve the linen shade, brass collar, cord, tabletop reflection and framing. Keep the glaze inside the ceramic edges.
```

验收时看釉色止于陶瓷与金属接缝，灯罩的纹理和阴影与底图相符。画幅沿用图一。

**建筑导览海报 · 文生图。** 明确图片和标题各占哪块区域，将想呈现的材质转成可见线索。以下示例从零撰写。

```text
Design a portrait exhibition poster for a public reading room. A cut-paper elevation fills the upper two thirds. Stack three ivory paper layers to describe the recessed doorway, window frames and projecting canopy. Let a single soft shadow fall to the lower right of every raised edge. Center the Chinese title “纸上的阅览室” below the building in dark indigo. Leave a generous bottom margin. This title is the only lettering.
```

画幅 3:4。核对标题逐字正确、纸层阴影同向、门窗与遮檐层级可辨。
