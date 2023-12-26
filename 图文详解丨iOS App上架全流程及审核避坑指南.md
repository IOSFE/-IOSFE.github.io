​

##  图文详解丨iOS App上架全流程及审核避坑指南

App Store作为苹果官方的应用商店，审核严格周期长一直让用户头疼不已，很多app都“死”在了审核这一关，那我们就要放弃iOS用户了吗？当然不是！本期我们从iOS app上架流程开始梳理，详细了解下iOS app上架的那些事。

iOS app上架总体流程：

![](https://img-blog.csdnimg.cn/img_convert/2a4c4b6af1722be7c3a078c65f54b5ab.jpeg)​



​

1登录苹果开发者中心，注册开发者账号

如果你是第一次申请注册使用Apple ID登录苹果开发者网站，需要同意“苹果开发者协议”，提交请求，这个时候你的Apple ID 就已经成为了一个开发者的ID了。如图1-1：

苹果开发者中心网址：[https://developer.apple.com/](https://link.zhihu.com/?target=https://developer.apple.com/ "https://developer.apple.com/")

![](https://img-blog.csdnimg.cn/img_convert/38efdf6a23c486d8f421bf4e235bb3a3.jpeg)​



​

图1-1 同意苹果开发者协议并提交申请

2、申请付费开发者，加入苹果开发计划

![](https://img-blog.csdnimg.cn/img_convert/14b063273762b71f7aade00d2901971e.jpeg)​



​

图2-2 开始注册

![](https://img-blog.csdnimg.cn/img_convert/67ef4669564347d48cfb4694bbe2c27f.jpeg)​



​

图2-3 注册说明

补充说明2-1：

-   双重验证相关

苹果新规定Apple ID需开启双重验证才能注册开发者账号，所以在加入开发者之前需要根据提示开启设备进行双重验证；验证方法采用登录电脑上的iCloud根据提示进行验证（或者其他设备，如登录手机进行双重验证），以下是部分相关图片

![](https://img-blog.csdnimg.cn/img_convert/5d2395e2e97b08362b0291dc5e53a697.jpeg)​



​

图2-4 双重验证相关

![](https://img-blog.csdnimg.cn/img_convert/5624d919bfa8d17e1d35163384bfc383.jpeg)​



​

图2-5双重验证相关

![](https://img-blog.csdnimg.cn/img_convert/c5c668ecae4955f1b7b02e843ca89066.jpeg)​



​

图2-6 选择开发者类型

补充说明2-2：

-   Apple 开发者账号

1.  个人账号：个人申请用于开发 Apple App 所使用的账号，仅限于个人使用，可以在 App Store 发布应用，申请比较容易，￥688.00/年 ($99.00/year)。
1.  公司账号：以公司名义申请的开发者账号，用于公司内部的开发者共用，可以在 App Store 发布应用，申请流程相对麻烦，￥688.00/年 ($99.00/year)。
1.  企业账号：一般是公司规模在 500 人以上的企业，用于内部测试、分发应用的账号，不能在 App Store 发布应用，申请流程相对麻烦，￥1988/($299.00/year)。

-   不同开发者账号步骤与所需资料

![](https://img-blog.csdnimg.cn/img_convert/1fe85a7497858d1f9c3bd9d784c0bd66.jpeg)​



​

![](https://img-blog.csdnimg.cn/img_convert/4c361c24dbc6438c60925eb93fbed5fb.jpeg)​



​

填写详细的注册信息，统一相关协议，通过验证审核之后再次点击继续进入支付页面，具体步骤参考图2-7：

![](https://img-blog.csdnimg.cn/img_convert/517ee85555d6d912dcaee2a042c7d971.jpeg)​



​

图2-7 填写注册信息

![](https://img-blog.csdnimg.cn/img_convert/63e964e07172243b8f2d463d3e4b0b29.jpeg)​



​

图2-8 同意协议并且继续

![](https://img-blog.csdnimg.cn/img_convert/b4b16edef4240b768eae91eb07985ec1.jpeg)​



​

图2-9 注册等待验证通过

![](https://img-blog.csdnimg.cn/img_convert/4d90c53be2d6aaed37085def4229f675.jpeg)​


​

图2-10 支付

![](https://img-blog.csdnimg.cn/img_convert/98bb71a3e5a5f05903178be227465794.jpeg)​



​

图2-11 再次登录

![](https://img-blog.csdnimg.cn/img_convert/690418fe943cb09ea5e24f3ef90b466a.jpeg)​



​

图2-12 填写付费信息的页面

支付成功后，苹果会在48小时内对订单进行处理，之后可能会收到邮件要求到指定的页面上传身份证照片。

如果遇到任何问题，可以拨打苹果开发的售后服务电话4006701855。

补充说明2-3：

-   邓白氏DUNS的申请

邓白氏DUNS编码相当于公司在苹果公认的权威组织中注册了自己的身份证；可以点击相关链接先进行验证，没有可以直接申请。具体申请步骤可以参考百度经验：https://www.applicationloader.net/doc/appuploader/uniapp-pack.html
3创建证书

使用APICloud平台开发iOS应用需要用到几个证书，下面的图为各个证书使用的地方。接下来为各个证书的创建教程。

![](https://img-blog.csdnimg.cn/img_convert/1f9a0eb3b8e72c09c52358864bca853b.jpeg)​



​

![](https://img-blog.csdnimg.cn/img_convert/5f0ed73beeacca7308d3dc1c8fabcf9b.jpeg)​



​

4创建App ID

首先打开苹果开发网站，通过Account进入开发账户，如图：

![](https://img-blog.csdnimg.cn/img_convert/abadaa9c724bf0e0394035b6d3e31ad3.jpeg)​



登录成功后选择Certificates, Identifiers & Profiles（如果没有这一项请查看教程最开始的说明），如图：

![](https://img-blog.csdnimg.cn/img_convert/62ed99a2992e521862351ef189314e43.jpeg)​



​

如图，在左侧菜单选择Identifiers，然后点击添加按钮

![](https://img-blog.csdnimg.cn/img_convert/8f4debf2acc1e5e922054c7cb5358ecb.jpeg)​



​

选择App IDs，点击右上角的Continue按钮

![](https://img-blog.csdnimg.cn/img_convert/2ad6440e17a5a5c19745535674dacfb5.jpeg)​



​

在Bundle ID处选择Explicit，填写自己项目的ID，这里填写的ID即是控制台上传证书页面需要填写的App IDs

![](https://img-blog.csdnimg.cn/img_convert/64bc6b55bfba4d33f10ac7d153bc2d04.jpeg)​



​

如果应用需要使用推送功能，在下面的Capabilities列表中勾选上Push Notifications项，点击Continue

![](https://img-blog.csdnimg.cn/img_convert/7ba1bdfcc8a8596d870d7307297422d3.jpeg)​



​

确认信息无误后点击Register，完成创建。

![](https://img-blog.csdnimg.cn/img_convert/84e488f279a5a7d035a9ae683c8a9db8.jpeg)​



​

5云编译p12证书制作

若开发账号下已经存在certificate了可以跳过创建的步骤，一个账号下有一个certificate即可，多个应用可以共用。

###

生成certSigningRequest文件

如图，打开应用程序->实用工具->钥匙串访问

![](https://img-blog.csdnimg.cn/img_convert/6457b2c24692aa7c02c07708de6c8d7c.jpeg)​



​

如图，选择从证书颁发机构请求证书

![](https://img-blog.csdnimg.cn/img_convert/4861cec6175e2a6e39e14799772a2200.jpeg)​



​

接下来填写邮件地址，选择存储到磁盘，点击继续

![](https://img-blog.csdnimg.cn/img_convert/b760fee684002b447153b84f7dc5be20.jpeg)​



​

如图，保存文件到桌面。

![](https://img-blog.csdnimg.cn/img_convert/7a7f3d419ef41da7cb670c7191a1dfaa.jpeg)​



​


6云编译mobileprovision发布证书制作

这里以个人、公司账号创建App Store类型发布证书为例，企业账号创建In House类型发布证书类似。

###  App Store类型证书

​

如图，选择上面创建的App ID，点击添加bundle id

![](https://img-blog.csdnimg.cn/img_convert/dab0ffb965caef7960639cf2a956e374.png)

​

App Store证书只能用于发布应用到AppStore，不能安装在非越狱设备上面。如图，点击左侧菜单证书管理页面，然后点击创建按钮

​

![](https://img-blog.csdnimg.cn/img_convert/632c84e2984bfb6fe3cfdd2b35e3cc75.png)

选择App Store，点击Continue

输入证书名称，点击确认，完成创建

![](https://img-blog.csdnimg.cn/img_convert/3dd2b1d808666bd5922690613b8f6b84.png)​

7云编译mobileprovision测试证书制作

个人或公司账号生成的App Store类型mobileprovision证书，应用在没有发布到App Store之前只能在越狱设备上安装，若要在非越狱手机上面安装，则需要把设备udid添加到测试设备列表Devices里，并且生成Ad Hoc类型mobileprovision证书。

### ![](https://img-blog.csdnimg.cn/img_convert/35a28b0485d702acccfc751b46aaa661.png)​

获取设备udid

获取设备udid可以通过老版本iTunes获取（最新版本无法获取），macOS Catalina及更新系统则可以直接通过“访达”获取，另外也可以通过其它一些手机助手获取。

1、连接设备，如图，点击划线上面区域后，会展示出序列号及udid信息，然后点鼠标右键拷贝（拷贝的内容包含序列号、udid等，需手动再筛选udid）也可通过老版本iTunes获取。。

​

![](https://img-blog.csdnimg.cn/img_convert/50033c7c5f2140cd512f8a0e1b9de53f.png)​
​

2、通过老版本iTunes获取。打开iTunes，连接设备，如图，找到序列号，然后点击序列号，该栏会变成UDID，点击鼠标右键，拷贝UDID。

![](https://img-blog.csdnimg.cn/img_convert/ca725fb74d706f7dd2cee8e22105cd0a.jpeg)​



​

![](https://img-blog.csdnimg.cn/img_convert/66acf333d2a84915bcc0b394066ce5a8.jpeg)​



​

### 添加测试设备

如图选择左侧菜单Devices，点击添加按钮，输入Name和获取的UDID，点击Continue

​

![](https://img-blog.csdnimg.cn/img_convert/04a97e54c459557e155150174e4571e7.png)​

点击Register，最后点击Done，添加设备完成。

###

更多内容详见：https://www.applicationloader.net/doc/
8创建App

![](https://img-blog.csdnimg.cn/img_convert/a2cef7430c326c09fa2ffecc692b2509.jpeg)​



​

图6-1 进入iTunes Connect

![](https://img-blog.csdnimg.cn/img_convert/4f74e81943accf4a1c4c1822cc5d1fc3.jpeg)​



​

图6-2 新建App

补充说明6-1“名称”是新建的app在App Store中显示的名字；“SKU”可以填写当天日期外加一个编号即可，这是你为你的应用指定的一个标识符。

![](https://img-blog.csdnimg.cn/img_convert/841f3c3655642bca9dae6f85c7687e41.jpeg)​



​

图6-3 点击“1.0准备提交”填写App相关信息

接着添加预览图和屏幕快照，编写应用描述和关键词，设置应用图标编辑应用分级，应用图标必须提供1024×1024的图片且图片不能设置alpha通道（透明度）；应用分级是为了确定应用使用群体的年龄段。

补充说明6-2苹果官方对于app屏幕快照及预览的规范要求：

![](https://img-blog.csdnimg.cn/img_convert/f4ede5c26155180b9ff8dc9dcf07c784.jpeg)​



​

![](https://img-blog.csdnimg.cn/img_convert/4132a61264e50b97d5e93af6a4716625.jpeg)​


​

![](https://img-blog.csdnimg.cn/img_convert/c0fb923ac75fa3123c87b99e3ed95b72.jpeg)​


​

![](https://img-blog.csdnimg.cn/img_convert/66225ec405e94931b6dc7780a13e3bbd.jpeg)​


​

![](https://img-blog.csdnimg.cn/img_convert/66b52b99239d2ec048f7f8e873bd901e.jpeg)​

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://img-home.csdnimg.cn/images/20230724024159.png?origin_url=%3C%3E%20%22%E7%82%B9%E5%87%BB%E5%B9%B6%E6%8B%96%E6%8B%BD%E4%BB%A5%E7%A7%BB%E5%8A%A8%22&pos_id=img-H8OGufdE-1703566753248)

​

![](https://img-blog.csdnimg.cn/img_convert/c0675f62494babcf0e271d06599057bc.jpeg)​



​

![](https://img-blog.csdnimg.cn/img_convert/250a0b8e700e841c190555a7809baa0a.jpeg)​

![外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传](https://img-home.csdnimg.cn/images/20230724024159.png?origin_url=%3C%3E%20%22%E7%82%B9%E5%87%BB%E5%B9%B6%E6%8B%96%E6%8B%BD%E4%BB%A5%E7%A7%BB%E5%8A%A8%22&pos_id=img-tSwYLlw0-1703566753248)

​

注：如果你的应用中有需要登录后才能使用的功能那么就必须提供一个演示账号以供审核应用时使用。

![](https://img-blog.csdnimg.cn/img_convert/ca3304f61224331efb1618a6a3c1c90a.jpeg)​



​

图6-4 提供联系人信息和演示账号

![](https://img-blog.csdnimg.cn/img_convert/493e08194171d87ade4cd2fb79d0c4a6.jpeg)​



​

图6-5 选择发布方式并保存应用信息

注：根据自己情况选择，是否手动发布版本。

9打包IPA

APICloud平台直接云编译生成ipa包，下载下来用Transporter工具上传到AppStoreConnect。

App审核相关

苹果的三种审核机制

![](https://img-blog.csdnimg.cn/img_convert/164c9c016ac9ec501f427fa40caed5b5.jpeg)​



​

外媒 CNBC 在一篇关于苹果 App Store 如何审核App 的报道中分享了一些关于应用审核的细节。

报道称，目前 App Review 总部有 300 多名评审员，苹果的每个评审员每天大概需要审核 50 — 100 个应用程序，Watchtower 会跟踪每一个 App 的审核情况，以便回复开发者或通过开发者修改后重新提交审核时进行比对，同时也为苹果收集 App 质量相关数据。

对于评审员来讲，苹果为其制定了 SLA 的考核制度（服务级别协议），要求评审员在 24 小时内需要达到 50% 的应用完成审核，48 小时内需要达到 90% 的应用完成审核。苹果称，会有 40% 的 App 被拒审或更新被驳回，核查出相关问题，并反馈给开发者。在同时多维度考核数据时，SLA 会达到正常标准，低于正常值时，评审员会收到邮件通知进行警告。新闻报道地址：[https://www.cnbc.com/2019/06/21/how-apples-app-review-process-for-the-app-store-works.html](https://link.zhihu.com/?target=https://www.cnbc.com/2019/06/21/how-apples-app-review-process-for-the-app-store-works.html "https://www.cnbc.com/2019/06/21/how-apples-app-review-process-for-the-app-store-works.html")

苹果审核标准共分为五大类:安全、性能、业务、设计及法律，我们要严格按照审核标准来开发和提交我们的APP。当然，在提审之前还有一些准备工作需要确保完成好：

-   要确保APP没有明显的崩溃和错误。
-   确保APP的可用性和完整性,不能是演示APP或demo。
-   APP所有预览图、简介、关键词等都要是和产品业务相关的。
-   更新您的联系信息，以便 App Review 部门在需要时与您取得联系
-   提供有效的演示帐户和登录信息，以及审核所需要的资源。
-   APP启用后台服务，确保其在审核期间处于活动和可用状态
-   相关权限要说明其⽤用途，如果是壳上架或混淆代码，就更需要注意

官方审查指南：[https://developer.apple.com/app-store/review/guidelines/](https://link.zhihu.com/?target=https://developer.apple.com/app-store/review/guidelines/ "https://developer.apple.com/app-store/review/guidelines/")

下面是七麦数据统计的近30天的被拒条款统计，仅供参考。

![](https://img-blog.csdnimg.cn/img_convert/1d15e16b8b5bb92970cd3832a628619c.jpeg)​



​

​
