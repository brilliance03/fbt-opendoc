需参与鉴权的参数定义:

2.sign=md5(timestamp=xxxx&data="xxxx"&sign\_key="xxx)转小写,注意顺序  

3.MD5采用org.apache.commons下DigestUtils.md5Hex(param)加密，不同的编程语言MD5加密是相同的，调用相对应的编程语言进行数据加密即可

```
String s="timestamp=151550234600&data={"type":"6"}&sign_key=e376f7f93020af4958c51de227d63368";
byte[] by = s.getBytes("utf-8");
String md5String = DigestUtils.md5Hex（by）




```

字段|名称|类型|必填|描述
----|----|---|---|---
timestamp|时间戳|long|Y|13位时间戳
sign_key|签名key|string|Y|鉴权接口获得的口令
data|请求的业务参数|jsonstring|Y||