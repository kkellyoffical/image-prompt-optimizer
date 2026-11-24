# 同一组参考，四份可交付提示词

**任务**　用户给了两张图。图一是台灯产品照，图二是海绿色釉面色样。用户只想改陶瓷灯座，沿用图一画幅，继续用作商品详情图。下面是原创的输入示例，上传顺序均为产品照、色样。四份稿共同锁定用户的要求，以便比较实际成图。

## Qwen Image 2.1

```text
编辑<image1>中的台灯产品照。把陶瓷灯座表面换成<image2>的海绿色斑驳釉面，让细小色斑沿灯座弧面自然分布，在朝窗一侧留一道柔亮反光。材质在黄铜接环处整齐收边。灯罩、接环、电线和台面位置沿用<image1>，保留原来构图、光向和投影。
```

实际配置按使用入口填写。需要严格对比时，记录该次是否启用提示词改写。 [Qwen 适配说明](qwen-image.md)

## GPT Image

> 以第一张产品照为编辑底图，镜头、灯具轮廓和摆放位置沿用原照片。只替换黄铜接环下方陶瓷灯座的表面，用第二张色样的海绿色釉与不规则细斑覆盖陶瓷。窗边柔亮的反射顺着曲面变窄，在接环处结束。灯罩保留亚麻织纹，桌上电线与投影保留原位置。

传入两张图片。用户要求透明背景或精确画布时，把入口支持的选项另列。 [GPT Image 适配说明](gpt-image.md)

## MiniMax H3-Image

```text
Edit the lamp photograph in <Picture 1>. Apply the mottled sea-green glaze from <Picture 2> only to the ceramic base below the brass collar. Curve the window highlight around the glazed body. Keep the rim clean where the glaze meets the brass. Preserve the linen shade, the cord, the tabletop shadow and the framing of <Picture 1>.
```

画幅沿用底图。 [H3-Image 适配说明](h3-image.md)

## Gemini Nano Banana

> 使用上传的第一张照片决定台灯造型、机位、光源和桌面环境。第二张只提供灯座釉面的海绿色、细斑尺度和反光质地。请基于第一张出一张成品照，让釉层贴合原灯座曲面并止于金属接环；亚麻灯罩、灯线、灯具尺寸和桌面投影与原照一致。

需要再微调时，对准已选成品提出一个局部变化，例如“把灯座亮边收窄一些”。 [Nano Banana 适配说明](nano-banana.md)

## 对照成图

1. 对齐两图后，灯罩外缘、接环和电线是否重合？
2. 釉斑是否有曲面起伏，反光方向是否与窗光一致？
3. 金属和亚麻是否保有各自的颜色与纹理？

这些是提示词设计稿。实际测试时记录模型版本、入口、素材、扩写状态、成图及具体通过项，便于回看哪一种写法在当前任务上有效。
