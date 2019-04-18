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

