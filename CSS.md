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



## 教程

> [Learn to Code HTML & CSS](<https://learn.shayhowe.com/>)
>
> [学习CSS布局](https://zh.learnlayout.com/)

