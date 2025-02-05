# 新版可续签的Office 365开发者试用订阅：E5（附自动续订方法）

近年来，Office 365的开发者试用订阅（E3版本）因其仅一年的有效期而备受诟病。一旦到期，用户的数据将不复存在，这给许多开发者带来了不便。

## 新版Office 365开发者订阅的亮点

现在，微软推出了新版Office 365开发者试用订阅，有效期为90天，并且支持自动续订！这一改进不仅延长了使用时间，还大大减少了手动续订的麻烦。

### 官方教程
官方教程链接：[Office 365开发人员计划](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program)

## 如何加入Office 365开发人员计划

### 1. 注册Microsoft帐户
首先，使用您的Microsoft帐户或启用Azure Active Directory的电子邮件进行登录。

### 2. 填写国家和地区信息
登录后，填写您的国家和地区信息。

![填写国家和地区](https://bbtdd.com/img/2963754673603.webp)

### 3. 创建订阅
在填写基本信息后，选择创建订阅。请注意，选择的国家将决定您的OneDrive数据存储位置。例如，选择美国，数据将存储在美国的微软数据中心。

![创建订阅](https://bbtdd.com/img/3633869376116027.webp)

![填写域名](https://bbtdd.com/img/313911061211067.webp)

### 4. 手机号验证
填写手机号进行验证。

![手机号验证](https://bbtdd.com/img/04839711134.webp)

### 5. 添加许可证
注册完成后，需要为您的账号添加许可证，否则无法正常使用。

![添加许可证](https://bbtdd.com/img/64478570664.webp)

### 6. 管理许可证
点击“Go to subscription”，进入后台管理页面。在“管理” -> “用户” -> “活跃用户”中，点击您的用户名，然后在“许可证和用户”中添加许可证并应用。

![管理许可证](https://bbtdd.com/img/8352181676763.webp)

## 自动续订（保活）方法

### OneDrive API调用
目前，仅通过调用OneDrive API即可实现保活，前提是必须使用自己创建的API密钥。OneIndex程序是一个不错的选择。

![自动续订](https://bbtdd.com/img/4052842284637.webp)

### Outlook API调用
调用Outlook API后的第二天，订阅将自动续期。如果在到期前20-30天调用，续期将提前进行。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

## 总结
新版Office 365开发者试用订阅（E5版本）不仅延长了有效期，还支持自动续订，极大地提升了开发者的使用体验。通过调用OneDrive和Outlook API，用户可以轻松实现订阅的自动续订，确保数据的安全和持续使用。