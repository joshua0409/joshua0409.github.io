---
enable html: true
---

# 绑定广告平台并添加广告源

## 简介

本文档旨在帮助媒体运营人、开发者在[ADmobile后台](http://app.admobile.top)关联绑定广告平台，并绑定对应的广告源。在进行广告平台绑定时请务必确认**您的应用已经通过审核**。<br>
注1：**广告源**是ADmobile聚合管理页面为避免名称重复，而对**三方平台广告位的别称**。<br>
注2：三方平台上的**广告位ID**，也就是本ADmobile广告聚合平台上的**广告源ID**。

- [绑定广告平台，新增广告源](#绑定广告平台，新增广告源)
- [获取三方平台的AppID](#获取三方平台的appid)   
- [获取三方平台的广告位ID](#获取三方平台的广告位id)  

下表为ADmobile 广告聚合SaaS接入各广告平台及接入需要必要参数。

| 广告平台                            | 操作系统        | 对应参数           | 备注      |
| ------------------------------- | ----------- | -------------- | ------- |
| [优量汇](#1、广点通)                | Android、iOS | APP ID         |      |
| [穿山甲toutiao](#2、穿山甲)            | Android、iOS | APP ID         |         |
| [inmobi](#3、inmobi)             | Android、iOS | APP ID         |         |
| [汇量Mintergral](#4、汇量mintergral) | Android、iOS | APP ID、APP Key |         |
| [快手ksad](#5、快手ksad)             | Android、iOS | APP ID         | 尚未开放注册  |
| [百度](#6、百度)                     | Android、iOS | APP ID         |         |
| [米盟](#7、米盟)                    | Android     | APP ID         |         |
|云码                              | Android、iOS | App ID、 账户ID  |  电商类为主   |  
| [华为广告联盟](../3-常见问题/5-HuweiPPS.md) | Android       |  App ID   | 仅支持华为手机  |
|爱奇艺 |   Android    |     Appid     |    视频类广告偏多    |

下表为三方平台支持的广告类型。

| 广告平台     | 操作系统        | 支持的广告样式            | 需要参数   |
| ---------------------- | ----------- | ---------------------------------- | ------ |
| [优量汇](#1、广点通)                | Android、iOS | 开屏广告、横幅广告、原生信息流、插屏广告、全屏视频(插屏广告 纯视频)、激励视频 | 广告位ID  |
| [穿山甲toutiao](#2、穿山甲)            | Android、iOS | 开屏广告、横幅广告、原生信息流、插屏广告、全屏视频、沉浸视频、激励视频      | 广告位ID  |
| [inmobi](#3、inmobi)             | Android、iOS | 横幅广告、原生信息流、插屏广告、全屏视频、激励视频                | 广告位ID  |
| [汇量Mintergral](#4、汇量mintergral) | Android、iOS | 原生信息流、插屏广告、全屏视频、激励视频                     | 广告位ID、 广告版位ID |
| [快手ksad](#5、快手ksad)             | Android、iOS | 开屏广告、原生信息流、全屏视频、沉浸视频、激励视频、 视频内容输出       | 广告位ID  |
| [百度](#6、百度)                     | Android、iOS | 开屏广告、横幅广告、原生信息流、插屏广告、激励视频                | 广告位ID  |
| [APPicAd](#9、appicad)          | Android     | 开屏广告、横幅广告、原生信息流、插屏广告、激励视频                | 广告位ID  |
| [米盟](#7、米盟)                    | Android     | 激励视频、插屏视频、原生信息流、系统开屏                       | 广告位ID  |
| 云码 |  Android、iOS      |  开屏广告、插屏广告、 横幅广告           |  广告位ID   |
|[华为广告联盟](../3-常见问题/5-HuweiPPS.md)| Android |横幅广告、插屏广告、全屏视频、激励视频、极速开屏   |  广告位ID |
| 爱奇艺 | Android  |       开屏广告、激励视频      | 广告位ID   |

## 绑定三方账号、广告平台以及新增广告源

1. 新建应用后，点击“聚合管理” ，进入聚合管理页面；
   ![1juheguanli](../images/2.0/1juheguanli.png)
2. 点击特定广告位下面的“增加广告源”按钮；
   ![2guanggaoyuan](../images/2.0/2guanggaoyuan.png)
3. 在新增广告源页面，选择**广告平台**后，若在网站的“**平台账号管理**”栏目未配置广告平台的账号信息，则会出现如下的**报表API配置**页面。请用户开通三方平台报表api后([如何开通三方平台报表API](../1-使用指南/10-ADNReport_API.md))，按下图中的参数填写对应的API密钥等值，使平台可以实现每天定时获取报表数据的功能，节约用户的数据上传时间；
   ![4apipeizhi](../images/2.0/4apipeizhi.png)
4. 若用户未开通三方平台报表API，或者选择了不支持报表API的平台，如下图，则只需填写相应的三方平台“账号”参数即可；
     ![5apipeizhi](../images/2.0/5apipeizhi.png)
5. 如上图，若用户没有真实的三方平台账户，则只需填写“**默认账户**”以作展示。
6. 填写后，点击下一步，可填入**应用ID**、**广告源ID**等参数，跟上一步填入的“**账号**”参数一一对应，点击保存，即完成账号、广告平台和广告源的绑定。
 ![3guanggaoyuanxinzeng2](../images/2.0/3guanggaoyuanxinzeng2.png)
7. 若用户已在网站的“**平台账号管理**”栏目配置了广告平台的账号信息，则选择**广告平台**后，会直接进入**广告源参数配置**页面，此时下拉选择跟**应用ID**对应的**账户**即可。
 ![6zhanghubangding](../images/2.0/6zhanghubangding.png)
**注意，在新增广告源页面：**
    - 点击“**+新增广告平台**”按钮，可以新增想要添加的三方广告平台。
    - 点击应用ID右侧的**修改**按钮，修改后，将影响当前应用下该平台所有广告位，若使用错误ID将无广告返回。
    - **“排序价格”参数**，即聚合管理页面的“价格”参数，是必填项，仅用于广告源瀑布流的优先级排序,并不会回传给广告平台;建议将一个符合实际的ecpm值填入此处。
    - **“自动价格”参数**，开启后，ADmobile会每天定时计算广告平台过去7天的平均ecpm值，并传到前端页面，用于广告源瀑布流排序;当数据过少时(7天平均展示数小于2000),仍使用人工填写的“排序价格”来进行排序。


## 获取三方平台的AppID及广告位ID

### 1、广点通

1. 登录广点通[优量汇后台](http://adnet.qq.com/)，在如下位置查看**App ID**。
   ![截屏2020-04-13 下午9.03.23](../images/2.1/gdt.png)
1. 将APP ID填入ADmobile 后台，关联广告平台对应应用上。
2. 在如下位置查看**广告位 ID**。
   ![gdtposid](../images/2.2/gdtposid.png)



### 2、穿山甲

1. 登录头条[穿山甲后台](https://partner.oceanengine.com/union/media/login/)，在如下位置查看**App ID**。
   ![chuanshajia](../images/2.1/chuanshajia.png)
1. 将APP ID填入ADmobile 后台，关联广告平台对应应用上。
2. 在如下位置查看**广告位 ID**。
   ![ttposid](../images/2.2/ttposid.png)

### 3、inmobi

1. 登录[inmobi后台](https://www.inmobi.cn/user/index?productId=1)，在如下位置查看**App ID**。
   ![inmobiappid](../images/2.1/inmobiappid1.png)
2. 在“MONETIZE”中点击应用，位置查看**广告位 ID**(Placement ID)。
   ![inmobiposid](../images/2.2/inmobiposid.png)   

### 4、汇量Mintergral

1. 登录[汇量Mintergral后台](https://dev.mintegral.com/user/login)，在如下位置查看**App ID** 和**App key**。
   ![mintegralappid](../images/2.1/mintegralappid.png)
1. 将APP ID填入ADmobile 后台，关联广告平台对应应用上。
2. 在“版位&广告单元”位置查看**Adunit ID**（广告单元ID）。
   ![mintegralposid](../images/2.2/mintegralposid.png)

### 5、快手ksad

1. 登录[快手联盟](https://ssp.e.kuaishou.com)，在如下位置查看**App ID** 。
   ![kuaishou](../images/2.1/kuaishou.png)
1. 将APP ID填入ADmobile 后台，关联广告平台对应应用上。
2. 在如下位置查看**广告位ID** 。
   ![kuaishouguanggaoweiid](../images/2.2/kuaishouguanggaoweiid.png)

### 6、百度

1. 登录[百度百青藤](https://mssp.baidu.com/bqt#/)，在如下位置查看**App ID** 。
   ![baiduAppid](../images/2.1/baiduAppid.png)
1. 将APP ID填入ADmobile 后台，关联广告平台对应应用上。
2. 在“代码位管理”下位置查看**ID** 。
   ![baiduposid](../images/2.2/baiduposid.png)


### 7、米盟

1. 登录[米盟](https://dev.mi.com/admob/fe/index.html)，在如下位置查看**App ID** 。
   ![mimengappid](../images/2.1/mimengappid.png)
   
2. 在“我的广告位”位置查看**广告位 ID** 。
   ![mimengguanggaoweiid](../images/2.2/mimengguanggaoweiid.png)
