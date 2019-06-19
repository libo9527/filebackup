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



vue的模版语法（即插值表达式，v-text，v-html等）中都是一个js表达式



计算属性有缓存的功能，即计算属性其实是可以用方法的方式来实现相同的功能，但当其他属性值改变时，页面重新渲染，此时方法会重新执行一次，但计算属性只有当其涉及到的属性发生变化时才会重新执行，其他属性变化所导致的页面重新渲染并不会导致计算属性的重新计算！

### 插槽

**插槽，也就是 slot，是组件的一块 HTML 模板，这块模板显示不显示、以及怎样显示由父组件来决定。但是插槽显示的位置却由子组件自身决定，slot写在组件template的什么位置，父组件传过来的模板将来就显示在什么位置。**

#### 作用域插槽

官方叫作用域插槽，实际上，对比匿名/具名插槽，我们可以叫它带数据的插槽。

### 组件

vue 组件分为全局组件和局部组件，全局组件使用 `Vue.component()` 方法注册，局部组件使用 vue 实例的 `compoments` 属性注册。

### props

> [vue props监听变化的几种方式](<https://www.jianshu.com/p/ff708a773dc0>)

prop默认是单向绑定：当父组件的属性变化时，将传递给子组件，但是反过来则不会传递。

可以使用`.sync`显式地指定双向绑定，这使得子组件的数据修改会回传给父组件。

```vue
<child-component v-bind:my-name.sync="name" v-bind:my-age.sync="age"></child-component>
```

可以使用`.once`显式地指定单次绑定，单次绑定在建立之后不会同步之后的变化，这意味着即使父组件修改了数据，也不会传递给子组件。

```vue
<my-component v-bind:my-name.once="name" v-bind:my-age.once="age"></my-component>
```

**注意：2.3.0版本将 v-bind 的 .once 和 .sync 修饰符移除了**

> [v-bind 的 .once和.sync 修饰符](https://cn.vuejs.org/v2/guide/migration.html#v-bind-的-once和-sync-修饰符-移除)
>
> Props 现在只能单向传递。为了对父组件产生反向影响，子组件需要显式地传递一个事件而不是依赖于隐式地双向绑定。

### 路由

//所有权限通用路由表
//如首页和登录页和一些不用权限的公用页面
export const constantRouterMap



//异步挂载的路由
//动态需要根据权限加载的路由表
export const asyncRouterMap

### 引入 Font-Awesome

> [Vue 第三方字体图标引入 Font Awesome](<https://blog.csdn.net/qq_27868533/article/details/79638725>)

1. npm 安装 font-awesome

   ```shell
   npm install font-awesome --save-dev
   ```

2. main.js 中引入 font-awesome

   ```shell
   import 'font-awesome/scss/font-awesome.scss'
   ```

3. 组件中使用 font-awesome

   ```vue
   <i class="fa fa-plus"></i>
   ```

### 使用 iconfont

> [在vue项目中引入iconfont字体图标]([https://hehuiyun.github.io/2018/01/22/%E5%9C%A8vue%E9%A1%B9%E7%9B%AE%E4%B8%AD%E5%BC%95%E5%85%A5iconfont%E5%AD%97%E4%BD%93%E5%9B%BE%E6%A0%87/](https://hehuiyun.github.io/2018/01/22/在vue项目中引入iconfont字体图标/))

1. [官网](www.iconfont.cn)注册

2. 新建项目，添加图标到项目

3. 在项目的 index.html 中引入 iconfont 的在线链接

   ```html
   <link rel="stylesheet" href="//at.alicdn.com/t/font_1243237_q38qtx4df3.css">
   ```

4. 组件中使用

   ```vue
   <i class="iconfont iconDollar"></i>
   ```


### Vue 项目中使用 Sass

1. 安装 Sass 依赖

   ```shell
   npm install --save-dev sass-loader
   //sass-loader依赖于node-sass
   npm install --save-dev node-sass
   ```

Sass

