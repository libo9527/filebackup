Idea 快捷键：

代码移动：shift + command + ↑/↓

快速复制：command + d



Background 属性是设置背景图片的，bgcolor 是设置背景颜色的。



<a> 标签的target属性规定在何处打开链接，默认为self（在当前页面打开），_blank 是在新标签页打开



HTML 格式化

| 标签     | 描述                 |
| -------- | -------------------- |
| `<b>`    | 粗体                 |
| `<big>`  | 大号字（H5中已废除） |
| `<em>`   | 着重文字             |
| `i`      | 斜体                 |
| `small`  | 小号字               |
| `strong` | 加重语气             |
| `sub`    | 下标字               |
| `sup`    | 上标字               |
| `ins`    | 插入字               |
| `<del`   | 删除字               |

<body>

<p>普通文字</p>
<p>
    <b>粗体</b>
</p>
<p>
    <big>大号字（H5中已废除）</big>
</p>
<p>
    <em>着重文字</em>
</p>
<p>
    <i>斜体</i>
</p>
<p>
    <small>小号字</small>
</p>
<p>
    <strong>加重语气</strong>
</p>
<p>
    aaa<sub>下标字</sub>bbb
</p>
<p>
    aaa<sup>上标字</sup>bbb
</p>
<p>
    <ins>插入字</ins>
</p>
<p>
    <del>删除字</del>
</p>

</body>



三种样式表插入方式

1. 外部样式表

   ```html
   <link rel="stylesheet" type="text/css" href="mystyle.css">
   ```

2. 内部样式表

   ```html
   <style type="text/css">
       p{
           color: aqua;
       }
   </style>
   ```

3. 内联样式表

   ```html
   <p style="color: aqua;">内联样式表</p>
   ```



文档内跳转

```html
<a name="tips">hello</a>

<a href="#tips">跳转到hello</a>
```



表格

1. 单元格边距：使用 cellpadding 属性

   ```html
   <table border="1" cellpadding="10px">
       <tr>
           <td>单元格1</td>
           <td>单元格2</td>
           <td>单元格3</td>
       </tr>
   </table>
   ```

2. 单元格间距：使用 cellspacing 属性

   ```html
   <table border="1" cellspacing="10px">
       <tr>
           <td>单元格1</td>
           <td>单元格2</td>
           <td>单元格3</td>
       </tr>
   </table>
   ```

   

列表

1. 无需列表

   使用标签： `<ul>`, `<li>`

   属性/样式：实心圆 disc，空心圆 circle，方块 square

2. 有序列表：`<ol> <li>`

   使用标签： `<ol>`, `<li>`

   属性/样式：A，a，I，i，指定从几开始 start

3. 嵌套列表

4. 自定义列表

   使用标签： `<dl>`, `<dt>`, `<dd>`



HTML 块

1. HTML 块元素

   块元素通常会以新行开始

   如：`<h1>`, `<p>`, `<ul>`

2. HTML 内联元素

   内联元素通常不会以新行开始

   如：`<b>`, `<a>`, `<img>`

3. HTML `<div>` 元素

   `<div>` 也被称为块元素，其主要是组合 HTML 元素的容器

4. HTML `<span>` 元素

   `<span>` 元素是内联元素，可作为文本的容器



H5 布局

1. div 布局
2. table 布局



H5 表单

- 单选框中的 name 属性是为了把 name 相同的元素绑定到一组，从而实现单选的功能。

  ```html
  性别：
  <input type="radio" name="sex">男
  <input type="radio" name="sex">女
  ```



XAMPP

XAMPP是相对LAMP而言的，而LAMP就是所谓的Linux+Apache+MySQL+PHP黄金组合，X代表通用系统，目前包括LINUX系统（在 Ubuntu、SuSE、RedHat、Mandrake 和 Debian 下通过测试），Windows系统（在Windows 98、NT、2000、2003、XP 和 Vista通过测试），Solaris系统（在 Solaris 8 环境下开发并测试），Mac OS X系统等。

[Mac XAMPP 7.2.0 htdocs文件夹](https://blog.csdn.net/ZY_FlyWay/article/details/79084468)



HTML框架（除了内联框架意外均已过时）

1. 框架标签(`<frame>`)
2. 框架集标签(`<frameset>`)
3. 常用标签
4. 内联框架(`<iframe>`)



HTML背景

1. 背景标签

   Background 指定图片

2. 背景颜色

   Bgcolor 指定颜色



HTML实体

html实体就是只html中的预留字符的替代编号，例如：`<`, `>`, `&`等

想要在页面中显示这些字符需要用实体代替。

[HTML 字符实体 - W3School 在线教程](http://www.w3school.com.cn/html/html_entities.asp)



XHTML 就是规范化的 HTML



H5与H4的区别

H5新增的属性

- 全局属性
  - contentEditable

    内容可编辑

    ```html
    <ul contenteditable>
        <li>l1</li>
        <li>l2</li>
        <li>l3</li>
    </ul>
    ```

  - tabIndex

    指定页按tab时的访问顺序

    默认只有表单元素和链接元素可以获取焦点

    ```html
    <p>按 tab 时的访问顺序是 a1 - a3 - a2</p>
    <a href="#" tabindex="1">a1</a>
    <a href="#" tabindex="3">a2</a>
    <a href="#" tabindex="2">a3</a>
    ```



H5 新增的主体结构元素

1. `<article>`

2. `<section>`

   一般 Section 需要一个标题

3. `<nav>`

4. `<aside>`

5. Time 与微格式



H5 新增的非主体结构元素

1. `<header>`
2. `<footer>`
3. `<hgroup>`
4. `<address>`



表单新增元素与属性

1. form属性
2. formaction属性
3. formmathod属性
4. formenctype属性
5. formtarget属性
6. autofocus属性
7. required属性
8. labels属性
9. 标签的control属性
10. 文本框的placeholder属性
11. 文本框的list属性
12. 文本框的autocomplete属性
13. 文本框的pattern属性
14. 文本框的selectionDirection属性
15. 复选框的indeterminate属性
16. image提交按钮的height属性与width属性