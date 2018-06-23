# ** 分贝通接口文档说明书**

> ## 1.郑重说明：
>
> 本接口文档属于分贝通科技有限公司的资产,个人不得将其据为己有或从事非法活动.在未经授权的情况下,分贝通科技有限公司员工不得将该文档提供给第三方公司及个人,如若因个人原因致使文档提供给第三方最终导致分贝通科技有限公司遭受经济损失或企业形象受损,或者给第三方相关公司带来经济损失或企业形象受损.分贝通科技有限公司有权对相应人员进行相应的处罚,后果严重的可以直接移交司法机关.如若需要业务合作使用需部门领导批准,望周知!!!
>
> ## 2.接口文档简介：

> 本接口文档使用说明书旨在帮助分贝通科技有限公司的合作伙伴更好的了解分贝通,同时也不断拓展分贝通的业务范围以及不断提高自身的业务水平，最终为客户以及合作伙伴提供更为优质的服务,促进多方共赢,达到愉快、高效、长久的合作  

>**文档模块主要包含以下内容:**  

>###2.1.H5模块  

>**2.1.1.鉴权模块:**根据分贝通开通的相关的企业相关鉴权信息，进行鉴权操作  

>**2.1.2.验证token模块:**通过鉴权后拿到token后进行认证操作,完成相应的登录操作  

>###2.2.API模块  

>**2.2.1.鉴权模块:**根据分贝通开通的相关企业相关鉴权信息，进行鉴权操作  

>**2.2.2.验证token模块:**通过鉴权后拿到token后进行接口调用使用  

>**2.2.3.组织架构模块:**包含部门,人员的新增,修改,删除,查询功能(暂时只支持标准的增删改查)  

>**2.2.4.审批单模块:**包含创建审批单的功能,通过第三方系统创建审批单到分贝通,然后通过分贝通APP下单时即可关联相应的审批单关联操作  

>**2.2.5.公用模块:**包含查询城市的编码信息,查询企业的权限规则信息  

>**2.2.6.订单模块:**包含机票,火车,酒店,用车,用餐的订单列表和订单详情,通过该模块可以查询企业使用分贝通APP所下的订单信息  

>**2.2.7.订单消息推送模块:**该模块包含用车,机票,火车,酒店,用餐的订单信息数据,可以把实时的订单信息推送给企业(根据企业的不同需求可以推送具有差异化的内容),企业可以拿到相应的订单信息进行相关的操作,不同的企业根据自己的业务需求进行相关操作.该功能需要企业也进行相应的开发任务(用于接收推送的订单信息接口)  


> ## 3.接口文档使用权限:
>
> 本接口文档的使用范围为与北京分贝通科技有限公司有业务合作的企业.使用本接口文档前需要北京分贝通科技有限公司的相关领导和其他相关人员(业务人员和技术人员)授权后方可使用,如若在未经授权的情况下使用该文档进行非法活动或者进行相关的影响北京分贝通科技有限公司正常的业务开展工作,致使北京分贝通科技有限公司遭受经济损失或有损分贝通科技有限公司企业形象的,根据中华人民共和国刑法以及2017年6月1日实施的中华人民共和国网络安全法的相关规定,北京分贝通科技有限公司有权追究其责任,并将其移交至相应的司法机关,并补偿北京分贝通科技有限公司的经济损失以及挽回对分贝通科技有限公司企业形象造成的影响



                                     分贝通-水镜
                                     2017.11.19

                         


