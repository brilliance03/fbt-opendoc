根据企业ID删除部门
----|---
POST|/open/api/org/departments/delete

请求参数：

字段|名称|类型|必填|描述
-----|-----|----|----|----
timestamp|时间戳 |long |Y|13位时间戳
sign|签名 |string |Y|
access\_token|token | string |Y|登录 token
employee\_id| 操作人id|string |Y|操作人id,调用接口人 id
data |请求数据| jsonstring |Y|请求
data.org\_ unit\_ids| 部门id|array |Y|部门id
 
 请求示例


}


返回结果

