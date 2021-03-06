# mdn - learn -note

## Getting started with html
[html概念](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)

---
html基本概念，基本术语的介绍，元素的结构，页面的结构 

---

### html的概念

> html全称 (hypertext markup language) 是一种标记语言，并不是一种编程语言，它的作用就是告诉浏览器如何去组织web页面给用户展示。元素*element*包含三个部分 *opening tap* 开始标签 *content*(内容) *closing tag*闭合标签，这3部分组成了一个元素**element** 


* 嵌套的元素

> 元素之间是可相互嵌套来组织页面 
* 块元素，行内元素 block & inline
   * 块级元素在页面上形成了一个可视的区块visible block,它会独占一行，它不应该被嵌套在行内元素中，是可以嵌套在块级元素中
   * 行内元素一般是包含在块级元素中，不会独占一行
* 空元素
   * 并不是所有的元素都包含开始标签，内容，闭合标签，有些元素仅仅包含一个开始标签，这些元素是为了插入或者嵌入外部的资源到页面中。例如img标签是在标签的位置上为了嵌入一张图片到页面位置上

### 属性 attribute
> 元素可以拥有属性，属性包含了你不想展示给实际内容的部分，例如class属性可以给这个元素加上标识符，用来定位查找到这个元素。有些属性只有属性名没有属性值，这种属性是属于boolean类型的属性。标签属性值通常是需要使用单引号或者双引号包起来的。单引号或者双引号都是允许的，个人建议使用双引号，里面也可以嵌入单引号字符。

### html document HTML文档
> html文档是由各个元素组成的，格式是相对固定的。举例
* ```<!DOCTYPE html>``` 标识文档类型，在混乱的年代，当html还刚刚产生不就的时候，doctype 是用来设定一组规则，html页面必须遵守这些规则，这样做的目的是为了减少页面的错误以及其他一些的作用。 现在的话，没人在关心这个问题, ```<!DOCTYPE html>```是一种简写形式，这种现在浏览器就可以认为是一种有效的doctype

* html元素是包裹了所有的页面的内容，被认为是**根元素**

* head元素可以看做是一个容器，用来包裹那些你不希望展示给用户看到的内容。包括的东西例如关键字、keywords 页面描述description 这些信息是为了给搜索引擎来识别页面的。

* title元素是用来设置你的页面的标题的，这个标题是显示在浏览器页面标签上的

* body元素是包含所有的内容，这些内容是你想展示给用户的内容的。

* white space 空格，在元素内容中添加多个空格时，在浏览器渲染页面的时候只会渲染一个空格。

* 特殊符号的引用，```< >, ' '' & ```这些符号都是特殊符号，需要转义表示，以及一些特殊符号。```< &lt >&gt```


## HTML介绍
[html介绍](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)

---
> 当页面在浏览器中加载的时候，html文档的头部是不会在页面上展示的。head元素就是html的头部，它的职责就是描述该html文档的的元信息metadata

### head 元素的主要内容

* ```<title>```元素，title元素表示的是整个html文档的标题，而不是局限于页面展示的内容中的h1标题内容

* meta元素，metadata是描述数据的数据，是元数据。html有一个官方的方式来给文档添加元数据，通过meta元素,这些元素是放置到head元素中的。

* 指定html的编码 ``` <meta charset="utf-8"> ```

* 添加html作者和描述 ``` <meta name="author"  content="chris mills"> ```

* ``` <meta name="description" content="sdfadfadsfadfcxfadfzcxfaijfoqerfqpoiwejr">  ```

* head 元素中添加网站icon图标， ``` <link ref="icon" href="favicon.icon" > ```

* 引入外部的css文件

* 引入外部的script文件，其实并不建议在head中引入script文件，一般的做法是在body的最后面引入script，这样可以保证在执行脚本的时候，页面元素都是已经加载好的。

* 在html跟元素中设置属性lang 来比较基本的语言，这对搜索引擎是友好的。


