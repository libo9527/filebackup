线上数据库连接信息中的用户名和密码加密了，不知道密钥（盐）

将数据库的用户名和密码进行加密

```java
public static void main(String[] args) {
    BasicTextEncryptor textEncryptor = new BasicTextEncryptor();
    //加密所需的salt(盐)
    textEncryptor.setPassword("G0CvDz7oJn6");
    //要加密的数据（数据库的用户名或密码）
    String username = textEncryptor.encrypt("root");
    String password = textEncryptor.encrypt("root123");
    System.out.println("username:"+username);
    System.out.println("password:"+password);
}
```

输出信息为:

```
username:i8QgEN4uOy2E1rHzrpSTYA==
password:6eaMh/RX5oXUVca9ignvtg==
```



如何从项目源码中查看数据库链接的那个 scheme



[Oracle中TO_DATE格式- D董一点- 博客园](https://www.cnblogs.com/ajian/archive/2009/03/25/1421063.html)



VMware Fusion 11序列号
7HYY8-Z8WWY-F1MAN-ECKNY-LUXYX



[中华人民共和国行政区划（五级）：省级、地级、县级、乡级和村级。](https://www.npmjs.com/package/china-division)



ElementUI, IView... 的级联选择器都不支持远程搜索



[Vue组件的三种调用方式](https://molunerfinn.com/vue-components/#Dialog)



[利用JavaScript在canvas中画一棵树| 吴锴的博客](http://www.wukai.me/2015/10/04/canvas-trees/)



https://segmentfault.com/a/1190000012015667



@RequestMapping("/deal")public class DealController {

@PutMapping(value = "/")

请求时找不到 /deal

改成`@PutMapping(value = "/update")`却可以找到 /deal/update



idea 热部署需重启项目的情况：

- 增加了属性（由于lombok是编译期间添加set/get等的）
- 修改注解时



<https://blog.csdn.net/sps900608/column/info/23911>



<https://juejin.im/post/5c3e9f946fb9a049f06a85ff>



<https://www.jianshu.com/p/76d38bd28fa6>



<https://www.jianshu.com/p/d87d7140944e>



<https://www.zmrenwu.com/courses/vue2x-todo-tutorial/materials/38/>



[手把手构建一个VUE项目](<https://segmentfault.com/a/1190000014409110#articleHeader10>)



[Java中VO、 PO、DO、DTO、 BO、 QO、DAO、POJO的概念 ...](https://www.hollischuang.com/archives/553)



Vue url 不能是 /cd/deal/ 可以是 /cd/deal

然后按RESTFul规范写后端接口



[Oracle dblink详解(转) - sumsen - 博客园](https://www.cnblogs.com/sumsen/archive/2013/03/04/2943471.html)



[Chrome浏览器如何安装&使用Axure RP扩展程序_百度经验](https://jingyan.baidu.com/article/e2284b2b8afad4e2e6118d91.html)



搭建分布式任务调度中心



[分布式定时任务调度系统技术选型--转](https://www.cnblogs.com/davidwang456/p/9057839.html)



<https://blog.csdn.net/sdta25196/article/details/76718617>







[关于如何设置echart图例（legend）的位置- qq_31135027的博客- CSDN ](https://blog.csdn.net/qq_31135027/article/details/79612966)



https://github.com/CntChen/cntchen.github.io/issues/15



popper-options  [popper.js](https://popper.js.org/documentation.html) 的参数 参考 [popper.js](https://popper.js.org/documentation.html) 文档  





<https://blog.csdn.net/Mr_JavaScript/article/details/88604270>

<https://github.com/KBeginner/vue-treeSelect-component>





<https://www.tangshuang.net/3507.html>













设置字体

```
<div align="center" style="font-family: 'San Francisco UI'; color: #909399;">Status</div>
<div align="center">Collecting</div>
```



















![](http://ww1.sinaimg.cn/large/005M2pcYgy1g2qawx3w8pj31ig0ms0z2.jpg)



[关于Java中的Calendar类获取月份- yubo_725 - CSDN博客](https://blog.csdn.net/yubo_725/article/details/41877625)













for-in 语句
一般会使用for-in来遍历对象的属性的,不过属性需要 enumerable,才能被读取到.
for-in 循环只遍历可枚举属性。一般常用来遍历对象，包括非整数类型的名称和继承的那些原型链上面的属性也能被遍历。像 Array和 Object使用内置构造函数所创建的对象都会继承自Object.prototype和String.prototype的不可枚举属性就不能遍历了.



`for-of` 和 `for-in` 的区别

`for-in` 语句以原始插入顺序迭代对象的可枚举属性。`for-in`会把继承链的对象属性都会遍历一遍,所以会更花时间.

`for-of` 语句只遍历可迭代对象的数据。



[JS - 计算两个数组的交集、差集、并集、补集（多种实现方式）](<http://www.hangge.com/blog/cache/detail_1862.html>)



[`Array.prototype.map()`](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/map)



[mybatis oracle两种方式批量插入数据](<https://blog.csdn.net/phantomes/article/details/70761603>)

[Oracle 批量插入数据 Insert All Into]([http://zhoupq.com/Oracle-%E6%89%B9%E9%87%8F%E6%8F%92%E5%85%A5%E6%95%B0%E6%8D%AE-Insert-All-Into/](http://zhoupq.com/Oracle-批量插入数据-Insert-All-Into/))



[oracle查询叶子节点](https://sujunfei.iteye.com/blog/664003)

```xml
<select id="selectLeafNodes" resultMap="globalLocationMap">
    select gl.*
    from GLOBAL_LOCATION gl
    where  CONNECT_BY_ISLEAF = 1
    start with gl.ID = #{locationId}
    connect by prior  gl.ID = gl.PARENT_ID
</select>
```



Mac idea 方法注射：

option + enter



[ORA-02287:此处不允许序号(sequence number not allowed here) 的避免以及强制实现](<https://blog.csdn.net/qq525099302/article/details/43053291>)

```xml
<insert id="batchAdd">
    INSERT INTO COLLECT_TASK (
        ID,
        CITY_ID,
        POPULATION,
        COLLECTOR_ID,
        ALLOCATED_TIME_START,
        ALLOCATED_TIME_END,
        STATUS_ID,
        CREATE_BY,
        CREATE_DATE,
        UPDATE_BY,
        UPDATE_DATE,
        DEL_FLAG,
        COLLECTED_QTY
    )
    select SEQ_COLLECT_TASK.nextval,t.c1,t.c2,t.c3,t.c4,t.c5,t.c6,t.c7,t.c8,t.c9,t.c10,t.c11,t.c12 from (
        <foreach collection="list" item="item" index="index" separator="union all" >
            select
            #{item.cityId} c1,
            #{item.population} c2,
            #{item.collectorId} c3,
            #{item.allocatedTimeStart} c4,
            #{item.allocatedTimeEnd} c5,
            #{item.statusId} c6,
            #{item.createBy} c7,
            #{item.createDate} c8,
            #{item.updateBy} c9,
            #{item.updateDate} c10,
            #{item.delFlag} c11,
            #{item.collectedQty} c12
            from dual
        </foreach>
    ) t
</insert>
```



[oracle排序后获取第一条数据](<https://blog.csdn.net/u010227447/article/details/26134087>)

[Oracle的递归查询详解](http://www.ibloger.net/article/256.html)



字符串数组转Long数组

```java
public static void main(String[] args) {
    String path = ",1,2,3,4,5,";
    List<Long> list = Arrays.stream(path.substring(1, path.length() - 1).split(",")).map(n -> Long.parseLong(n)).collect(Collectors.toList());
    System.out.println(list);
}
```



oracle 是否为叶子节点

```xml
<select id="getLocationNodeListByParentId" resultType="com.sst.cloud.provider.cd.location.vo.LocationTreeNodeVo">
      SELECT CONNECT_BY_ISLEAF AS isLeaf,
      ID,
      PARENT_ID as parentId,
      ENGLISH_NAME as englishName,
      STATUS
      FROM GLOBAL_LOCATION
WHERE PARENT_ID = #{PARENTID}
      START WITH PARENT_ID = #{PARENTID}
      CONNECT BY PARENT_ID = PRIOR ID
ORDER BY ID
  </select>
```

```java
public class LocationTreeNodeVo {

    private Long id;

    private Long parentId;

    private Boolean isLeaf;

    private String englishName;

    private Long collectedQTY;

    private Long status;
}
```

直接用Boolean接收



Css 粗体

```css
.fontclass{
  font-weight: bold;
}
```



[vue非父子组件之间的传值--bus（总线/观察者模式）](<https://my.oschina.net/u/3229305/blog/1820279>)

[vue非父子组件怎么进行通信](https://segmentfault.com/a/1190000008042320)



Vue 组件传值时的时机

传默认值，即首次传的值需要在watch里监听，然后做相应处理。否则获取不到对应值



span默认不像[div](http://www.thinkcss.com/)是块元素，对span使用文字居中[text-align:center](https://www.thinkcss.com/css/1131.shtml)样式，文字内容是无法在span居中的。

[span内文字居中css布局方法_让span内容居中](<https://www.thinkcss.com/jiqiao/1425.shtml>)

[如何让span中的文字垂直居中- Dzq_Boyka的博客- CSDN博客](https://blog.csdn.net/dzq_boyka/article/details/54585435)

[终于搞清楚DIV和SPAN怎么样垂直居中对齐了](<http://zhlwish.blog.sohu.com/19140744.html>)



```html
<div style="height:400px; border:1px #e4e4e4 solid">
  <span style="display:block; text-align: center;line-height: 400px">No Data</span>
</div>
```

`border:1px #e4e4e4 solid`中的solid代表实线



[漂亮的水平分隔線➖，利用 CSS](<http://forever0411.blogspot.com/2017/05/hr.html>)



[/CSS/font](<https://developer.mozilla.org/zh-CN/docs/Web/CSS/font>)



[CSS垂直居中的12种实现方式](<https://juejin.im/post/5a5ca65a6fb9a01ca3254537#heading-6>)

使用flex布局
HTML
```html
<div id="box">test vertical align</div>
```

CSS
```css
#box {
    width: 300px;
    height: 300px;
    background: #ddd;
    display: flex;
    align-items: center;
}
```





webstorm 展开与收起：

全部展开/收起：shift + command `+`

局部展开/收起：option + command `+`





<https://vue-loader.vuejs.org/en/features/scoped-css.html>



[自定义elementui中的图标](<https://www.jianshu.com/p/32251dcf6fca>)



<https://fontawesome.com/v4.7.0/>



CSS——去重叠边框

<https://blog.csdn.net/wzj0808/article/details/51690118>

<https://blog.csdn.net/u013344993/article/details/80081151>



[重新认识vue之事件阻止冒泡](https://segmentfault.com/a/1190000015852875)



[例外的 `!important` 规则](<https://developer.mozilla.org/zh-CN/docs/Web/CSS/Specificity>)

当在一个样式声明中使用一个`!important` 规则时，此声明将覆盖任何其他声明。虽然技术上`!important`与优先级无关，但它与它直接相关。

使用 `!important` 是一个坏习惯，应该尽量避免，因为这破坏了样式表中的固有的级联规则 使得调试找bug变得更加困难了。当两条相互冲突的带有 `!important` 规则的声明被应用到相同的元素上时，拥有更大优先级的声明将会被采用。



[el-select 默认样式问题](<https://github.com/ElemeFE/element/issues/2240>)



[Oracle查询忽略大小写的实现方法](<http://database.51cto.com/art/201010/231561.htm>)



[Window setTimeout() 方法](<http://www.runoob.com/jsref/met-win-settimeout.html>)



[在elementUI中使用 el-autocomplete 实现远程搜索的下拉框](<https://blog.csdn.net/qq_37746973/article/details/78402812>)

autocomplete只识别value字段并在下拉列中显示

| trigger-on-focus | 是否在输入框 focus 时显示建议列表 | boolean | —    | true |
| ---------------- | --------------------------------- | ------- | ---- | ---- |
|                  |                                   |         |      |      |



https://github.com/apache/incubator-echarts/issues/4829#issuecomment-328254135



[Js计算时间差，天数，小时数，余数](https://qiaolevip.iteye.com/blog/1329292)





Mac - navicat 执行选中：command + r



[Java的几个基本类型之间的相互转换| Matt's Blog](https://matt33.com/2015/10/27/TheTransformOfJava/)

```java
location.setStatus((long) GLOBAL_LOCATION_STATUS_ASSIGNED);
```



[es6数组去重（连重复的对象也可以去掉）](<https://juejin.im/post/5b17a2c251882513e9059231>)



js数组倒序reverse





js增加class或者删除class

html5增加了classList

classList 属性返回元素的类名，作为 DOMTokenList 对象。

该属性用于在元素中添加，移除及切换 CSS 类。

classList 属性是只读的，但你可以使用 add() 和 remove() 方法修改它。

增加：document.getElementById("myDIV").classList.add("mystyle", "anotherClass", "thirdClass");

去除：document.getElementById("myDIV").classList.remove("mystyle");



[css3之animation制作闪烁文字效果](<https://blog.csdn.net/alex8046/article/details/52754737>)

[**CSS animations**](<https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Animations/Using_CSS_animations>)

[css3 文字闪烁效果_html实现文字闪烁代码的多种形式](<http://www.fly63.com/article/detial/616>)





[[elementUI tree 懒加载 更新节点](https://segmentfault.com/a/1190000017512508)]

[elementui tree如何重新渲染指定节点及其子节点(懒加载方式)](https://segmentfault.com/q/1010000015680930)

[ElementUI如何展开指定Tree树节点](<https://blog.csdn.net/gaojie_csdn/article/details/80738488>)这种试了没用

el-tree setCurrentKey能干嘛？



[定时器](<https://javascript.ruanyifeng.com/advanced/timer.html>)

JavaScript 提供定时执行代码的功能，叫做定时器（timer），主要由setTimeout()和setInterval()这两个函数来完成。它们向任务队列添加定时任务。

setTimeout和setInterval函数，都返回一个整数值，表示计数器编号。将该整数传入clearTimeout和clearInterval函数，就可以取消对应的定时器。

debounce 函数（防抖动）



[Number.MAX_SAFE_INTEGER](<https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Number/MAX_SAFE_INTEGER>)



[JavaScript 中 Map 与 JSON 转换](<https://www.jianshu.com/p/af4e04cb72bf>)

```js
var map = new Map()
map.set(0, [2])
Cookies.set('location-sort', JSON.stringify(map))
var locationSort = new Map(JSON.parse(Cookies.get('location-sort')))
```



[Access to ES6 array element index inside for-of loop](https://stackoverflow.com/questions/34348937/access-to-es6-array-element-index-inside-for-of-loop)



[如何在 Mac 上强制退出应用](<https://support.apple.com/zh-cn/HT201276>)



Array.prototype.unshift()

**unshift()** 方法将一个或多个元素添加到数组的开头，并返回该数组的新长度。

```
var a = [{id: 1, name: 'a'}, {id: 2, name: 'b'}]
var b = [{id: 3, name: 'c'}, {id: 4, name: 'd'}]
a.unshift(b)
console.log(a)
// (3) [Array(2), {…}, {…}]
// 0: Array(2)
// 0: {id: 3, name: "c"}
// 1: {id: 4, name: "d"}
// length: 2
// __proto__: Array(0)
// 1: {id: 1, name: "a"}
// 2: {id: 2, name: "b"}
// a.unshift({id: 3, name: 'c'}, {id: 4, name: 'd'})
// console.log(a)
// (4) [{…}, {…}, {…}, {…}]
// 0: {id: 3, name: "c"}
// 1: {id: 4, name: "d"}
// 2: {id: 1, name: "a"}
// 3: {id: 2, name: "b"}
```





el-tree调整节点顺序的方法：

通过调整父节点childNodes中子节点的相对位置来改变子节点的顺序。

需要注意的是不能通过remove结合insertBefore的方式来调整顺序，因为romove方法删除节点后就无法再通过getNode方法获取到该节点了

```js
topCheckedNodes () {
  var checkedNodesData = this.$refs.locationTree.getCheckedNodes()
  for (let nodeData of checkedNodesData) {
    this.recursionTop(this.$refs.locationTree.getNode(nodeData.id))
    this.$refs.locationTree.setChecked(nodeData, false, true)
  }
},
recursionTop (node) {
  while (node.parent != null) {
    var parent = node.parent
    if (node !== parent.childNodes[0]) {
      parent.childNodes.splice(parent.childNodes.indexOf(node), 1)
      parent.childNodes.unshift(node)
      // this.swap(parent.childNodes, 0, parent.childNodes.indexOf(node))
      // this.$refs.locationTree.remove(node)
      // parent.childNodes.unshift(node)
    }
    node = parent
  }
}
```



el-tree通过如下方式可动态收起子节点：

```js
this.$refs.locationTree.getNode(7).expanded = false
```



Array.prototype.reverse()

`reverse()` 方法将数组中元素的位置颠倒,并返回该数组。该方法会改变原数组。



删除的对象数组中的某一项：

```js
array.splice(array.indexOf(item), 1)
```

indexOf()方法返回在数组中可以找到一个给定元素的第一个索引，如果不存在，则返回-1。



[js实现交换数组元素位置的方法总汇](<http://www.fly63.com/article/detial/1089>)

可使用splice方法来交换数组的位置，如下：

```
array.splice(index2,1,...array.splice(index1, 1 , array[index2]));
```

array.splice(index1, 1 , array[index2])会将index1位置上的元素替换为index2位置的元素，同时返回[array[index1]]（注意此时返回的是数组，所以在代码中加入了扩展运算符...将数组转为参数序列）。再利用同样的方式将index2位置上的元素替换为被删除的原数组的array[index1]的值。完成交换。



[Why does javascript map function return undefined?](https://stackoverflow.com/questions/16037049/why-does-javascript-map-function-return-undefined)



[Oracle创建序列，删除序列，得到序列的例子](https://www.cnblogs.com/rootq/articles/1089392.html)



[vue中自定义按钮组件为什么要加.native](https://segmentfault.com/q/1010000011186651)

 `.native` 修饰符就是用来注册元素的原生事件而不是组件自定义事件的



[JS阻止冒泡和取消默认事件(默认行为)](http://caibaojian.com/javascript-stoppropagation-preventdefault.html)



[iView - A high quality UI Toolkit based on Vue.js](https://www.iviewui.com/)



[Atom 列编辑](<https://atom.io/packages/Sublime-Style-Column-Selection>)

[如何选择编辑器中的列（Atom，Notepad ++，Kate，VIM，Sublime，Textpad等）和IDE（NetBeans，IntelliJ IDEA，Eclipse，Visual Studio等）](<https://cloud.tencent.com/developer/ask/27877>)



[oracle通过sql获取表结构](<https://blog.csdn.net/u010663021/article/details/77775721>)



[Oracle CHAR，VARCHAR，VARCHAR2,nvarchar类型的区别与使用 ...](https://blog.csdn.net/javaloveiphone/article/details/8155827)

varchar/varchar2

varchar是长度不固定的，比如说，你定义了varchar(20),当你插入abc，则在数据库中只占3个字节。

varchar同样区分中英文，这点同char。

varchar2基本上等同于varchar，它是oracle自己定义的一个非工业标准varchar，不同在于，varchar2用null代替varchar的空字符串

varchar/varchar2适用于长度不固定的，一般不含中文的情况



[Webstorm 文档注释模板及函数代码注释](<https://blog.csdn.net/qq_39108466/article/details/79712547>)



[inner join with group by expression in oracle sql `[duplicate]`](https://stackoverflow.com/questions/15870331/inner-join-with-group-by-expression-in-oracle-sql)

```sql
SELECT
	SG.ID,
	SG.GROUP_NAME,
	SG.DESCRIPTION,
	SG.GROUP_TYPE,
	SG.STATUS,
	COUNT( SGR.STORE_GROUP_ID ) AS MEMBERQTY
FROM
	STORE_GROUP SG
	LEFT JOIN STORE_GROUP_REL SGR ON SG.ID = SGR.STORE_GROUP_ID
GROUP BY
	（ SG.ID,
	SG.GROUP_NAME,
	SG.DESCRIPTION,
	SG.GROUP_TYPE,
	SG.STATUS,
	SGR.STORE_GROUP_ID）
```



chrome 预览 markdown 文件：

使用 Markdown Viewer 插件

```
✚ Local Files

1. Navigate to `chrome://extensions`
2. Locate Markdown Viewer and click on the `DETAILS` button
3. Make sure that the `Allow access to file URLs` switch is turned on
```

需要在设置里允许该插件访问文件网址



[如何使用 Mac 上的“文件共享”进行连接](<https://support.apple.com/zh-cn/HT204445>)



[Vue冲突解决 [Vue warn]: The computed property "fields" is already defined in data.](https://www.jianshu.com/p/63d9540040af)



el-form的表单验证：

1. prop要和v-model绑定的属性名相同。

2. v-model绑定的必须是el-form 所绑定对象下的属性

   ```html
   <el-form ref="form" :model="form" :rules="rules">
   	<el-input v-model="name"></el-input> <!-- wrong -->
     <el-input v-model="form.name"></el-input> <!-- right -->
   </el-form>
   ```

3. `<el-form>` 标签中数据绑定要用 `:model` 不能用 `v-model`

   [vue使用填坑之:model和v-model的区别- baoyadong - 博客园](https://www.cnblogs.com/xuzhudong/p/8617487.html)





.trim
如果要自动过滤用户输入的首尾空白字符，可以给 v-model 添加 trim 修饰符：

`<input v-model.trim="msg">`



```html
<template>
  <el-form ref="assignForm" :model="collectTaskForm" label-width="120px" :rules="assignRules">
    <el-form-item label="Collector:" prop="collector">
      <el-select v-model="collectTaskForm.collector" style="display: block">
        <el-option
                   v-for="item in collectorOptions"
                   :key="item.id"
                   :label="item.name"
                   :value="item.id"
                   >
        </el-option>
      </el-select>
    </el-form-item>
  </el-form>
  <span slot="footer" class="dialog-footer">
    <el-button @click="assignDialog.visible = false">Cancel</el-button>
    <el-button type="primary" @click="assignCollect">Assign</el-button>
  </span>
</template>

<script>
export default {
  data () {
    collectTaskForm: {
        collector: {type: Number}
      }
  }
</script>
```

collector必须初始时就指定Number类型，否则选中option之后不会显示。


Brew 全称为Binary Runtime Environment for Wireless（无线二进制运行环境）。

在Mac os系统中经常使用HomeBrew来安装相关应用

Homebrew到底是什么个东西？

linux系统有个让人头疼的通病，那就是软件包依赖，好在当前主流的两大发行版本都自带了解决方案，Red hat有yum，Ubuntu有apt-get。那么我们用Mac OSx系统怎么办？别担心，这一切Homebrew可以帮你搞定。

Homebrew是一款Mac OS平台下的软件包管理工具，拥有安装、卸载、更新、查看、搜索等很多实用的功能。简单的一条指令，就可以实现包管理，而不用你关心各种依赖和文件路径的情况，十分方便快捷。



[BaiduPCS GO Mac安装指南]([https://github.com/iikira/BaiduPCS-Go/wiki/BaiduPCS-GO-Mac%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97](https://github.com/iikira/BaiduPCS-Go/wiki/BaiduPCS-GO-Mac安装指南))



[idea maven打包 install 报错The packaging for this project did not assign a file to the build artifact](https://www.cnblogs.com/bestxyl/p/9065897.html)



Js 异步

```js
async mounted () {
  this.sstFilter.locationOptions = await this.getLocation(null, 2)
},
  async getLocation (parentId, locationLevel) {
    if (!locationLevel && locationLevel > 4) {
      return null
    }
    let result = []
    let _param = {
      parentId: parentId,
      locationLevel: locationLevel
    }
    let res = await http.post('cd/globallocation/findList', _param)
    if (res && res.code === '200') {
      res.data.sort(extra.sortBy('englishName'))
      result = res.data.map(c => {
        let r = {
          id: c.id,
          label: c.englishName,
          value: c.englishName
        }
        if (c.locationLevel && c.locationLevel < 4) {
          r.children = []
          r.loading = false
        }
        return r
      })
    } else {
      this.$message({
        type: 'error',
        message: res ? res.message ? res.message : 'System error, please try later.' : 'System error, please try later.'
      })
    }
    return result
  },
```



[delete 操作符- JavaScript | MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Operators/delete)



[分布式任务调度平台XXL-JOB](http://www.xuxueli.com/xxl-job/)



修改 el-select 的 width

[el-select 默认样式问题· Issue #2240 · ElemeFE/element · GitHub](https://github.com/ElemeFE/element/issues/2240)



[如何给span设置宽度(width)？](https://coding1688.iteye.com/blog/1562652)

给 `<span>` 标签设置宽度：

需要先将 display 设置为 inline-block



[cursor - CSS（层叠样式表） | MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/cursor)



Oracle 中复杂查询中设计 clob 类型的字段时，如果报 `expected - got CLOB`

可以尝试使用 `to_char`

```sql
SELECT
            c.ID,
            c.GROUP_NAME,
            c.DESCRIPTION,
            c.GROUP_TYPE,
            c.STATUS,
            TO_CHAR(c.STORE_FILTERS),
            COUNT( d.STORE_GROUP_ID ) AS MEMBERQTY,
            su1.name AS assigner,
            su2.name AS assignee,
            e.create_date AS assignedDate,
            c.ASSIGNED_START_DATE,
            c.ASSIGNED_END_DATE,
            c.COMMISSION
        FROM
        (
          SELECT
          a.ID,
          a.GROUP_NAME,
          a.DESCRIPTION,
          a.GROUP_TYPE,
          a.STATUS,
          a.STORE_FILTERS,
          b.ID AS CALL_TASK_DETAILS_ID,
          b.CALL_TASK_ID,
          b.ASSIGNED_START_DATE,
          b.ASSIGNED_END_DATE,
          b.COMMISSION,
          ROW_NUMBER () OVER ( PARTITION BY b.STORE_GROUP_ID ORDER BY b.create_date DESC ) rn
          FROM
          STORE_GROUP a
          LEFT JOIN CALL_TASK_DETAILS b ON a.ID = b.STORE_GROUP_ID
          WHERE
          A.DEL_FLAG = 0
        ) c
        LEFT JOIN STORE_GROUP_REL d ON c.ID = d.STORE_GROUP_ID
        LEFT JOIN CALL_TASK e ON e.id = c.CALL_TASK_ID
        LEFT JOIN sys_user su1 ON e.CREATE_BY = su1.id
        LEFT JOIN sys_user su2 ON e.assigned_id = su1.id
        WHERE
            ( c.rn = 1 OR c.CALL_TASK_DETAILS_ID IS NULL )
						AND e.assign
        GROUP BY
            (
              c.ID,
              c.GROUP_NAME,
              c.DESCRIPTION,
              c.GROUP_TYPE,
              c.STATUS,
              TO_CHAR(c.STORE_FILTERS),
              su1.name,
              su2.name,
              e.create_date,
              c.ASSIGNED_START_DATE,
              c.ASSIGNED_END_DATE,
              c.COMMISSION
            )
```



[Oracle两表关联，只取B表的第一条记录](https://www.cnblogs.com/luxd/p/8527457.html)

使用 `row_number() over`

```sql
SELECT
                a.ID,
                a.GROUP_NAME,
                a.DESCRIPTION,
                a.GROUP_TYPE,
                a.STATUS,
                a.STORE_FILTERS,
                b.ID AS CALL_TASK_DETAILS_ID,
                b.CALL_TASK_ID,
                b.ASSIGNED_START_DATE,
                b.ASSIGNED_END_DATE,
                b.COMMISSION,
                ROW_NUMBER () OVER ( PARTITION BY b.STORE_GROUP_ID ORDER BY b.create_date DESC ) rn
            FROM
                STORE_GROUP a
                LEFT JOIN CALL_TASK_DETAILS b ON a.ID = b.STORE_GROUP_ID
            WHERE
                A.DEL_FLAG = 0
```



Error in v-on handler: "TypeError: Cannot set property 'type' of undefined"

```html
<span slot="footer" class="dialog-footer">
  <el-button type="primary" @click="saveSubmit()">Save</el-button>
</span>
```

```js
saveSubmit () {
  this.$refs.storeGroupForm.validate((valid) => {
    if (valid) {
      let res = this.$api.storeGroup.save(this.editDialog.storeGroup)
      if (res.code === '200') {
        this.$message.success('Edit Success!')
        this.cancelEdit()
        this.getPage()
      } else {
        this.$message.error(res.message)
      }
    } else {
      return false
    }
  })
},
```

原因：请求前没加 `await` ，原理未知。。。



Uncaught (in promise) cancel

```js
confirmDelete (storeGroupId) {
this.$confirm('Confirm deleting operation?', 'Confirm', {
confirmButtonText: 'OK',
cancelButtonText: 'Cancel',
type: 'warning'
}).then(() => this.submitDelete(storeGroupId))
},
```

原因：confirm 没加 `.catch(() => {})`

[这不是报错，只是被 reject 的 Promise 没有 catch。好像只有 Chrome 会这样。](<https://github.com/ElemeFE/mint-ui/issues/705>)



[手摸手，带你用vue撸后台 系列一(基础篇)](https://segmentfault.com/a/1190000009275424)



springboot中查看mybatis执行的sql语句，只用将日志级别设置为debug就可以了



JSON parse error: For input string: "05/19/2019";

原因，json默认的日期格式是 '2019-05-19'

解决方法，在日期类型的字段上加上 `@JSONField(format = "MM/dd/yyyy")`



[挖掘IntelliJ IDEA的调试功能](http://qinghua.github.io/intellij-idea-debug/)



查看是否异步执行的方法：

```java
private final ThreadFactory threadNameFactory = new ThreadFactoryBuilder().setNameFormat("store-group-thread-%d").build();
private final ExecutorService threadPool = new ThreadPoolExecutor(1, 3,
                                                                  0L, TimeUnit.MILLISECONDS,
                                                                  new LinkedBlockingQueue<>(),threadNameFactory);

public StoreGroupVo updateDynamicGroup(StoreGroupVo storeGroupVo) {
  List<StoreVo> storeList = storeService.findStoreList(JSON.parseObject(storeGroupVo.getStoreFilters(), CustomerFilterVo.class));
  storeGroupVo.setMemberQTY(storeList.size());
  Long operator = UserUtils.getUserId();
  threadPool.submit(() -> {
    log.info("aabbcc");
    groupTo(storeList.stream().map(storeVo -> storeVo.getId()).collect(Collectors.toList()), storeGroupVo.getId(), operator);
  });
  log.info("bbccaa");
  return storeGroupVo;
}
```



[Element Form表单布局（一行多列） - ICode9](https://www.icode9.com/content-4-193448.html)



[VUE的for循环一行两列 - Linux下修改mysql ROOT密码](http://hacksteven.com/?p=173)



[html怎样让两个语句显示在同一行- xiaoxiaohui520134的博客- CSDN博客](https://blog.csdn.net/xiaoxiaohui520134/article/details/51800968)



[vue关于父组件调用子组件的方法- Baby_加油_的博客- CSDN博客](https://blog.csdn.net/qq_34664239/article/details/80386153)



[当下拉列表数据过大时，该如何应对？](<https://juejin.im/post/5be534086fb9a049ef2615e2#heading-11>)



[从Windows 过度到Mac 必备快捷键对照表- IntelliJ IDEA 使用教程- 极客 ...](https://wiki.jikexueyuan.com/project/intellij-idea-tutorial/keymap-win-mac.html)



[JS中变量名作为if条件的真/假- gulingeagle的专栏- CSDN博客](https://blog.csdn.net/gulingeagle/article/details/8757039)



[console对象-- JavaScript 标准参考教程（alpha）](https://javascript.ruanyifeng.com/stdlib/console.html)

`console.log`方法支持以下占位符，不同类型的数据必须使用对应的占位符。

- `%s` 字符串
- `%d` 整数
- `%i` 整数
- `%f` 浮点数
- `%o` 对象的链接
- `%c` CSS 格式字符串



[Object.keys()](<https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/keys>)

```js
Object.keys(this.statusList).forEach((prop) => {
  if (this.statusList[prop] === 'Assigned') {
    node.data.status = prop
    console.log('node', node)
  }
})
```



[编程式的导航| Vue Router](https://router.vuejs.org/zh/guide/essentials/navigation.html)



关于浅析VO、DTO、DO、PO的概念、区别和用处 [这里](http://blog.csdn.net/zjrbiancheng/article/details/6253232)有很好的讲解



[mybatis collection 传递Map参数- 神手-追魂的个人空间- OSCHINA](https://my.oschina.net/berthome/blog/1817862)



[编程式的导航](https://router.vuejs.org/zh/guide/essentials/navigation.html)

```js
// 后退一步记录，等同于 history.back()
router.go(-1)
```



[Echarts xAxis boundaryGap](https://www.cnblogs.com/xp1056/p/Echart.html)

echarts boundaryGap留白属性
[如何获取百度云下载直链- TateBrwonJava的博客- CSDN博客](https://blog.csdn.net/TateBrwonJava/article/details/82990235)



最难理解的是作用域插槽。看了文档说明的朋友可能还会有点晕，大概是说在作用域插槽内，父组件可以拿到子组件的数据。子组件可以在slot标签上绑定属性值

- 如：

```
<slot :nickName="'Tusi'"></slot>
复制代码
```

而父组件通过slot-scope绑定的对象下拿到nickName的值。

```
<template>
    <section>
        <slot-child>
            <template slot-scope="scope">
                <div>{{scope.nickName}}</div>
            </template>
        </slot-child>
    </section>
</template>
```



[Mac os下快速从终端进入Finder & 从Finder进入终端- xktxoo的博客 ...](https://blog.csdn.net/xktxoo/article/details/78506487)



[vue-cli项目中使用mockjs模拟数据](<https://www.jianshu.com/p/aea89b5e6d33>)

[Vue配置Mock.js模拟后端数据](<https://wangdaodao.com/20190215/vue-mock.html>)



[自定义事件传参问题](https://github.com/vuejs/vue/issues/5735)



Mac wechat 双开命令：

```shell
open -n /Applications/WeChat.app/Contents/MacOS/WeChat
```





[自定义组件的 `v-model`](https://cn.vuejs.org/v2/guide/components-custom-events.html)



[GitHub开发者](<https://githuber.cn/>)



[Java List去掉重复对象-java8](<https://blog.csdn.net/jiaobuchong/article/details/54412094>)



[一个设计的很好看的个人博客](<https://www.dandyweng.com/>)



camelCase：驼峰命名

kebab-case：短横线命名方式



[在vue项目中如何定义全局变量全局函数- 掘金](https://juejin.im/post/59eddbfe6fb9a0450908abb4)



[类型检查和其它 prop 验证](<https://cn.vuejs.org/v2/guide/components-props.html>)



[解密vue-router: 从源码开始- 掘金](https://juejin.im/post/5af108dc518825672565cf31)



npm -i 是 npm -install 的缩写

[npm i和npm install的区别](<https://blog.csdn.net/chern1992/article/details/79193211>)



npm -S 是 npm —save 的缩写，表示安装的包将写入`package.json`里面的`dependencies`。

[npm install 命令参数的一些简写方式| 清风轩](https://xovel.cn/article/npm-alias.html)



要知道你使用的Mac OS X是什么样的Shell，

打开终端，输入：echo $SHELL 回车执行

如果输出的是：csh或者是tcsh，那么你用的就是C Shell。

如果输出的是：bash，sh，zsh，那么你的用的可能就是Bourne Shell的一个变种。

Mac OS X 10.2之前默认的是C Shell。

Mac OS X 10.3之后默认的是Bourne Shell。



[使用 Sass 编译 `<style>` 语言块](<https://vue-loader-v14.vuejs.org/zh-cn/configurations/pre-processors.html>)

[SCSS 与 Sass 异同](<http://sass.bootcss.com/docs/scss-for-sass-users/>)



Atom

打开命令行面板：Command + Shift + P



除了可以用command+F3 来**显示桌面**以外，我们还可以通过Fn+F11 **键**来**显示桌面**。 使用**快捷键**Command+M，可以实现快速最小化当前窗口的目的。 使用**快捷键**Command+Option+M，可以实现快速最小化当前应用程序所有窗口的目的。 比如你想一下子最小化多个Finder 窗口，就可以用该**快捷键**。



<https://www.zhihu.com/question/34544815>



[数组去重合并](<https://blog.csdn.net/qq_39207948/article/details/80369606>)

<https://blog.csdn.net/qingmengwuhen1/article/details/79876813>



[Array.prototype.find() - JavaScript | MDN - Mozilla](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/find)



[嵌套的 Dialog](<https://element.eleme.io/2.0/#/zh-CN/component/dialog#qian-tao-de-dialog>)

如果需要在一个 Dialog 内部嵌套另一个 Dialog，需要使用 `append-to-body` 属性。



[vue项目如何刷新当前页面](<https://blog.csdn.net/qq_16772725/article/details/80467492>)



[vue 父组件传值给子组件遇到的生命周期问题](<https://blog.csdn.net/qq_36416878/article/details/80219134>)

如果要在子组件打印父组件传来的数据必须是在beforeUpdate和updated生命周期才能监听的到，



[Object.assign()](<https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/assign>)



[Uncaught SyntaxError: Unexpected token u in JSON at position 0 ...](https://stackoverflow.com/questions/46613243/uncaught-syntaxerror-unexpected-token-u-in-json-at-position-0)



[通过 sass-resources-loader 全局注册 Sass/Less 变量](https://www.cnblogs.com/cangqinglang/p/10573151.html)



[vue.js自定义组件上使用v-model](<https://juejin.im/post/5afd95fa6fb9a07a9e4d72a8>)



[如何在Mac 上强制退出应用- Apple 支持](https://support.apple.com/zh-cn/HT201276)



[Vue.js 技术揭秘](<https://ustbhuangyi.github.io/vue-analysis/>)



[Vue Element.ui tree, emit reload event](https://stackoverflow.com/questions/47855365/vue-element-ui-tree-emit-reload-event)



[10个最好的JavaScript在线编辑器 - Education Ecosystem Blog](https://blog.education-ecosystem.com/10个最好的javascript在线编辑器/)



[Oracle / PLSQL: Check Constraints - TechOnTheNet](https://www.techonthenet.com/oracle/check.php)





<https://learnku.com/>



[当绑定空的验证对象时, 会导致el-input组件输入框无法输入,将其type ...](https://github.com/ElemeFE/element/issues/1009)



[Axure 9 注册码](<https://blog.csdn.net/zff980320/article/details/89634536>)

axure rp pro 9.0 Team团队版：
被授权人：www.ddooo.com
授权秘钥：BaOifFBSUZ8tROgZzdfn/TV77k8+D8lVumI5alvEHXctoJNVeSR77YlckA+oAJKE



[Axure RP 9 培训教程：Gif动画＋示例＋QQ答疑教学](http://www.webppd.com/thread-19496-1-1.html)



[liangxiaojuan/vue-todos: vue最新实战项目教程，从零开始 ... - GitHub](https://github.com/liangxiaojuan/vue-todos)



<http://www.todolist.cn/>



[史上最简单的Spring Cloud教程](<https://github.com/forezp/SpringCloudLearning>)



[JDK源码阅读顺序](<https://blog.csdn.net/qq_21033663/article/details/79571506>)



[Spring Boot 实现原理与源码解析系统 —— 精品合集](http://www.iocoder.cn/Spring-Boot/good-collection/)



<https://github.com/ElemeFE/element/issues/3217>

<https://github.com/ElemeFE/element/issues/1534>



[Spring Boot(六)：如何优雅的使用 Mybatis](https://www.cnblogs.com/ityouknow/p/6037431.html)



[如何参与一个 GitHub 开源项目？](<https://blog.csdn.net/lanxuezaipiao/article/details/23546349>)

[Github上怎么修改别人的项目并且提交给原作者！图文并茂！](<https://blog.csdn.net/qq_26787115/article/details/52133008>)







[HTMLElement.offsetTop - Web API 接口参考| MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/HTMLElement/offsetTop)



[触摸事件- Web API 接口参考| MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/Touch_events)







[Java SpringBoot 循环依赖问题](https://wars.cat/blog/index.php/archives/14/)

循环依赖发生于使用构造函数注入的时候，其他注入方式不会发生此问题，
因为其他方式会在程序用到这个依赖时，才会注入，而不是发生在Spring Context加载阶段。



![](http://www.w3school.com.cn/i/kaikeba.gif)https://s.growingio.com/0W5deo



[[CSS\]图片水平排列并且有固定间隔- 我是涛锅- CSDN博客](https://blog.csdn.net/qq807081817/article/details/49099401)



[如何修改Mac文件默认打开方式-百度经验](https://jingyan.baidu.com/article/d5a880ebdd3b2f13f147cc1c.html)



Design Music logo, @2, @3.



[CSS之Position详解](https://www.cnblogs.com/Zigzag/archive/2009/02/19/position.html)



https://www.leiyun.org/sf/8a9f0eb75aced5731b91fc109c9aba44.html

[慕课网2018年全站付费资源共800G百度网盘资源免费分享- 福利巢](https://www.fulichao.com/7383.html)



[Vue 设置 Script 标签首层不缩进](https://www.jianshu.com/p/622c463ff925)





将本地的已有项目关联到github上的新的项目上
在github上新建一个仓库，然后在本地仓库中执行git remote add origin git@github.com:stormzhang/test.git
origin是仓库的名字，可能你的本地项目关联着几个仓库，你可以根据仓库的名字
git push origin master 将代码提交到不同仓库中，可以指定分支
然后执行git pull origin master 先将github上的代码pull下来
然后在git push origin master





[vue-cli的build的文件夹下没有dev-server.js文件，怎么配置mock数据。---mock数据配置(一)](https://juejin.im/post/5aba11da51882577b45f0ad1)



[百度云盘HTML5视频倍速播放]([https://greasyfork.org/zh-CN/scripts/374693-%E7%99%BE%E5%BA%A6%E4%BA%91%E7%9B%98html5%E8%A7%86%E9%A2%91%E5%80%8D%E9%80%9F%E6%92%AD%E6%94%BE](https://greasyfork.org/zh-CN/scripts/374693-百度云盘html5视频倍速播放))



[CSS秘密花园： Sticky footers](https://www.w3cplus.com/css3/css-secrets/sticky-footers.html)



[2019年Web前端最新导航（常见前端框架、前端大牛）](https://www.cnblogs.com/qianguyihao/p/10701923.html)



[前端代码乱糟糟？是时候引入代码质量检查工具了](https://www.cnblogs.com/imwtr/p/9189414.html)



[解决 vue中props值无法赋值给data域的问题](https://blog.csdn.net/baidu_31333625/article/details/84789416)



[Mybatis对Oracle的批量操作 增加，更新，删除](https://www.iteye.com/blog/crukor-2215573)

https://blog.csdn.net/lwpczy1/article/details/79158535



[SpringBoot构造器注入循环依赖及解决](https://blog.csdn.net/Revivedsun/article/details/84642316)



https://docs.oracle.com/en/database/oracle/oracle-database/12.2/adjsn/overview-of-inserting-updating-loading-JSON-data.html#GUID-94E37619-C242-44F0-B1C3-9A63859AD0C5

Update operations on a document in a JSON column require the replacement of the entire document. You can make fine-grained modifications to a JSON document, but when you need to save the changes to disk the entire updated document is written.



[JSONObject和JSONArray遍历数组与对象](https://blog.csdn.net/shanliangliuxing/article/details/25163005)



[fastjson对JSONObject中的指定字段重新赋值](https://blog.csdn.net/matrix_google/article/details/80855471)



[Java Set集合的详解](https://blog.csdn.net/qq_33642117/article/details/52040345)



mybatis `<association/>` 必须在 `<collection/>` 前



线程池的使用

```java
private final ThreadFactory namedFactory = new ThreadFactoryBuilder().setNameFormat("GlobalLocationService-ThreadPool-%d").build();
private final ExecutorService executorService = new ThreadPoolExecutor(1, 5, 500, TimeUnit.MILLISECONDS, new LinkedBlockingDeque<>(), namedFactory, new ThreadPoolExecutor.DiscardOldestPolicy());
```



[中英文自动添加空格](http://wingjay.com/2017/06/08/rebuild-personal-blog/)



[Hexo博客跳过渲染，创建自定义网页](http://blog.fcj.one/hexo-custom-page.html)

[关于如何在Hexo上添加原生HTML页面](https://tailsxky.github.io/2018/03/22/add-html-page/)



[使用 github pages, 快速部署你的静态网页](https://zhuanlan.zhihu.com/p/38480155)



https://developer.mozilla.org/zh-CN/docs/Web/CSS/object-fit



https://stackoverflow.com/questions/10123953/how-to-sort-an-array-by-a-date-property



https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1-QO003JbLVaUcqt2G_BfMgo-e-rpsbS3XxuoYaEDEc4&font=Default&lang=zh-cn&initial_zoom=2&height=650

https://docs.google.com/spreadsheets/d/1-QO003JbLVaUcqt2G_BfMgo-e-rpsbS3XxuoYaEDEc4/edit#gid=0



http://www.runoob.com/w3cnote/javascript-two-decimal.html



https://www.linchaoqun.com/html/cms/content.jsp?menu=index&id=bdfad840-7607-4ec2-a440-4da31c3b70cb





购买

https://zhuanlan.zhihu.com/p/29006953

A6300机身 + 套机镜头16-50 + 一只FE50mm f1.8（人像虚化），共计人民币9000左右



使用

https://zhuanlan.zhihu.com/p/30243263



评测

https://cn.engadget.com/2016/05/04/sony-a6300-review/



[聊聊Tomcat的架构设计](http://objcoding.com/2019/05/30/tomcat-architecture/)





[解决git pull/push每次都需要输入密码问题- 生如夏花炫至茶靡 ...](https://blog.csdn.net/nongweiyilady/article/details/77772602)



[IDEA 整合jira - jacker - CSDN博客](https://blog.csdn.net/wangmeng951011/article/details/72613719)

需要把插件也装上



[idea生成类注释和方法注释的正确方法](https://blog.csdn.net/qq_34581118/article/details/78409782)



[SpringMVC 中 request.getInputStream() 为空解惑](https://emacsist.github.io/2017/12/04/springmvc-中-request.getinputstream-为空解惑/)



[【Java基础】InputStream 、 InputStreamReader和BufferedReader](https://blog.csdn.net/zgljl2012/article/details/47267609)



[为什么使用TypeReference](https://yq.aliyun.com/articles/609441)



[产品之术：一目了然的状态机图](http://www.woshipm.com/pmd/828671.html)

[如何绘画状态机来描述业务的变化](http://www.woshipm.com/pd/594751.html)



[使用Git Stash Save 将暂存区命名| Shawn's Blog](https://blog.just666.com/2018/03/05/git-stash/)



[Convert String to JsonObject with Gson | Baeldung](https://www.baeldung.com/gson-string-to-jsonobject)



[移动端真机调试指南| Aotu.io「凹凸实验室」](https://aotu.io/notes/2017/02/24/Mobile-debug/index.html)



Charles 注册码

```bash
Registered Name:https://zhile.io
License Key: 48891cf209c6d32bf4
```



[charles连接手机抓包](https://www.cnblogs.com/xiaoshidi/p/6878557.html)

将手机wifi位置的ip地址设置成静态ip



[如何通过蓝牙和Mac OS X转移的Android智能手机之间的文件（照片，视频，文档）](https://zh-cn.amtelefon.com/cum-facem-transfer-de-fisiere-poze-clipuri-documente-prin-bluetooth-intre-un-smartphone-si-mac-os-x/samsung/)

到 **系统偏好设定** la **共享** 然后点击图标打开 **共享设置**.

在共享菜单选项，去酒吧在左， **激活文件共享服务** 为 **蓝牙**。 蓝牙共享。



```java
Gson gson = new Gson();  
String json = gson.toJson(obj);  
```



[docker中宿主机与容器（container）互相拷贝传递文件的方法](https://blog.csdn.net/dongdong9223/article/details/71425077)

```dockerfile
docker cp ID全称:容器文件路径 本地路径
```



**docker exec ：**在运行的容器中执行命令

OPTIONS说明：

- **-d :**分离模式: 在后台运行
- **-i :**即使没有附加也保持STDIN 打开
- **-t :**分配一个伪终端

在容器 mynginx 中开启一个交互模式的终端:

```shell
runoob@runoob:~$ docker exec -i -t  mynginx /bin/bash
```



[idea跳转到某行的快捷键(mac os) - www_minna_com的博客 ...](https://blog.csdn.net/www_minna_com/article/details/88576638)



[java数组的三种初始化方式- Blog 微笑的草莓丶- CSDN博客](https://blog.csdn.net/Elias94/article/details/79808581)



String.lastIndexOf()



[Docker实践(二)：容器的管理(创建、查看、启动 ... - CSDN博客](https://blog.csdn.net/u010246789/article/details/53958662)

- `docker ps`: 查看当前运行的容器



Excel: [在单元格中插入当前日期和时间]([https://support.office.com/zh-cn/article/%E5%9C%A8%E5%8D%95%E5%85%83%E6%A0%BC%E4%B8%AD%E6%8F%92%E5%85%A5%E5%BD%93%E5%89%8D%E6%97%A5%E6%9C%9F%E5%92%8C%E6%97%B6%E9%97%B4-b5663451-10b0-40ab-9e71-6b0ce5768138](https://support.office.com/zh-cn/article/在单元格中插入当前日期和时间-b5663451-10b0-40ab-9e71-6b0ce5768138))

注意是在英文输入格式下。



[查看提交历史 - Git SCM](https://git-scm.com/book/zh/v1/Git-基础-查看提交历史)



Idea: fn + alt + f12 打开/关闭 Terminal



[Null safe equals method | Examples Java Code Geeks - 2019](https://examples.javacodegeeks.com/core-java/class/null-safe-equals-method/)

[Compare two objects in Java with possible null values - Stack ...](https://stackoverflow.com/questions/11271554/compare-two-objects-in-java-with-possible-null-values/11271611)

```
Objects.equals()
```



```java
Gson gson = new Gson();
String json = gson.toJson(user);
```



[对区域或表中的数据进行排序- Excel - Office Support - Office 365](https://support.office.com/zh-cn/article/对区域或表中的数据进行排序-62d0b95d-2a90-4610-a6ae-2e545c4a4654)



[创建下拉列表- Office 支持 - Office Support - Office 365](https://support.office.com/zh-cn/article/创建下拉列表-7693307a-59ef-400a-b769-c5402dce407b)

第四点中的“列表”在2019版中叫“序列”



[版本回退- 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/896043488029600/897013573512192)



[Git远程操作详解- 阮一峰的网络日志](http://www.ruanyifeng.com/blog/2014/06/git_remote.html)

如果远程主机的版本比本地版本更新，推送时Git会报错，要求先在本地做`git pull`合并差异，然后再推送到远程主机。这时，如果你一定要推送，可以使用`--force`选项。

> ```git
> $ git push --force origin
> ```



https://www.jianshu.com/p/4d135cafe245



https://devqa.io/convert-list-to-array-in-java/



[Handling null values in Freemarker - Stack Overflow](https://stackoverflow.com/questions/13950289/handling-null-values-in-freemarker/27614219)



[在Premiere Pro 中创建和更改序列 - Adobe](https://helpx.adobe.com/cn/premiere-pro/using/creating-changing-sequences.html)



pr 调整照片大小
https://www.youtube.com/watch?v=PcMarwNxv8U



[播放时没有声音 - Adobe](https://helpx.adobe.com/cn/premiere-pro/kb/no-sound-playback-premiere-pro.html)



[Mac查看端口占用情况- 破男孩- 博客园](https://www.cnblogs.com/ayseeing/p/4097686.html)



[Tomcat 8以上版本文件上传后无权限访问的问题- 简书](https://www.jianshu.com/p/c6de9b93dbd2)



[配置别名- 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/896043488029600/898732837407424)



[Git远程操作详解- 阮一峰的网络日志](http://www.ruanyifeng.com/blog/2014/06/git_remote.html)

取回特定分支的更新

取回`origin`主机的`master`分支。

```javascript
$ git fetch origin master
```



[使用java 8 提取出list中bean的某一属性- Nightliar的博客 ...](https://blog.csdn.net/Nightliar/article/details/78657949)



查看linux文件的权限：ls -l 文件名称

查看linux文件夹的权限：ls -ld 文件夹名称



任何maven仓库都下载不到oracle的jar包

因为oracle的jar包要去官网登陆才能拿到

除非你下载好之后自己上传的私服



https://blog.csdn.net/qq_39940866/article/details/80320328

设置远程跟踪

git branch --set-upstream-to=origin/branchName



[Git远程操作详解- 阮一峰的网络日志](http://www.ruanyifeng.com/blog/2014/06/git_remote.html)

拉取远程分支到本地，并切换到该分支下

```javascript
$ git checkout -b branchName origin/branchName
```



Mac 

Command+Shift+. 可以**显示隐藏文件**、**文件**夹，再按一次，恢复**隐藏**；

[10 个实用技巧，让Finder 带你飞- 少数派](https://sspai.com/post/27403)



https://stackoverflow.com/questions/20171768/using-sql-query-with-group-by-date

```sql
select trunc(system_date), count(is_paid)`
  from TPWEB.TP_CLIENT_TENDER_TRANS
 where system_date between date '2012-12-01' and date '2012-12-31'
 group by trunc(system_date)
```



```xml
<if test="importedDateStart != null">
    AND ih.IMPORTED_DATE >= #{importedDateStart}
</if>
<if test="importedDateEnd != null">
    <![CDATA[AND ih.IMPORTED_DATE <= #{importedDateEnd} + 1]]>
</if>
```





https://www.youtube.com/watch?v=jXcnLmymJWI



http://www.vstcrack.com/guitar-pro-7-5-mac/#page-content

http://crackreview.com/guitar-pro-crack/



excel 显示所有隐藏行：

全选、右键、取消隐藏



[Array.prototype.find() - MDN - Mozilla](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/find)



oracle order by 多条件：

```sql
ORDER BY t.maxDate DESC, t.VendorName ASC, t.IncidentDate DESC
```



git查看本地分支关联（跟踪）的远程分支之间的对应关系

git branch -vv



http://www.voidcn.com/article/p-edflrmln-bts.html





[CSS 开关样式| 菜鸟工具](https://c.runoob.com/codedemo/3146)

[css3实现的switch开关按钮 - CodePen](https://codepen.io/chutou/pen/qdGZQr)



使用 Linux alias 配置 git 快速提交命令

[git 快速提交| frostbelt's home](https://frostbelt.github.io/2018/12/19/git-快速提交/)

命令改成

```shell
alias gitqkci='git add . && git commit -m ${1:-update} && git push'
```

https://man.linuxde.net/alias

https://www.liaoxuefeng.com/wiki/896043488029600/898732837407424

https://unix.stackexchange.com/questions/329994/alias-and-functions

https://www.zhihu.com/question/23137414





Git checkout 时忘记关联远程仓库，可以利用

git pull origin branchName 来将本地和远程仓库关联起来。





https://pandoc.org/getting-started.html

```shell
pandoc test.md -s -o test.docx
```



[javascript中的双波浪线~~与双感叹号!!,.NET双问号??用法](https://blog.cozof.com/pieces/pieces/13.shtml)

双波浪线 `~~` 等价于Math.floor取整，`~~` 的效率较高可读性较差,"Math.floor"效率较高可读性较低。

双感叹号"!!"等价于"Boolean",把值转换为bool类型；



https://www.bilibili.com/read/cv1069327/

百度云播放页面，控制台输入

```js
videojs.getPlayers("video-player").html5player.tech_.setPlaybackRate(2)
```



B2C：人与商品，例如京东、淘宝

P2P：人与人，例如微信、QQ

C2P：人与服务，例如小程序





https://www.baeldung.com/gson-string-to-jsonobject



https://stackoverflow.com/questions/2003505/how-do-i-delete-a-git-branch-locally-and-remotely

```bash
$ git push -d <remote_name> <branch_name>
$ git branch -d <branch_name>
```



```sql
UPDATE (
SELECT
	ow.FREESHIPPINGTYPE 
FROM
	ORDERWAREHOUSE ow
	LEFT JOIN ORDERS o ON ow.ORDERID = o.ORDERID 
WHERE
	o.ORDERSOURCE = 1 
	AND ow.SHIPPINGPRICE = 0 
	AND ow.FREESHIPPINGTYPE IS NULL 
	) t 
	SET t.FREESHIPPINGTYPE = 1
```



Oracle  between 区间是闭区间



https://blog.csdn.net/w958796636/article/details/53611133

不删除工作空间改动代码，撤销 `commit`，并且撤销 `git add .` 操作

这个为默认参数, git reset --mixed HEAD^ 和 git reset HEAD^ 效果是一样的。



http://blog.itpub.net/205377/viewspace-1278977/

1) 执行:ALTER SEQUENCE SEQ_TEST INCREMENT BY 1000;

2) 执行:SELECT SEQ_TEST.NEXTVAL FROM DUAL;

3) 执行:ALTER SEQUENCE SEQ_TEST INCREMENT BY 1;