## 接入指南
### 一、 接入需要客户端、服务端参与开发
### 二、 接入文档 [android](https://github.com/aiwuyu-sdk/aiwuyu-android-sdk)，[iOS](https://github.com/aiwuyu-sdk/aiwuyu-iOS-sdk)，[java](https://github.com/aiwuyu-sdk/aiwuyu-server-sdk)
### 三、 联合登录配置申请
#### 1、 邮件申请方式
* 将生成好的RSA公钥或者MD5密钥发送至 caojiayao001@aiwuyu.com
* 邮件发送模版
```
  商户名称：xxxx
  签名方式：RSA\MD5
  签名密钥：XXXXXXX
```
* 配置完成后会收到回执邮件，内容如下
```
  渠道编码：xxxx
  首页地址：https://h5.aiwuyu.com/awy/index.html?channel=xxx#/index
```
* RSA密钥生成可参考支付宝生成工具(https://docs.open.alipay.com/291/106097/)
### 四、 联合登录交互逻辑
![Image text](http://aiwuyu-cms-prd.oss-cn-hangzhou.aliyuncs.com/Pic/sdk-doc/union_login.png)

### 五、 联调测试
#### RSA测试配置信息
```
  渠道Code：channel-test
  RSA私钥：MIIEvQIBADANBgkqhkiG9w0BAQEFAASCBKcwggSjAgEAAoIBAQCi2pFZiVy0ey9HX6X4+Hx8lVAIphu6nYLPOkYpG3mApKZsKyCoaezdQc9inuNENmFfDC66s9QWPj6vnjMgf2kQt2FULK1IbDaY6n+9Y6UejuQJhY+oy1p3VPPn6kTsVmm945V3kkvAHLyhAlxUA0oOQw99myOJevuDrCC79OFQ6p5t6ICr5i0kH1tkRt/E5Y7oH6dLzb9kDFQFUZZ6va71P6gEmbbXoyW8EAFlMRO2W0dBoI8xUqZxM+vpMhyh77nqTGYW20Kt6aeJAkfRGAhYkhiJzf0rMFo2U2hIqKVNT05HlJcBLydOyAefJxX2IM4csNkL/REX/DCMssy9dLNbAgMBAAECggEAAKnZS78WhJm34JeQKoqAn1VQZSigFkuL++Il5Qb6oL6K+wfV8zmzQFeDS8iP7ng2P1fiXNpcs9Z/FOIVHT3HpMzKdbhU4GWod0kFSjU8t/onDa7gnfRuIuxSrhAzRa84cRCbTEhpTJgRYKqMy77Tr2kwh/d41peMrMWnwHxH6rd4S/v5xSxDu08eqZvy/MuZ+c3QHd5keYsF2oQZyBTK1F1wjhoDF7sdv5MsR7RaWUUsjMIM4e+T0u00J5v2+YvIWbG11Z3blHz3fS81Hb5LXh9w9D1VQiBAlb0CkDivrlQaLto7zVEIwCnK9oK8L0gjdLopeIvpV0X9wonFoawvEQKBgQDxA5O7L15ujmd62e8GcHhV1OAlGfh5NX04DK9VM80YX+rHZO34pwP5WWdahFp/XbIEfnyD9aqs8IIqpcmaihyVvZ1oGeG8tBc4/Mp9VZBlY02PpHNMUklpTO4fnlaQP4M269U8LJiCFwBRJW9X1SQc3VMzVsZfhS8BLoFrnoayUwKBgQCs+tlSSa4wIdiA643ttajjWmblQaUBNcCWLl7agstHz49w4j5A1VXYTplzOHDlPzsr0PKH4/bToE7roUGYnVStyOj44XbwEjoBGXPoQKY2NqZCQCpF+u3uC1eSRWg6btgQsK5tep5AWrwWEIoDJXihE6CSz7GHNXqyN1SxO97p2QKBgQDPshJ0ZAzP315jqz1l4jSBWxLSRkAvTB4d2CiclyhukfIEZQECoAM3tYjwo1BNpFPNtabeHS45HIY/9GD5EX4yuJXWaT90XAoLLSXevobSKLJlUAWgRuVGnmoyy0OzyVftU2yOD6xZpzK5uzXpjh8x1LVnb6dCF8b7ELWtJY7USwKBgGva0OxE8q4iPFtOBCXGUfLIaEXj411YxacebJg0W0mAOoD5IDXOjwMbJwS3mXTnMx7D3qUqV7lmSC8VUdA1sRnWnqSn+EACLVaIJ0QWI0zEUHAYkAMoTXhSbBzQ2AcvG9t0Pp4WiVu493OOhm8lywwsL7+6bofOqZ07cLw9h2UpAoGANJqbcfzZxwAQipPqfLK4wuK8nEIquqo4grhNvyeK4ehbh8TnMHy3F6uLd7kzbvBiYFoRMtu0gcNHXCN2bXmhZdWIRdPsJqdBapW+r7Lu2ZrV6Bkawdg7ZcdQ33yHQP14cC9Tz66r32/T7agiYl/Y+t8VLLLScUWsyJhlnst8NOs=
  访问首页：https://test-h5.aiwuyu.com/awy/#/index
  网关地址：https://test-gateway.aiwuyu.com/sdkapi/invoke
```
