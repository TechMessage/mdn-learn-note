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
> 元素可以拥有属性，属性包含了你不想展示给实际内容的部分，例如class属性可以给这个元素加上标识符，用来定位查找到这个元素。有些属性只有属性名没有属性值，这种属性是属于boolean类型的属性，