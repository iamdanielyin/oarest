# 移动OA项目REST接口文档

接口整体描述

* 接口字符编码为UTF-8
* 访问所有非公共开放接口需上传access_token，access_token值具有时效性，超过有效时间后，需通过登录重新获取access_token，具体接口见报文定义。
* 时间字段如未额外标注，默认格式为:yyyy-MM-dd HH:mm:ss，例如2015-09-01 12:30:57
* 每个接口需上传公共参数，<font color=red>公共传入参数</font>如下所示：

|编码|名称|类型|必须|说明|默认|
|:---|:---|:---|:---:|:---|:-----|
|tt|终端类型|<code>int</code>|是|1安卓，2iOS，3Web|无|
|vsn|终端版本|<code>string</code>|是|暂无|无|

* 每个接口将返回公共参数，<font color=red>公共返回参数</font>如下所示：

|编码|名称|类型|必须|说明|默认|
|:---|:---|:---|:---:|:---|:-----|
|statuscode|状态编码|<code>int</code>|是|0000为正常，具体见《[接口状态码对照表](STATUSCODE.md)》|无|
|statusmsg|状态信息|<code>string</code>|是|暂无|无|
|usermsg|用户提示信息|<code>string</code>|是|暂无|无|

* 有些接口需上传翻页参数，<font color=red>公共翻页参数</font>如下所示：

|编码|名称|类型|必须|说明|默认值|
|:---|:---|:---|:---:|:---|:-----|
|page|页码|<code>int</code>|是|页码从0开始|无|
|size|每页大小|<code>int</code>|是|暂无|无|



