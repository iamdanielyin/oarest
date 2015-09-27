#本月信息
>CRM主页获取数据的接口

| 接口名称 | *CRM本月信息* |
| -- | -- |
| **接口地址** | /crm/home |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
* [<公共传入参数>](../README.md)

##返回参数
* [<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|monthdeal|本月成交|<code>string</code>|是|暂无|无|
|monthtarget|本月目标|<code>string</code>|是|暂无|无|
|monthback|本月回款|<code>string</code>|是|暂无|无|

##接口示例

```
暂无

```

***

#效率统计
>这里是接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|mobile|手机号|<code>string</code>|是|暂无|无|
|mobile|手机号|<code>string</code>|是|暂无|无|
|mobile|手机号|<code>string</code>|是|暂无|无|

##返回参数
|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:--|:--|---|
|mobile|手机号|<code>string</code>|是|暂无|无|
|mobile|手机号|<code>string</code>|是|暂无|无|
|mobile|手机号|<code>string</code>|是|暂无|无|

##接口示例

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
#CRM主页
>这里是接口描述

| 接口名称 | *CRM主页* |
| -- | -- |
| **接口地址** | /home |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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

#效率统计
>这里是接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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
#CRM主页
>这里是接口描述

| 接口名称 | *CRM主页* |
| -- | -- |
| **接口地址** | /home |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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

#效率统计
>这里是接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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
#CRM主页
>这里是接口描述

| 接口名称 | *CRM主页* |
| -- | -- |
| **接口地址** | /home |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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

#效率统计
>这里是接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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
#CRM主页
>这里是接口描述

| 接口名称 | *CRM主页* |
| -- | -- |
| **接口地址** | /home |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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

#效率统计
>这里是接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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
#CRM主页
>这里是接口描述

| 接口名称 | *CRM主页* |
| -- | -- |
| **接口地址** | /home |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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

#效率统计
>这里是接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |





##请求参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##返回参数
|编码|名称|类型|说明|默认值|
|:---|:---|:---|:---|:-----|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|
|mobile|手机号|<code>string</code>|暂无|无|

##接口示例

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
