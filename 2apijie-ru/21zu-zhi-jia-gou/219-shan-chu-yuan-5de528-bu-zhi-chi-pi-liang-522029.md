根据企业ID和员工ID删除员工
----|---
POST|/open/api/org/employees/delete

字段|名称|类型|必填|描述
-----|-----|----|----|----
timestamp|时间戳 |long |Y|13位时间戳
sign|签名 |string |Y|
access\_token|token | string |Y|登录 token
employee\_id| 操作人id|string |Y|操作人id,调用接口人 id
data || jsonstring |Y|
data.employee\_id| 操作人id|员工ID| String |Y|
 
 请求示例

	"access_token": "xxx.xxx.xxx",

```

返回结果

