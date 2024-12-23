登录 --> 填写个人信息（选择是用户还是陪诊员），合约存储信息，进行注册 --> 首页

首页（用户端）：
地图上标注当前人位置以及周边医院，下面给出医院列表。
点击医院进入详情，列出相关的陪诊师。点击可继续查看陪诊师详情



注册：合约保存陪诊师和用户信息

registry.sol:保存姓名，手机，邮箱，生日

下单：合约需要保存订单信息，收取押金到合约中


结算：付尾款，评分
erc20的合约


我想实现一个solidity合约，他大致可拆分成两部分。registry.sol：此合约用于用户注册，注册时选择身份(普通用户和陪诊员)，合约有对应结构体保存两种身份的用户信息，提供常用的查询接口。用户信息主要有：评分、名字、生日、手机号、邮箱；陪诊员会有单价。order.sol:此合约用于保存订单信息。用户在选择陪诊员后可进行下单，填写订单开始结束时间、对应医院、手机号、留言和押金(陪诊员单价的20%)。当订单完成，用户需要进行结算，付清尾款并对陪诊员进行打分，分数要及时更新到关联的陪诊员。请给出示例代码，尽可能使用比较新的solidity版本
