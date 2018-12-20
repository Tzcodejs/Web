最近的项目遇到了这样的需求：（要求标题部分不管文字多少，都必须两端对齐）

如图：

<img src="../../screenshot/html css/text1.png">

当时也没有多想直接使用'\&ensp;\'进行代替，毕竟产品同学想快一点看到效果，不敢怠慢！不过到第二个页面就傻眼了。

如图：

<img src="../../screenshot/html css/text2.png">

这很明显'\&ensp;\'已经无法满足我了，只好上'\&emsp;\'。

这里简单说下几种空格的区别：

1. '\&nbsp;\' 半角的不断行的空白格

2. '\&ensp;\' 半角的空格

3. '\&emsp;\' 全角的空格

 
页面效果倒是有了，但是后面复盘的时候发现这样的写法一是不灵活（虽然这里是固定内容），二是不够语义化。所以自然想通过css的方式来解决，在text-align中我们可能用到最多的是center属性，还有一个属性是justify（两端对齐），不过页面刷新后并没有（luan）用。其实这里的text-align：justify是可以单独使用的，前提是文本需要超过两行，并且最后一行不会两端对齐。

因此我们需要借助一个空标签span。

html:
```html
<div>职务：<span></span></div>  
```

css:
```css
div{
  width:200px;
  text-align: justify;
}
div span{
  display:inline-block;
  width:100%;
}
```
这里最完美的做法是使用::after伪元素代替空标签。

PS：后面查阅资料发现text-align-last: justify;可以实现最后一行两端对齐，但似乎兼容性很差（Safari不支持）
<img src="../../screenshot/html css/text3.png">
