## Oracle

### 模糊查询

```sql
select * from deal where del_flag = 0 and deal_content like '%' || 'a' || '%'
```

> `||` 为字符串连接符

### varchar 与 varchar2 的区别

1. varchar2 中所有字符都占两个字节，varchar 中只有汉字和全角字符占两个字节，其余占一个字节
2. **varchar2 将空字符串按照 NULL 处理**

### 主键子增

1. 创建序列

   ```sql
   CREATE SEQUENCE SYS_USER_SEQ
   MINVALUE 1 
   NOMAXVALUE 
   INCREMENT BY 1 
   START WITH 1 NOCACHE ;
   ```

2. 插入时调用序列

   ```sql
   INSERT INTO sys_user ( user_id, user_name, user_pwd, sex )
   VALUES
   	( SYS_USER_SEQ.NEXTVAL, 'shaoduo', 'shao111', '男' );
   ```

   项目中使用 MyBatis 的注解 @KeySql 调用

   ```java
   @Id
   @Column(name = "ID")
   @KeySql(sql = "select SYS_USER_SEQ.nextval from dual", order = ORDER.BEFORE)
   private Long id;
   ```

### 递归查询

> [ORACLE 递归查询](https://www.cnblogs.com/bpdwn/archive/2013/06/08/3125987.html)

在具有层次结构的表中竟然需要递归查询。最经典的就是 Address 的查询。

### CHECK

```sql
ALTER TABLE STORE_GROUP ADD CONSTRAINT STORE_FILTERS_JSON_CHECK CHECK ( STORE_FILTERS IS json );
```

### 查询最新的一条记录

```sql
SELECT * FROM
	( SELECT * FROM tableName ORDER BY CREATED_DATE DESC ) 
WHERE
	ROWNUM = 1
```

### 获取当前日期

  [SYSDATE](http://psoug.org/definition/SYSDATE.htm)

