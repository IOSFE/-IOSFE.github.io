​

## 打包生成的苹果APP上架到苹果官方appstore商店的详细流程与教程

第一步：创建app发布证书以及配置文件

1、打开苹果开发者中心网站：https://developer.apple.com，点击右上角 Account 使用开发者账号登录，如下图所示：

![](https://img-blog.csdnimg.cn/img_convert/19b37de7f00e8101a89cd0d05a61869e.png)​


​

2、登录成功后，点击 Certificates, ldentifiers & Profiles，如下图所示：

![](https://img-blog.csdnimg.cn/img_convert/28d0371b6d290fe70f9019d46de14e3d.png)​



​

2. 点击进入 Certificates，Identifiers & Profiles

![](https://img-blog.csdnimg.cn/img_convert/d426e64842be7b2cc0c5411f2bf380e9.png)​


​

说明：因为这次需要的是发布app，所以证书需要选择的是Production版本，而开发测试的话是Development版本。

3. 在Identifers中创建App IDs

![](https://img-blog.csdnimg.cn/img_convert/93e0aecac2284da4e886e40190142dec.png)​



​

说明：APPid也叫包名，APPid必须是唯一的，不能包含特殊符号。填写AppID名称, 输入AppID Deion Name，用来描述您的AppID。（注意，必须输入英文）,下方App ID Suffix输 入Bundle ID：这是您AppID的后缀，这个需要仔细命名，因为这个内容和您的程序直接相关，很多地方都需要用到，最好是com.yourcompany.yourappname的格式。当然对于没有公司名的个人开发者，也可以用您自己的英文名字或者拼音。

![](https://img-blog.csdnimg.cn/img_convert/6fb34dc9695c39b2adbc5c75da0f844d.png)​



​

App Services服务选择推送服务

![](https://img-blog.csdnimg.cn/img_convert/7be5ccc6e0b4a464a3ee2fa245fa0994.png)​



​

说明：这里勾选“推送”服务，下一步“完成”。

第二步：导出本地证书文件

1、打开“应用程序”–>“实用工具”–>“钥匙串访问”–>“证书助理”中选择“从证书颁发机构请求证书”，如下图：

![](https://img-blog.csdnimg.cn/img_convert/33c68f66648cb076d4b9317206729cb3.png)​



2、选择从证书颁发机构请求证书，如下图：

![](https://img-blog.csdnimg.cn/img_convert/c0191493a7bde4c1dcadd04e8f1d80fb.png)​



​

3、打开后进入下图所示界面：

![](https://img-blog.csdnimg.cn/img_convert/befc7cba33dc5d53111b29a86a3ec4fa.png)​



“用户电子邮件地址”：必须填开发者账号所用的邮箱地址,

“常用名称”：用户可以自定义名称，建议直接填写APP名称，后面导出证书的时候容易分辨

选择存储到磁盘,点击“继续”。将本地证书文件文件保存到电脑中备用。

注：本地证书文件（即CSR文件），如下图样子：

![](https://img-blog.csdnimg.cn/img_convert/1db803539872f24d365ab921cc737562.png)​



第三步：创建发布证书

![](https://img-blog.csdnimg.cn/img_convert/57071b4c4995ac619622d325d2df493a.png)​



​

这里选择的类型是Production下的，然后选择 App Store and Ad Hoc.

![](https://img-blog.csdnimg.cn/img_convert/8e9a6a32e1ea3a79e664cce9d3edc269.png)​



​

选择本地的CSR请求文件，下一步“完成”。

5.创建推送证书：

![](https://img-blog.csdnimg.cn/img_convert/8c1da8dd99545cf49e12f4cece8ddb78.png)​



​

选择刚才创建的APPID

![](https://img-blog.csdnimg.cn/img_convert/eb16c0efd9d2181ef0940bec99f16030.png)​



​

下一步，选择本地生成的CSR文件。

![](https://img-blog.csdnimg.cn/img_convert/1294ab48cc27de10bf208b5262f64d81.png)​



第四步：创建配置文件

![](https://img-blog.csdnimg.cn/img_convert/c4e4148a6e41f816f7088678faaa4425.png)​



选择App Store，进入下一步。

![](https://img-blog.csdnimg.cn/img_convert/b3aea31190e9cf79eb8283e5a19dc9c9.png)​



选择刚才创建的APP ID

![](https://img-blog.csdnimg.cn/img_convert/eaf90d0eb0b19ee0827ddb4612edc9d1.png)​


​

选择创建好的发布证书，进入下一步。

![](https://img-blog.csdnimg.cn/img_convert/1b08520526c4e88f36b7b5baddf92d7a.png)​



​

填写配置文件，进入下一步“完成”，下载即可。

![](https://img-blog.csdnimg.cn/img_convert/362ba3e64253196d10855e7e30dcb0df.png)​



​

第五步：创建推送证书

![](https://img-blog.csdnimg.cn/img_convert/e5c386e81fc2e2435a41eed153456b09.png)​



​

至此，申请苹果证书步骤完成，我们得到三个有效的文件，如下图所示：

![](https://img-blog.csdnimg.cn/img_convert/3c7fb74bebb8cbb66be597984d7b95a9.png)​



​

可以看到上述证书，描述文件制作是非常复杂的。我们可以借助辅助工具appuploder，[一键制作证书描述文件](https://www.applicationloader.net/doc/hot/cert.html "一键制作证书描述文件")，还有[打包IPA上架](https://www.applicationloader.net/doc/hot/uploader.html "打包IPA上架")功能。

![](https://img-blog.csdnimg.cn/img_convert/97d5d9032ebc1dd9516b299f35747065.png)

APP Store上架需要注意以下几点：

1、不能有产品下载（非iOS，以及企业发布地址）的链接及二维码。2、不能带有升级的按钮以及提示。3、在app提交平台填上该网站的测试帐号。4、页面要保持简洁美观。5、网站不能出现测试页面、Beta等。

6、APP内容完善，不能访问各页面都是空的。

​
