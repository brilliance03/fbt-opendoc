修改企业部门

----|---
POST|/open/api/org/departments/update

请求参数

字段|名称|类型|必填|描述
-----|-----|----|----|----
timestamp|时间戳 |long |Y|13位时间戳
sign|签名 |string |Y|
access\_token|token | string |Y|登录 token
employee\_id| 操作人id|string |Y|操作人id,调用接口人 id
data |请求数据| jsonstring |Y|
data.org\_unit\_id|部门ID |string|Y|部门ID
data.org\_unit\_name|部门名称| string |Y|部门名称
data.parent\_id| 父部门 id|string |Y|父部门 id
data.manager\_list||array|N|列表

请求示例


}


返回结果

