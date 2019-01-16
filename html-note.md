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

* head 元素中添加网站icon图标， ``` <link ref="icon" href="favicon.icon" > ```

* 引入外部的css文件

* 引入外部的script文件，其实并不建议在head中引入script文件，一般的做法是在body的最后面引入script，这样可以保证在执行脚本的时候，页面元素都是已经加载好的。

* 在html跟元素中设置属性lang 来比较基本的语言，这对搜索引擎是友好的。



