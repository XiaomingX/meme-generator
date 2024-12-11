### Meme生成API

这是一个基于URL自动生成图片地图的API服务。

## 图片生成方式

这个API是无状态的。不用保存任何信息在服务器上，所有信息都包含在URL中。例如：

**例子链接**: [https://api.memegen.link/images/buzz/memes/memes_everywhere.webp](https://api.memegen.link/images/buzz/memes/memes_everywhere.webp)

![示例图片](https://api.memegen.link/images/buzz/memes/memes_everywhere.webp?width=800)

## 图片格式

API支持下列格式的图片：

| 图片格式 | 示例 |
|-----------------|-------|
| PNG | [高质量 PNG](https://api.memegen.link/images/ds/small_file/high_quality.png) |
| JPEG | [小文件 JPEG](https://api.memegen.link/images/ds/high_quality/small_file.jpg) |
| GIF (动画背景) | [动画 GIF](https://api.memegen.link/oprah/you_get/animated_text.gif) |
| GIF (静态背景) | [静态 GIF](https://api.memegen.link/iw/animates_text/in_production.gif) |
| WebP (动画背景) | [动画 WebP](https://api.memegen.link/images/oprah/you_get/animated_text.webp) |
| WebP (静态背景) | [静态 WebP](https://api.memegen.link/images/iw/animates_text/in_production.webp) |

## 自定义图片尺寸

你可以通过`width=<字面>`和`height=<字面>`参数调整图片尺寸。例如：

**例子链接**: [自定义尺寸](https://api.memegen.link/images/both/width_or_height/why_not_both~q.png?height=450&width=800)

![自定义图片](https://api.memegen.link/images/both/width_or_height/why_not_both~q.png?height=450&width=800)

## 专用字符

为了保持URL的正确性，在地图中使用特殊字符时需要做下列转换：

| 原始字符 | 转换后 |
|-----------------|--------|
| 空格 | `_` 或 `-` |
| `_` | `__` |
| `-` | `--` |
| `?` | `~q` |
| `&` | `~a` |

## 模板列表

想要查看可用地图模板，可访问下面链接：

[模板列表](https://api.memegen.link/templates/)

## 自定义样式

用`style=<样式名>`参数来选择图片样式。

示例：

![默认样式](https://api.memegen.link/images/ds.png?width=375)

![更换样式](https://api.memegen.link/images/ds.png?width=375&style=maga)

## 样式变驱

你可以通过设置`layout=<样式名>`来调整文字的位置。

![文字位置](https://api.memegen.link/images/rollsafe/When_you_have_a_really_good_idea.webp?layout=top)

