## 接入指南
### 一、 接入需要客户端、服务端参与开发
### 二、 接入文档 [android](https://github.com/aiwuyu-sdk/aiwuyu-android-sdk)，[iOS](https://github.com/aiwuyu-sdk/aiwuyu-iOS-sdk)，[java](https://github.com/aiwuyu-sdk/aiwuyu-server-sdk)
### 三、 联合登录配置申请
#### 1、 邮件申请方式
* 将生成好的RSA公钥或者MD5密钥发送至 caojiayao001@aiwuyu.com
* 邮件发送模版
```
  商户名称：xx
  签名方式：RSA\MD5
  签名密钥：XXXXXXX
```
* 配置完成后会收到回执邮件，内容包含“渠道编码”信息
* RSA密钥生成可参考支付宝生成工具(https://docs.open.alipay.com/291/106097/)
### 四、 联合登录交互逻辑
![Image text](http://aiwuyu-cms-prd.oss-cn-hangzhou.aliyuncs.com/Pic/sdk-doc/union_login.png)

