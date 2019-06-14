## JavaScript

### == 与 ===

=== 会进行先强制类型转换，之后再进行比较

### 数组合并

> [Array.prototype.concat() - MDN - Mozilla](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)

```js
var array1 = ['a', 'b', 'c'];
var array2 = ['d', 'e', 'f'];

console.log(array1.concat(array2));
// expected output: Array ["a", "b", "c", "d", "e", "f"]
```

### Map 和 Set

> [Map和Set - 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000/0014345007434430758e3ac6e1b44b1865178e7aff9082e000)

### async

> [async 函数的含义和用法- 阮一峰的网络日志](http://www.ruanyifeng.com/blog/2015/05/async.html)
>
> [async 函数- ECMAScript 6入门](http://es6.ruanyifeng.com/#docs/async)
>
> [async function - MDN - Mozilla](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/async_function)
>
> [await - MDN - Mozilla](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/await)

`await`  操作符用于等待一个[`Promise`](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise) 对象。它只能在异步函数 [`async function`](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/async_function) 中使用。

### 数组遍历

> [JavaScript 数组遍历方法的对比- 掘金](https://juejin.im/post/5a3a59e7518825698e72376b)

