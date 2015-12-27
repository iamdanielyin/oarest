# 移动OA项目接口文档

**接口整体描述：**

* 接口字符编码为UTF-8
* 访问所有非公共开放接口需上传access_token，access_token值具有时效性，超过有效时间后，需通过登录重新获取access_token，具体接口见报文定义。
* 时间字段如未额外标注，默认格式为:yyyy-MM-dd HH:mm:ss，例如2015-09-01 12:30:57
* 接口字段类型约定：
 * string，字符串，如：tes；
 * digit，整数，如：123；
 * number，浮点数，如：123.4；
 * boolean，布尔值，如：true/false；
 * object，对象，如：{"code":"编码"}；
 * array，数组，如：[ {"code":"编码1"},{"code":"编码2"} ]。
* 后台超级管理员账号：admin/admin123
* 测试用户账号：test1/123456、test2/123456、test3/123456、test4/123456
* 接口地址组成：http://{服务端地址}:{服务器端口}/{接口地址}
* 测试服务器地址：http://112.74.131.85:80/oa
* 所有接口的返回报文结构具有固定格式，具体如下所示  

返回对象数据时：
```
{
  "statuscode": "接口状态码",
  "statusmsg": "接口提示信息",
  "data": {  },
  "usermsg": "用户提示信息"
}
```

返回数组数据时：

```
{
  "statuscode": "接口状态码",
  "statusmsg": "接口提示信息",
  "data": [  ],
  "usermsg": "用户提示信息"
}
```
* 每个接口需上传公共参数，<font color=red>公共传入参数</font>如下所示：

|编码|名称|类型|必须|说明|默认|
|:---|:---|:---|:--:|:---|:-----|
|tt|终端类型|<code>digit</code>|是|1安卓，2iOS，3Web|无|
|vn|终端版本|<code>string</code>|是|暂无|无|
|access_token|访问令牌|<code>string</code>|否|登录接口除外|无|
* 每个接口将返回公共参数，<font color=red>公共返回参数</font>如下所示：

|编码|名称|类型|必须|说明|默认|
|:---|:---|:---|:--:|:---|:-----|
|statuscode|状态编码|<code>digit</code>|是|0000为正常，具体见《[接口状态码对照表](STATUSCODE.md)》|无|
|statusmsg|状态信息|<code>string</code>|是|暂无|无|
|usermsg|用户提示|<code>string</code>|是|暂无|无|
* 部分接口需上传翻页参数，<font color=red>公共翻页参数</font>如下所示：

|编码|名称|类型|必须|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|page|页码|<code>digit</code>|否|页码从0开始|0|
|size|每页大小|<code>digit</code>|否|暂无|20|

* 第三方账号

|平台|账号|密码|地址|
|:---|:---|:---|:---|
|环信|menghua-admin|menghuaadmin|http://www.easemob.com/|
|极光|menghua|menghuats|https://www.jpush.cn/|
|极光|menghua|menghuats|https://www.jpush.cn/|

