## CSS 之 position

> [position - CSS（层叠样式表） | MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/position)
>
> [CSS中position属性( absolute | relative | static | fixed )详解](https://blog.csdn.net/chen_zw/article/details/8741365)

CSS position属性用于指定一个元素在文档中的定位方式。top，right，bottom 和 left 属性则决定了该元素的最终位置。

### 相关概念

- 文档流

  即按照自上而下，从左至右的顺序排放元素。

### 取值

- `static`

  position 的默认值，该关键字指定元素使用正常的布局行为，即元素在文档流中位置。此时 `top`, `right`, `bottom`, `left` 和 `z-index `属性无效。

- `relative`

  该关键字下，元素先放置在未添加定位时的位置，再根据 top，right 等属性调整元素位置（因此会在此元素未添加定位时所在位置留下空白）。

  - 相对定位没有脱离文档流，遵循正常的文档流，相对的是它原本在文档流中的位置而进行的偏移。但是它的 top/left/right/bottom 属性是生效的，可以说它是 static 到 absoult 的一个中间过渡属性
  - 它还占有文档空间，而且占据的文档空间不会随 top / right / left / bottom 等属性的偏移而发生变动
  - margin / padding 是占据文档空间的。也就是说给相对定位的元素指定 margin / padding 之后是会影响后面的元素位置的。


- `absolute`

  不为元素预留空间，通过指定元素相对于最近的非 static 定位祖先元素的偏移，来确定元素位置。绝对定位的元素可以设置外边距（margins），且不会与其他边距合并。

  - 绝对定位的元素会脱离文档流
  - relative 和 static 方式在最外层时是以 `<body>` 标签为定位原点的，而absoulte方式在无父级是 position非 static定位时是以 `<html>` 作为原点定位。`<html>` 和 `<body>` 元素相差9px左右。
  - 使用 absoulte 或 fixed 定位时，必须指定 left、right、 top、 bottom 属性中的至少一个，否则 left/right/top/bottom 属性会使用它们的默认值 auto，这将导致 absoulte 退变为 relative
  - top 和 bottom 同时存在时只有 top 生效。
  - left 和 right 同时存在时只有 left 生效。
  - absoulte 是根据祖先元素的 border 进行的定位。即祖先元素的 margin 会让子类的 absoulte 跟着偏移，而 padding 却不会让子类的 absoulte 发生偏移。
  - 绝对定位元素在可视区域之外会导致滚动条出现。而放置相对定位元素在可视区域之外，滚动条不会出现。

- fixed

  不为元素预留空间，而是通过指定元素相对于屏幕视口（viewport）的位置来指定元素位置。元素的位置在屏幕滚动时不会改变。打印时，元素会出现在的每页的固定位置。`fixed` 属性会创建新的层叠上下文。

### z-index

z-index 称为层叠顺序属性，用一个整数来定义堆叠的层次。

同级元素间的堆叠，z-index 值越大，则被层叠在越上面，z-index 相等时，将依据它们在HTML文档中流的顺序层叠，后面的将会覆盖前面的。

父子关系是无法用 z-index 来设定上下关系的，一定是子级在上父级在下。