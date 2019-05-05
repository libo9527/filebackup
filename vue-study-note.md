## Vue 学习笔记

### 表单

#### Vue 原生表单练习

给定一个表单，包含三个字段，其中两个是必填项。

```html
<form id="app" @submit="checkForm" action="https://vuejs.org/" method="post">
```

action 和 method 是必填项。

@submit 是 v-on:submit 的简写

#### Vue + Element 表单练习




Vue 里的style标签的scoped属性表示局部样式



组件挂载、更新、销毁等时刻所出发的方法称为生命周期函数，vue官网叫生命周期钩子。

Es6 方法的简写

```js
fun: function(){}

fun(){}
```





时间对象的作用

- 获取DOM节点

  ```js
  e.srcElement
  ```

- 获取自定义属性

  ```js
  e.srcElement.dataset.自定义的属性名
  ```



试着用vue实现[todolist](<http://www.todolist.cn/>)



### [JavaScript *splice*() *方法*](http://www.baidu.com/link?url=DGvtusq4T51oKWHx6QZuTNpyNzVq4Ododem0zh7n2yleQxASF5PTnpnPKzO3N7IfUvSxzFIrGUwApcsbMAWcQa)



keyup/keydown 键盘弹起/按下事件

e.keycode，按键代码，回车的代号是13



自定义方法需要写在methods里面，生命周期函数与methods同级



缓存数据

```js
localStorage.setItem('list', JSON.stringify(this.list))
```



在生命周期函数mounted中读取缓存。mounted表示每次刷新将触发的方法。

```js
mounted(){
  var list = JSON.parse(localStorage.getItem('list'));
  if(list){
    this.list = list;
  }                      
}
```


Vue-resource 是官方提供的一个插件，用来请求数据。

npm install vue-resource --save

save 会将依赖写入package.json

安装好之后需要在main.js文件中加入：

```js
import VueResource from 'vue-resource';
Vue.use(VueResource);
```





使用箭头函数，函数里的this指向的就是实例，如果没有使用箭头函数，需要在外面定义一个that来指向实例。



使用第三方插件axios请求数据时的步骤：

1. 安装
2. 在那个组件中使用在哪儿引入



Element UI 和 Mint UI 是饿了么开发的 vue 组件库。Element UI 是 PC 端，Mint UI 是移动端。

组件不会用可以看官方的文档，也可以看其GitHub上的examples。



Vuex 是为了解决不同组件之间的数据共享及持久化





V-cloak 能够解决插值表达式闪烁的问题。

V-text 默认没有闪烁问题

v-text 会覆盖元素原本内容，二差值表达式前后可加其他内容



v-bind 用于绑定属性，v-bind 可以绑定合法的js表达式



js定时器

setInterval() 开启一个定时器并返回定时器id

clearInterval(id) 停止对应ID的定时器



时间修饰符

.stop 阻止冒泡（嵌套元素的事件会从内到外冒泡）

.prevent 阻止默认事件

.capture 添加事件监听器时使用事件捕获模式

.self 只有当事件在该元素本身触发时才触发回调

.once 事件只触发一次



.stop 和 .self 都可以阻止冒泡，区别在于 stop 阻止所有的冒泡，而self 只阻止自己的。



能与用户进行交互的元素：表单元素



V-bind 只能实现数据的单向绑定，从 M 到 V到绑定

v-model 只能用于表单元素中



Js parseInt函数

js eval 函数



vue中对象的属性可以带引号，也可以不带引号，如果属性中有特殊字符，则需要加引号。

Js 对象就是无序键值对的集合



vue中遍历数组或者对象时，索引一般都在后面。

```js
v-for="(item, i) in list"

v-for="(val, key, i) in object"
```

使用 v-for 迭代数字的时候起始值是1

```js
v-for="count in 10"
```

在组件中使用 v-for 时一般都要指定 key 属性，以 v-bind 属性绑定的方式指定key



Js 数组的push和unshift函数

push 尾部添加，unshift 头部添加



v-if 每次都会删除或者创建元素，v-show 只是切换元素的 display: none 样式，不回进行 DOM 操作