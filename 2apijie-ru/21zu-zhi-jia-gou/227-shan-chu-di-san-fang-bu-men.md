请求方式|请求地址
----|---
POST|/open/api/third/departments/delete

请求参数

字段|名称|类型|必填|描述
-----|-----|----|----|----
timestamp|时间戳 |long |Y|13位时间戳
sign|签名 |string |Y|
access\_token|token | string |Y|登录 token
employee\_id| 操作人id|string |Y|操作人id,调用接口人 id
employee\_type| 用户类型|string|Y|类型，0为分贝用户，1为第三方用户
data || jsonstring |Y|请求数据
data.company\_id|公司ID|string|Y|分贝通
data.third\_org\_id|部门id| string |Y|第三方机构部门ID







请求示例:


"company_id":"57872y4ksdfh8732h78sd89",
"third_org_id": "879938j7dj38d73jd8"
}

}


返回结果

```


{
 "code": 0,
 "msg": "success" 
}


{"request_id":"JBf1zsdKYCjUoEuQMEKN",
"code":200002,
"msg":"当前第三方部门ID不存在"
}








