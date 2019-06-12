## Oracle

```sql
select * from deal where del_flag = 0 and deal_content like '%' || 'a' || '%'
```

> `||` 为字符串连接符