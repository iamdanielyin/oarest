# 移动OA
>移动OA项目REST接口文档

* 接口字符编码为UTF-8
* 每个接口需上传公共参数，<font color=red>公共传入参数</font>如下所示：

|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|tt|终端类型|<code>int</code>|1安卓，2iOS，3Web|无|
|vsn|终端版本|<code>string</code>|暂无|无|

* 每个接口将返回公共参数，<font color=red>公共返回参数</font>如下所示：

|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|statuscode|终端类型|<code>int</code>|1安卓，2iOS，3Web|无|
|statusmsg|状态信息|<code>string</code>|暂无|无|

* 有些接口需上传翻页参数，<font color=red>公共翻页参数</font>如下所示：

|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|page|页码|<code>int</code>|暂无|无|
|size|每页大小|<code>int</code>|暂无|无|