复刻自 [soryu-ryouji/novel-tex-theme](https://github.com/soryu-ryouji/novel-tex-theme)，将 `academic-tex-l.css` 及其依赖的相关文件提取出来，并做出了一定的个性化修改，使之更接近 [Keldos-Li/typora-latex-theme](https://github.com/Keldos-Li/typora-latex-theme) 了一点，虽然是 `academic` 但修改过后已经不再适用于写论文了，可以作为日常使用。

修改内容如下：

- 修改行内代码、超链接颜色为蓝色。
- 修改代码字体为 [`JetBrains Mono`](https://www.jetbrains.com/lp/mono/) ，看起来更顺眼一些。
- 增加了 [Keldos-Li/typora-latex-theme](https://github.com/Keldos-Li/typora-latex-theme)  主题一样的页面阴影。
- 增大页宽为 31cm 。
- 提升了 Dark 主题下整个页面的暗度；提升了 Dark 主题下字体的亮度，使主题没那么”灰蒙蒙“了。
- 修改正文文本的对齐方式： `text-align: justify` 修改为 `text-align: left` 。
- 给 markdown 文档最上方的 YAML front matter 区域增加了 `box-shadow` 属性。
- 修改了 html 代码块部分背景颜色。



---

<div align=center>
    <img src="./.assets/novel-tex-logo.png">
</div>

# Novel Tex

> Novel Tex 是基于 [typora-latex-theme](https://github.com/Keldos-Li/typora-latex-theme) 的修改版本，沿用 GPL 3.0 许可证。

主要修改：

1. 移除了 typora-latex-theme 的标题自动编号特性
2. 修改了 typora-latex-theme 的页面大小与字体大小，优化了笔记本设备的使用体验
3. 将 mermaid 的默认主题修改为灰色，使其与主题风格更加统一
4. 增加了代码块线框，使代码块在文档中更加显眼
5. 更改了默认字体

NovelTex 使用思源宋体作为文档中文字体、Times New Roman 作为文档英文字体、微软雅黑作为 UI 字体、Consolas 作为代码字体

<!-- 思源黑体：https://github.com/adobe-fonts/source-han-sans/releases/download/2.004R/SourceHanSansSC.zip -->

思源宋体：https://github.com/adobe-fonts/source-han-serif/releases/download/2.002R/09_SourceHanSerifSC.zip

> 正文字体相关配置在 `novel-tex\basic\base-config.css`
>
> UI 字体相关配置在 `novel-tex\basic\ui.css`
>
> 代码字体字体相关配置在 `novel-tex\basic\basic-code.css`

## 主题版本介绍

各个主题文件之间没有相互依赖的关系，可以只复制自己需要的主题文件使用，但 `novel-tex` 文件夹需要完整复制，里面包含了主题文件所需要的基础配置。

### 主题颜色

| Name | Description  |
| ---- | ------------ |
| FD   | Full Dark    |
| ND   | Normal Dark  |
| FL   | Full Light   |
| NL   | Normal Lignt |

## 开发指南

所有基础性的配置全部放入`novel-tex/basic/`中，所有与明暗配置相关的内容放入`novel-tex/dark/`与`novel-tex/light/`中，放在根目录的主题文件只用于修改颜色变量。

```shell
theme/
├─novel-tex/
│   ├─basic/
│   ├─dark/
│   └─light/
├─novel-tex-f-d.css
├─novel-tex-f-l.css
├─novel-tex-n-d.css
└─novel-tex-n-l.css
```

考虑到大多数人的使用习惯，表格的对齐方式默认设置为左对齐，如果希望表格默认居中对齐，可以去 `novel-tex/basic/table.css` 的 `#write table` 中修改 `text-align` 变量。

## Screenshots

> 通过身边使用该主题的朋友反馈，主题样式会不定期更新
>
> 文档中的界面预览图与实际安装后的界面不保证百分百相同（有空时会上传新的预览图）


**Full Light**

![fd](./.assets/novel-tex-f-l.png)

![fd](./.assets/novel-tex-f-l-code.png)

**Normal Light**

![fd](./.assets/novel-tex-n-l.png)

![fd](./.assets/novel-tex-n-l-code.png)

**Full Dark**

![fd](./.assets/novel-tex-f-d.png)

![fd](./.assets/novel-tex-f-d-code.png)

**Normal Dark**

![fd](./.assets/novel-tex-n-d.png)

![fd](./.assets/novel-tex-n-d-code.png)
