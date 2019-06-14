## Java List合并去重

```java
A.removeAll(B);
A.addAll(B);
```

## MyBatis 批量查询

```java mapper.java
Page<UserPoJo>  findUserListByIds(@Param("Ids") List<Integer> Ids);
```

```xml mapper.xml
<select id="findUserListByIds" resultType="com.glory.api.job.pojo.UserPoJo">
  SELECT * from yy_users
  WHERE id in
  <foreach collection="Ids" item="dramaId" open="(" close=")" separator=",">
    #{dramaId}
  </foreach>
</select>
```

**注意：mapper 接口中参数必须加@Param("Ids")，否则报错说Ids not found**

Hutool

> [Hutool](https://hutool.cn/)

*Hutool*是一个Java工具包，也只是一个工具包，它帮助我们简化每一行代码，减少每一个方法，让Java语言也可以“甜甜的”。

## Convert a `Map<key,value>` to a `List<value>`

> [How to convert a Map to List in Java? - Stack Overflow](https://stackoverflow.com/questions/1026723/how-to-convert-a-map-to-list-in-java)

```java
List<Value> list = new ArrayList<Value>(map.values());
```

