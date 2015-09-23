#CRM信息
##CRM


###CRM主页
>**CRM相关交互接口**

####接口描述
| 接口地址 | */home* |
| -- | -- |
| **请求方式** | <code>GET</code> |





####请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

####返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

####接口示例

```
POST /2013-12-26/Accounts/297e7c37446272f301/IM/PushMsg?sig=C1F20E7A97 HTTP/1.1
Accept:application/json;
Content-Type:application/json;charset=utf-8;
Authorization:ZmY4MDgwODEzYzM3ZGE1MzAxM2M4MDRmODA3MjAwN2M6MjAxMzAyM=

{
  "pushType":"1",
  "appId":"2aabdefff0",
  "sender":"13291217102",
  "receiver":["18201370642","13121353225"],
  "msgType":"1",
  "msgContent":"你好",
  "msgDomain":"yuntongxun",
  "msgFileName":"",
  "msgFileUrl":""
}
```

***

###效率统计
>**效率统计交互接口**

####接口描述
| 接口地址 | */home* |
| -- | -- |
| **请求方式** | <code>GET</code> |





####请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

####返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

####接口示例

```
POST /2013-12-26/Accounts/297e7c37446272f301/IM/PushMsg?sig=C1F20E7A97 HTTP/1.1
Accept:application/json;
Content-Type:application/json;charset=utf-8;
Authorization:ZmY4MDgwODEzYzM3ZGE1MzAxM2M4MDRmODA3MjAwN2M6MjAxMzAyM=

{
  "pushType":"1",
  "appId":"2aabdefff0",
  "sender":"13291217102",
  "receiver":["18201370642","13121353225"],
  "msgType":"1",
  "msgContent":"你好",
  "msgDomain":"yuntongxun",
  "msgFileName":"",
  "msgFileUrl":""
}
```

***