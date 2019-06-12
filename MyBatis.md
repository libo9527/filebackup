## MyBatis

### 模糊查询

```xml
<select id="getDealList" resultType="com.sst.cloud.provider.cd.customer.vo.dealvo.DealVo">
  select *
  from deal
  where del_flag = 0
  <if test="dealContent != null and dealContent.trim() != ''">
    and deal_content like '%' ||  #{dealContent} || '%'
  </if>
  <if test="dealResult != null and dealResult.trim() != ''">
    and deal_result like '%' || #{dealResult} || '%'
  </if>
</select>
```

### SQL 片段

```xml
<mapper namespace="com.sst.cloud.provider.cd.customer.mapper.DealMapper">
	<sql id="commonSql">
		ID,
    STORE_EMPLOYEE_ID,
    DEAL_CONTENT,
    DEAL_RESULT,
    CREATE_BY,
    CREATE_DATE,
    UPDATE_BY,
    UPDATE_DATE,
    DEL_FLAG,
    STATUS
	</sql>
  <select id="select" resultType="Deal">
	   select 
        <include refid="CommonSQL.commonSql"></include> 
     from deal
  </select>
</mapper>
```

