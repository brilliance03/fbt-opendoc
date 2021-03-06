2.10.1 创建审批单
####接口说明
- 1.**最新接口**
- 2.如果有审批业务，则需要进行通过该接口创建审批单，在下单时可以选择创建的相应审批单


| 请求方式 | 请求地址 |
| --- | --- |
| POST | /open/api/approve/create |

| 字段 | 名称 | 类型 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| access\_token | 鉴权Token | string | Y | 5747fbc10f0e60e0709d8d722 |
| sign | 签名 | string | Y | oihfnlyeofdh98 |
| timestamp | 时间戳 | long | Y | 13位时间戳  1241243250000 |
| employee\_id | 用户ID | string | Y | 分贝用户id或者第三方用户id,为创建人的ID|
| employee\_type | 用户类型 | string | Y |  类型，0为分贝用户，1为第三方用户 |
| data |  请求数据 | jsonobject | Y |请求数据
| data.apply | 申请单内容 | jsonobject | Y|申请单详细内容
| data.apply.type| 申请单业务类型 | integer | Y | 1.差旅\(对应trip\_list下的type值为7、11、15\) 2.用车\(对应trip\_list下的type值为3\) 3.采购 |
| data.apply.flow\_type | 审批类型 | integer | Y | 固定为4 |
| data.apply.third\_id | 申请单id | string | Y | 第三方审批单id |
| data.apply.third\_remark | 第三方备注 | string | Y |详细备注信息
| data.apply.budget | 申请单预算 | integer | Y | 预算总额\(为trip\_list中estimated\_amount的总和 \) |
| data.trip\_list | 行程列表 | jsonarray | Y | 行程列表 |
| data.trip\_list.type | 业务类型 | integer | Y | 行程类型 7.机票 11.酒店 15.火车 3.用车 |
| data.trip\_list.start\_city\_id | 出发城市ID | string | Y | 在酒店业务中，start_city_id和arrival_city_id都传入目的地城市ID|
| data.trip\_list.start\_time | 出发时间 | string | Y | 行程开始日期 2017-12-13
| data.trip\_list.arrival\_city\_id | 目的地城市 | string | Y | 行程到达城市ID |
| data.trip\_list.end\_time | 结束时间 | string | Y | 行程结束日期 2017-12-23
| data.trip\_list.estimated\_amount | 预估价格 | integer | Y | 100,单位分 |

请求示例：

```
{
    "access_token":"5747fbc10f0e60e0709d8d722",
    "timestamp":124124325,
    "sign":"oihfnlyeofdh98",
    "employee_id":"59b74c1323445f2d54dd07922",
    "employee_type":1,
    "data":{            
           "apply":{
               "type":1,
              "flow_type":4, 
               "budget":1,
             "third_id":"59dc7fe62798635263b8414a",
              "third_remark":"approve-openapi-test2"
             },
         "trip_list":[{
               "type":7,  
               "start_city_id":"2000002",        
              "start_time":"2017-12-13",
              "arrival_city_id":"1000001",
              "end_time":"2017-12-13",
             "estimated_amount":1
             }]    

     }
}
```

响应结果：

```
{
    "request_id": "xUolOnJHWhIO4YP8MozO",
    "code": 0,
    "msg": "success",
    "data": {
        "id": "58baa2866819481560f013ac"
    }
}
```



