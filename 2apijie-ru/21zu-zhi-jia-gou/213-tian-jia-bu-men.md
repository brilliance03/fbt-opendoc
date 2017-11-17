请求方式|请求地址
----|---
POST|/open/api/org/departments/create


请求参数:

字段|名称|类型|必填|描述
-----|-----|----|----|----
timestamp|时间戳 |long |Y|13位时间戳
sign|签名 |string |Y|
access\_token|token | string |Y|登录 token
employee\_id| 操作人id|string |Y|操作人id,调用接口人 id
data || jsonstring |Y|请求数据
data.org\_unit\_name|部门名称|string|Y|部门名称
data.parent\_id| 父部门 id|string |Y|父部门id
data.org\_unit\_id|部门 id| string |Y|部门 id
 
 请求示例:
 

}


返回结果

```

{
