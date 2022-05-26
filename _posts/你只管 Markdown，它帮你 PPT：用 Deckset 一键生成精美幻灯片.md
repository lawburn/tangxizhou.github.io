---
layout: post
title:  "你只管 Markdown，它帮你 PPT：用 Deckset 一键生成精美幻灯片"
---
## 前言

对我而言，做 ppt 实在是一件消耗精力的事，这并不是因为有多难，而是在做 ppt 的时，需要去频繁地拖动鼠标去把元素放在某个位置、调整它们的大小，反复修改等等……那么如果不是在大型项目进行展示，只是在小团队内部展示或者录制一个教程，我希望能有好看的模版，我只需要从中挑一个我喜欢的，并且我不需要手动应用样式，我只需要专注于把内容写上去就可以了。

我之所以喜欢 MarkDown，因为我们喜欢用语义逻辑去完成内容，我在我想要的标题前面加个 `#`，我就知道它将以一个标题的大小展示，而不是选中标题去调整样式，也就是做到了「内容与格式分离」

那么我们自然会想到能否把 MarkDown 文件转换成 ppt 文件，号称「文档的瑞士军刀」的 Pandoc 可以做到，并且 Obsidian 也有个插件叫做「Pandoc Plugin」，可以直接在 Obsidian 里进行转换，而不用打开终端，如果你和我一样没法翻墙，无法访问社区插件，你可以在这里搜索下载 https://ob.pory.app

但是这样做有一个问题，使用 Pandoc 转换出的 ppt 非常的不美观，只是白底黑字的堆砌，你需要将导出的 ppt 应用于一个提前准备好的母版，但这样就做不到了「所想即所得」，试想一下，假如每次编辑完 md 文件都需要导出才能看到效果的话，一定会很恼人吧。

能不能有一个软件，不仅不需要应用母版就得到精美的效果，最好连导出这一步也不要，能直接把 md 文件预览为 ppt 的样式，就像平时使用 MarkDown 做笔记一样自然，我看到 ppt 的样式后，我也不要再导入 PowerPoint 里再使用，我要直接在这个软件里开始我的演讲。

Deckset 就是专门服务将 MarkDown 转为 ppt 文件这个需求的，我会将 deckset 放在屏幕左侧md 文件放在右侧，由于此时 md 文件是为了制作 ppt 而不是写文章，所以我不需要打开 markdown 编辑器看到它的预览效果，使用 mac 自带的文本编辑就足够了，文本编辑检测到你短时间内没有操作时就会保存文件，ppt 也会随之更新，如果你想立马看到改动后的 ppt 效果，就按 cmd + s手动保存。

![分屏使用演示](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/分屏使用演示.png)

## 有多少主题？

共有 21 个主题，每个主题都有多种配色，我最喜欢的配色是 skecnote 里的第一个配色，很有万圣节的风格。

![最爱主题展示](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/最爱主题展示.png)

## 如何使用

### 导言区

导言区是写在文档开头对 ppt 的一些设置，因为 LaTeX 里把这个部分叫导言区，我也就把这个部分叫做导言区了。

![导言区](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/导言区.png)

`.autoscal`：内容自动缩放，deckset 会自动根据你标题正文的字数分配空间、设置大小，但如果你的内容太多又想放在一页 ppt 里，你可以开启这个选项让 deckset 自动缩放你内容以将它们全部放下。

`.build-lists`：你可以像在 MarkDown 里写 `- ` 或 `1.` 构建无序列表和有序列表，而这个设置可以让你播放 ppt 时使列表里的各个项依次出现，乔布斯也说，要让你的观众每次只关注于一个内容。

另外我觉得非常细节的一个设计是，你可以第一行写 `1. `，其余行写 `- `，这将仍会是一个有序列表，方便你在列表中添加删除项的时候不用再修改项的序号。

![列表以此出现](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/列表以此出现.png)

`.slidenumber`：在 ppt 每一页右下角标注页码

`.footer`：每一页 ppt 下方加上脚注，通常写上内容的作者或出品方

![脚注](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/脚注.png)

### 展示形式

#### 代码

![代码](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/代码.png)

#### LaTeX 数学公式

![数学公式](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/数学公式.png)

#### 音频视频

![音视频](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/音视频.png)

#### 图片

插入的图片除了直接放在内容中，页可以设置放在左侧或者右侧，deckset 里还支持将你的图片作为背景，并会自动调色与你的主题相配。

![图片](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/图片.png)

#### 表格

![表格](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/表格.png)

#### 注释

在页面下方用小字注释正文中的内容。

![注释](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/注释.png)

### 其他功能

#### 演讲者模式

在你演讲时，演讲屏幕呈现的是 ppt 内容，而在你的 mac 上会额外展示一页内容，用于提示你演讲的思路。

![演讲者模式](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/演讲者模式.png)

#### 练习演讲模式

在你演讲时，同时也会出现下一页内容，帮助你练习演讲时打磨自己的思路，乔布斯每次在做演讲前，都会自己演练很多遍，重要的场合，演练是很有必要的。

![练习演讲模式](https://tangxizhou-1306036558.cos.ap-beijing.myqcloud.com/uPic/练习演讲模式.png)

## 结语

这是 deckset 的官网 https://www.deckset.com/features/ ,你可以下载试用版本，deckset 为个人或团队出售，如果你是教育工作者，可以获得 50% 的折扣。

 这篇文章里我只是展示了 deckset 大概有哪些功能，并没有多讲具体的语法，你只要打开 deckset 的菜单栏点击帮助，开发者写的文档非常短小精悍，你只需花几分钟就能掌握 deckset 的所有用法，我愿称之为教科书级的帮助文档。

还有一点需要注意的是，你可以直接在 deckset 里进行演讲，但它并不支持直接导出为 ppt 格式，我猜测是上面我介绍的各种展示效果很难直接在 ppt 里简单地去做到，但你可以导出为一系列 PNG 或 JPG 图片，打开 PowerPoint 将图片都放进去就好了。

我个人很喜欢将 deckset 用于组内讨论、录屏制作教程以及应付学校老师布置的任务，希望你也能享受这个软件。
