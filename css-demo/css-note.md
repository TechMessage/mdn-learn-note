## css - cascading stylesheet 层叠式样式
> html用来定义页面的结构和内容，css用来装饰和布局

### css 选择器
1. simple selector 简单选择器
   1. id选择器
   2. 类选择器
   3. 元素元素器
2. attribute selectors 属性选择器
3. pseudo-classes  伪类选择器
4. pseudo-elements 伪元素选择器
5. combinators:  交集选择器
6. multiple selectors 并集选择器
7. * 通配符选择器 通配符选择器是选择所有的元素(基本没啥用)


### 伪元素
* ::after
* ::before
* ::first-letter
* ::first-line
* ::selection
* ::backdrop

### 交集选择器
* 后代选择器 A B
* 子代选择器 A > B
* 直接兄弟选择器 A + B
* 一般兄弟选择器 A ~ B


### css中属性值的单位问题
* 数字类的值  长度
* 百分比值
* 颜色值
* 简单函数

### 1em的大小
* 1em 是当前元素的font-size的大小(宽度值)，浏览器给页面设置的默认字体大小是16px，意味着1em的默认大小是16px。

* 字体大小是可以继承的，如果是父元素设置了字体大小，那么子元素将继承父元素的大小，1em的大小就会发生改变。

* em 也是最常用的相对单位

### rem大小

* rem 单位在 ie678不兼容
* rem 是相对单位，相对的是根元素html的字体大小
* vw vh相对单位，是把视口大小平分100份，使用没有em常用
* 值为0的时候，可以省略单位

### line-height
* 对于行高的值，如果不适用单位时，是相对于当前字体的大小。例如font-size:16px, line-height:1.5; 1.5倍的字体大小

* a 元素的默认颜色是蓝色，它是浏览器的默认样式，不会继承父元素的颜色，这是特殊情况。


### box model 盒子模型
> 盒子模式是网页布局的基础，每个元素被一个方盒子来表示，包含内容，内边距，边框， 外边距组成了一个整体。
* overflow
* background-clip
* outline

### style text  文字样式

* font-family