## HTML text fundamentas
[htmlm 文本结构](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

---
> html的其中一大职责就是提供文本接口和语义化，这样浏览器可以正确的显示

* 大多数的结构化的文本都包含标题和段落，例如新闻，杂志...

* h1元素作为页面的顶级标题，一般只会出现一次, h2一般是某个段落的标题，h3作为h2的子标题，层级顺序不能问题

* 为何需要结构化文本？
   * 用户需要通过标题快速定位感兴趣的内容 标题 + 内容
   * 搜索引擎会根据标题元素来建立网页索引 标题
   * 屏幕阅读器的友好 标题
   * css以及js的应用丰富视觉和交互，需要元素包裹内容

* 为何需要语义化？ why we need semantics?
   * 语义化是为了更好的理解页面的内容

## creating hyperlinks
[超链接](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)

> 超链接是非常重要的，web之所以成为web是因为超链接的存在

* 什么是超链接？
> 超链接是web最激动人心的创新，自从有web开始就具备这个特性
* 超链接的内容
> a元素，href属性就是超链接对应的地址，  title属性可以是链接地址的描述信息, a元素内是可以包含其他元素的，例如图片，那么就是图片链接， 或者是按钮
* 链接到特定的页面的特定片段
> a元素的href属性值是url地址，后面你可以跟#para,这样就可以点击链接的时候直接定位到链接地址对应的页面的内容，显示出id值为para的地方
* 绝对地址和相对地址
> 相对地址是相对于该文件的位置，如果文件目录发生改变，链接有可能是会失效的，需要注意的。

### 最佳实践 best 
* 尽量使用相对路径，特别是同一个网站的不同页面时，建议使用相对路径
* 当使用链接来执行一个可下载的资源时，可以使用download属性来执行下载资源的默认名

* 当给某个email地址添加超链接的时候，用户点击后直接打开email而不是一个网址，这时可以给href属性值设置mailto:xxxx@gmail.com 这种协议的方式，事实上如果仅仅写mailto:忽略email地址的话，点击之后也会打开email工具，只不过不会自动将收件人地址填充，这样方式一般用来处理页面的分享时，用户点击之后，跳转到email工具。

* 在网页中嵌入图片，通常是有img元素或者使用css的background-image属性来实现，后者用来做一些图标的非语义化的事情

* 如果引入的图片对于页面的内容是有语义的，建议使用img元素， 如果是做一些图标类的装饰作用的话，建议使用background-image 属性

## 页面中嵌入多媒体
[多媒体](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)
> 在页面中加入音频和视频是通过多媒体的元素audio和video实现的，在web发展的早期，那时候网路带宽不足以加载音频视频等资源，html原生也不支持这些资源的载入，那么都是通过第三方的技术像是flash来解决多媒体的的嵌入，当时flash有很多的缺点包括不能兼容css样式，安全问题等等
* 随着html5的到来，html原生就支持了多媒体资源的嵌入，audio和video元素的以及相应的api都可以很好的支持多媒体在页面中的嵌入问题。

* video元素的使用方法
   * video元素是用来载入视频文件的，那么通常都会在video的内容中使用source来引入文件，src是地址，type是Mime类型，type对于浏览器是重要的，浏览器直接读取type类型就能判断是否支持该类型的文件，如果不支持就走下一个source，这样可以提高页面效率，应该加上type属性
   * video元素的重要属性，controls是表示进度条等视频控制条。
   * width  heigth 这是控制video元素的宽和高，当然也可以使用css来写，但是需要注意的是载入的视频资源本身是有长宽比的aspect ratio, 如果设置的长宽比和视屏自身的长宽比不符合的话，那么视屏就会拉伸，保证长度方向填满，宽度方向保持自身的比例，如果不能填满整个video元素，空的地方就是黑色背景
   * autoplay 属性是在页面一打开的时候就加载视频并且播放，最好不要使用autoplay属性
   * loop 属性是控制视频循环播放的属性
   * muted 静音属性，视屏会静音
   * poster 属性将视频画面直接展现为video的上画面
   * preload 预加载，当视频文件比较大的时候可以使用

* iframe embed object元素用来在页面中嵌入其他的资源，不局限于多媒体资源
   * iframe元素被用来在当前页面中嵌入其他的页面中，基本属性
   * allowfullscreen 允许全屏

* ifame的安全问题
   * 由于iframe可以嵌入别的网页，那么一些用心不良的人会将一些敏感的页面嵌入到自己设计的页面中伪装成真的，从而获取到用户的敏感数据那么应该如何解决这个安全问题呢，可以通过设置让自己的网站不能被别人的网页嵌入。
   * 同时如果在自己的页面中嵌入别人的网页，也会涉及到版权的问题


* 矢量图是某些情况下非常有效，它文件体积小，高度可缩放不失真
   * 在web网页中的图像大致分为像素图片和矢量图片
   * 像素图片是通过像素点形成的，每个像素点代表一个颜色，组成一个图片，常见的格式有.bmp, .png, .jpg, .gif
   * 矢量图是通过算法形成的，包含形状和路径定义，计算机可以通过这些来计算出它的实际显示的图像， svg就是其中一种矢量图

### what is svg? 什么是svg
> svg 是基于xml定义的矢量图，它也是标记语言和html类似

* 响应式图片 responsive images



## 


