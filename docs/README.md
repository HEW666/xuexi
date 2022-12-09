# 冷知识
- [ ] 1.在一个 HTML 中已使用一种引号，你可以在此引号中嵌套另外一种引号：

- [ ] 2.在HTML当中不管打多个空格，多个换行都会被解释为一个空格符

- [ ] 3.你可以将一些内容转换为链接，你只需要把你想要的内容放在`<a>`标签里

# 分析HTML
`<html></html>`: `<html>`元素。这个元素包裹了整个完整的页面，是一个根元素。

`<head></head>`: `<head>`元素。这个元素是一个容器，它包含了所有你想包含在 HTML 页面中但不想在 HTML 页面中显示的内容。这些内容包括你想在搜索结果中出现的关键字和页面描述，CSS 样式，字符集声明等等。

`<body></body>`: `<body>`元素。包含了你访问页面时所有显示在页面上的内容，文本，图片，音频，游戏等等。

# <head>标签
`<title></title>`: 设置页面标题，出现在浏览器标签上，当你标记/收藏页面时它可用来描述页面。

`<meta charset="utf-8">`: 这个元素设置文档使用 utf-8 字符集编码，utf-8 字符集包含了人类大部分的文字。基本上他能识别你放上去的所有文本内容。毫无疑问要使用它，并且它能在以后避免很多其他问题。
## 作者描述
用于**搜索引擎优化**
```
<meta name="author" content="Chris Mills">

<meta name="description" content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing web sites and applications."
```
## 在你的站点增加自定义图标
1.将其保存在与网站的索引页面相同的目录中，以 .ico格式保存
2.将以下行添加到 HTML 的 `<head>` 中以引用它：
`<link rel="icon" href="favicon.ico" type="image/x-icon">`
## 插入 CSS
`<link>`元素经常位于文档的头部。这个 link 元素有 2 个属性，rel="stylesheet" 表明这是文档的样式表，而 href 包含了样式表文件的路径：
`<link rel="stylesheet" href="my-css-file.css">`


# 其他元素
## 超链接
`<a>`//超链接 例：`<a href="https://download.mozilla.org/?product=firefox-latest-ssl&os=win64&lang=zh-CN"
   download="firefox-latest-64bit-installer.exe">` download是保存的文件名

### 锚点
在`<a>`标签的`href`里添加`#首页` 然后在要跳的位置写`name="首页"`

### 电子邮箱链接
`<a href="mailto:1365884335@qq.com">向 畫未 发邮件</a>`
#### 指定详细信息
发送带有抄送、密件抄送、主题和正文的邮件  
`<a href="mailto:1365884335@qq.com?cc=z1314s5201314@qq.com&bcc=2926862683@qq.com&subject=这里是标题&body=这里是内容">
  Send mail with cc, bcc, subject and body
</a>`
cc是抄送 bcc是密件抄送 subject 是标题 body 是内容

## 图片

`<img>`//图片链接 例：`<img src="图片链接地址" alt="无障碍阅读">`


# 标签
title: 例如：title="标题"。当鼠标悬停在超链接上面时，这部分内容将会提示

target: target="_blank"用新网页打开链接。如果你希望在当前标签页显示链接，忽略这个属性即可。其他属性暂不知作用（常用于`<a>`标签）。

# 注释

`<!-- <p>我在注释内！</p> -->`  
我更喜欢用 // 不喜欢用 `<!-- 太麻烦了 -->`

# 列表排序

`<ul>`//无序列表

`<ol>`//有序列表

`<li>`//开始排序
# 字体样式
  `<s>删除线</s>`
  `<u>下划线</u>`
  `<i>斜体</i>` `<em>斜体</em>`
  `<b>粗体</b>` `<strong>粗体</strong>`

# 高级文本
## 描述列表
`<dl>` 开始  
`<dd>` 缩进  
`<dt>` 顶格

## 缩略语
`<abbr title="美国国家航空航天局（National Aeronautics and Space Administration）">NASA</abbr>`  
代码的显示效果如 <abbr title="美国国家航空航天局（National Aeronautics and Space Administration）">NASA</abbr>

## 标记时间和日期
`<p>This article was created on <time pubdate>2011-01-28</time>.</p>`
- 不知道有啥用
## 上标下标
用途：使用日期、化学方程式、和数学方程式时会偶尔使用上标和下标。
| 例子 | 代码 | 说明 |
| :-----| :---- | :---- |
| x<sup>2</sup> | `<sup>`| 上标 |
| C<sub>8</sub> | `<sub>`| 下标 |

## 展示计算机代码
| 标签 | 说明 |
| :-----| :---- | 
| `<code>` | 代码模块，不会被吞  |
| `<pre>` | 可以使标签内保留空白，常用于`<code>`  |
| `<var>` | 斜体，用于标记具体变量名。 |
| `<kbd>` | 用于标记输入电脑的键盘（或其他类型）输入。 |
| `<samp>` | 用于标记计算机程序的输出。 |

- 不知道有啥用

# 在HTML中引用特殊字符
**HTML 中，字符 <、>、"、' 和 & 是特殊字符。**
| 原义字符 | 字符引用 |
| :-----| :---- |
| < | `&lt;` |
| > | `&gt;` |
| " | `&quot;` |
| ' | `&apos;` |
| & | `&amp;` |

如果你要向用户展示这些特殊字符可以引用。例：  
`<p>这是小于号：&lt; 这是大于号：&gt; 这是双引号&quot;&quot; 这是单引号&apos; 这是我也不知道叫什么：&amp;</p>`

# HTML布局(暂且不知用途)
| 标签 | 解释 |
| :-----| :---- |
| `<main>` | 存放每个页面独有的内容。每个页面上只能用一次`<main>`，且直接位于 `<body>` 中。最好不要把它嵌套进其它元素。 |
| `<article>` | 包围的内容即一篇文章，与页面其它部分无关（比如一篇博文）。 |
| `<section>` | 与 `<article>` 类似，但 `<section>` 更适用于组织页面使其按功能（比如迷你地图、一组文章标题和摘要）分块。一般的最佳用法是：以 标题 作为开头；也可以把一篇 `<article>` 分成若干部分并分别置于不同的 `<section>` 中，也可以把一个区段 `<section>` 分成若干部分并分别置于不同的 `<article>` 中，取决于上下文。 |
| `<aside>` | 包含一些间接信息（术语条目、作者简介、相关链接，等等）。 |
| `<header>` | 是简介形式的内容。如果它是 `<body>` 的子元素，那么就是网站的全局页眉。如果它是 `<article>` 或`<section>` 的子元素，那么它是这些部分特有的页眉（此 `<header>` 非彼 标题）。 |
| `<nav>` | 包含页面主导航功能。其中不应包含二级链接等内容。 |
| `<footer>` | 包含了页面的页脚部分。 |


# 布尔属性(暂且不知具体用途)
`<input type="text">`//如果加一个 disabled 属性，用户就无法输入。例：`<input type="text" disabled>`

