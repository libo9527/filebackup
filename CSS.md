## CSS

### 组合选择器

> [组合器和多个选择器- 学习Web 开发| MDN](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors)

| 名称           | 组合器 | 选择                                                         |
| :------------- | :----- | :----------------------------------------------------------- |
| 选择器组       | A,B    | 匹配满足A（和/或）B的任意元素（参见下方 [同一规则集上的多个选择器](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors#同一规则集上的多个选择器)）. |
| 后代选择器     | A B    | 匹配B元素，满足条件：B是A的后代结点（B是A的子节点，或者A的子节点的子节点） |
| 子选择器       | A > B  | 匹配B元素，满足条件：B是A的直接子节点                        |
| 相邻兄弟选择器 | A + B  | 匹配B元素，满足条件：B是A的下一个兄弟节点（AB有相同的父结点，并且B紧跟在A的后面） |
| 通用兄弟选择器 | A ~ B  | 匹配B元素，满足条件：B是A之后的任意一个兄弟节点（AB有相同的父节点，B在A之后，但不一定是紧挨着A） |

### 布局

> [Flex 布局教程：语法篇- 阮一峰的网络日志](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)
>
> [Flex 布局教程：实例篇- 阮一峰的网络日志](http://www.ruanyifeng.com/blog/2015/07/flex-examples.html)

### 虚线

> [html+css画虚线，实线](<http://www.voidcn.com/article/p-mocvaqvp-bga.html>)

### 圆角边框

在 CSS2 中添加圆角矩形需要技巧。我们必须为每个圆角使用不同的图片。在 CSS3 中，创建圆角是非常容易的。在 CSS3 中，border-radius 属性用于创建圆角：

向 div 元素添加圆角：

```css
div {
  border:2px solid;
  border-radius:25px;
  -moz-border-radius:25px; /* Old Firefox */
}
```

其中：border:2px solid; solid是实线的意思

### 盒模型（Box model）

盒模型主要定义四个区域：内容 (content)、内边距 (padding)、边框 (border) 和外边距 (margin)。

![](https://images0.cnblogs.com/blog/270324/201402/191935386296017.jpg)

#### 边距

##### Margin

定义：margin 称为边界，是指元素边框之外的空间。

使用时机：

- border 外侧添加空白

- 空白处不需要背景色

- 相邻盒子之间的空白，需要能够相互抵消时

  例如上面的盒子的下边界为 15px，下面的盒子的上边界为 20px，合起来后上下盒子之间的距离为 20px，即 15px + 20px = 20px

##### Padding

定义：padding 称为内边距，是指边框与正文之间的空间，CSS 权威指南中形象的将其称为 “留白”。

使用时机：

- border 内侧添加空白

- 空白处需要背景色

- 相邻盒子之间的空白，需要相互累加时

  例如上面的盒子的下内边距为 15px，下面的盒子的上内边距为 20px，合起来后上下盒子之间的距离为 35px，即 15px + 20px = 35px

##### 属性

margin 和 padding 都包含上、 右、下、左四个方向的属性，即 margin-top、margin-right、margin-bottom、margin-left 或者 padding-top、padding-right、padding-bottom、padding-left。

对于 margin 和 padding  的赋值可以分别制定 1 - 4 个值，分别代表不同的含义。

1. 一个值：代表四个方向的距离均为该值
2. 两个值：第一个值代表上下的距离，第二个值代表左右的距离
3. 三个值：分别代表 “上，左右， 下” 的距离
4. 四个值：按照**顺时针**方向 “上，右，下，左” 的距离

## 教程

> [Learn to Code HTML & CSS](<https://learn.shayhowe.com/>)
>
> [学习CSS布局](https://zh.learnlayout.com/)

