灰雀小程序程序参考GO中文网小程序https://github.com/studygolang/go_small_wx

以下是灰雀小程序的大体文档


一 登录授权：
小程序：
个人信息页（“pages/login/login”）
最上面是授权登录（参考样例小程序）request  端口/login
在下面添加一栏完善个人信息（不强制）request  端口/user
完善个人信息页（pages/information/information）暂时选填手机号	request	端口/user
服务器：
授权登录	端口/login
个人信息	端口/user
UserInfo，手机号，家庭所在地（省市）
二 基金
小程序：
基金页（pages/fund/fund）
页面参照样例小程序（把四大块改成两块，分别是基金详情，获取帮助）
基金列表页（pages/fundDetail/fundDetail）
request 端口/fundDetail
fundClass []保存所有的基金的种类
基金的具体的内容

获取帮助页（pages/help/help）
填写个人具体信息（病情，联系方式等）request		POST	端口/help
GET		端口/user

服务器：
按照小程序相对应的内容设置相同变量的名




三 活动
小程序
活动页（pages/index/index）
Statistics_datas [] 保存使用小程序的人数，基金数，活动数 request  端口/stat/site

活动展示	request  端口/activity

点击每个活动进入对应活动页面（pages/activity/activity）	request	端口/activity



服务器端就看着小程序需要什么看着来点吧，变量名一样，requset的位置一样就行了


