需参与鉴权的参数定义:

3.MD5采用org.apache.commons下DigestUtils.md5Hex(param)加密；

字段|名称|类型|必填|描述
----|----|---|---|---
timestamp|时间戳|long|Y|13位时间戳
sign_key|签名key|string|Y|鉴权接口获得的口令
data|请求的业务参数|jsonstring|Y|