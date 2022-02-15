# 三方广告平台ADN Report API开通指南

当前，ADmobile已支持部分三方广告平台的Report API功能设置。开发者向三方广平台申请开通Report API权限后，可以在ADmobile开发者后台填入相应参数，ADmobile会自动拉取对应广告平台的表报数据。

## ADmobile 后台ADN Report API添加方法
1. 在【**开发者平台-广告平台-平台账号管理**】页面，点击添加，可对三方平台的API参数进行添加。
![4apitianjia](../images/10.0/4apitianjia.png)

2. 添加完成后，可以在页面中设置API的开关，以及修改相应参数。
![5apishezhi](../images/10.0/5apishezhi.png)

3. 若关闭“状态”开关，则API将终止从三方平台调取数据。
4. 另外，在**聚合管理-新增广告源**时，也可配置Report API，具体可参考[绑定广告平台并添加广告源](../1-使用指南/2-绑定广告平台并创建广告源.md)栏目。

## 三方ADN平台Report API开通方法

### 优量汇
开通优量汇的Report API权限，需要获得优量汇平台的**账号 ID、Secret Key** 。开发者可将账户ID、账户名称、申请理由等信息发送到优量汇的官方邮箱**ADNET@tencent.com**进行申请。

### 穿山甲
开通穿山甲的Report API权限，可以通过商务对接，获得穿山甲平台的**RoleId、SecurityKey**   

### 快手
开通快手的Report API权限，可以通过商务对接，获得快手平台的**Access Key、Security Key**   

### inmobi
开通inmobi的Report API权限，需要获得inmobi平台的：**Publisher ID、Access Token**。可以从下图的位置处获取，图中右上角处即为Publisher ID，API Key即为Access Token
![7inmobi](../images/10.0/7inmobi.png)

### 汇量
开通汇量(Mintegral)的Report API 权限，需要获得汇量平台的：**Skey、Secret**。可以从下图的位置处获取：
![6huiliang](../images/10.0/6huiliang.png)

### 华为联盟
1. 开通华为联盟的Report API 权限，请先进入“我的API”页面，点击“申请新的HMS API服务”。
![huawei1.png](../images/10.0/huawei1.png)

2. 下拉找到“广告服务”，点击“流量变现服务报表API”。
![huawei2.png](../images/10.0/huawei2.png)

3. 点击“启用”，可以开始使用流量变现服务报表API。
![huawei3.png](../images/10.0/huawei3.png)

4. 进入**凭证**页面，选择指定App并创建OAuth2.0客户端ID，在如下图页面中，获得华为联盟的：**客户端ID、密钥**。
![huawei4.png](../images/10.0/huawei4.png)


