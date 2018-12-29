## 常见块级元素

```html

  <div></div> 
  <!-- 块标签 -->

  <p></p>  
  <!-- 段落 -->

  <h1></h1>  
  <!-- 标题一级 -->

  <h2></h2>  
  <!-- 标题二级 -->

  <h3></h3>  
  <!-- 标题三级 -->

  <h4></h4>  
  <!-- 标题四级 -->

  <h5></h5>  
  <!-- 标题五级 -->

  <h6></h6>  
  <!-- 标题六级 -->

  <ul></ul>  
  <!-- 无序列表 -->

  <ol></ol>  
  <!-- 有序列表 -->

  <dl></dl>  
  <!-- 定义列表 -->

  <hr>  
  <!-- 水平分割线 -->

  <table></table>  
  <!-- 表格 -->

  <form></form>
  <!-- 表单 -->
```
**H5 新增块元素**

```html

<!-- 主要是提高页面语义化 -->

  <header></header>

  <nav></nav>

  <section></section>

  <article></article>

  <aside></aside>

  <footer></footer>

```
## 常见行内元素

```html
  <span></span>

  <a></a>

  <img />  
  <!-- 图片 -->

  <br> 
  <!-- 换行 -->

  <b></b>  
  <!-- 加粗 -->

  <strong></strong>  
  <!-- 加粗 -->

  <sup></sup>  
  <!-- 上标 -->

  <sub></sub>  
  <!-- 下标 -->

  <i></i>  
  <!-- 斜体 -->

  <em></em>  
  <!-- 斜体 -->

  <del></del>  
  <!-- 删除线 -->

  <u></u>  
  <!-- 下划线 -->

  <input>
  <!-- 文本框 -->

  <textarea></textarea>  
  <!-- 多行文本 -->

  <select></select>  
  <!-- 下拉列表 -->

```

## 块级元素与行内元素区别

1. 块级元素会独占一行，默认情况下，其宽度自动填满其父元素宽度。

2. 行内元素不会独占一行，相邻的行内元素会排列在同一行里，直到一行排不下才会换行，其宽度随元素的内容而变化。

3. 块级元素可以设置width，height属性。

4. 行内元素设置width，height属性无效，它的长度高度主要根据内容决定。

5. 块级元素即使设置了宽度，仍然是独占一行。

6. 块级元素可以设置margin和padding属性。

7. 行内元素水平方向的padding-left，padding-right，margin-left，margin-right都会起效果，但竖直方向的padding-top，padding-bottom，margin-top，margin-bottom却不会产生效果。

8. 行内元素padding-top，padding-bottom从浏览器显示的效果上是增加的，但并不会对他周围的元素产生任何影响。
