#投票列表
>按开始时间顺序排列

| 接口名称 | *投票列表* |
| -- | -- |
| **接口地址** | */votes* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|投票数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|投票标题|<code>string</code>|是|暂无|无|
|status|投票状态|<code>digit</code>|是|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|是|0单选，1多选|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```




#投票详情
>暂无

| 接口名称 | *投票详情* |
| -- | -- |
| **接口地址** | */votes/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  


##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|数据详细|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|投票标题|<code>string</code>|是|暂无|无|
|content|投票描述|<code>string</code>|是|暂无|无|
|status|投票状态|<code>digit</code>|是|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|是|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|options|选项数组|<code>array</code>|是|暂无|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：options

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|option|选项|<code>string</code>|是|暂无|无|
|times|投票人数|<code>digit</code>|是|暂无|无|

##接口示例

```
暂无

```





#新增投票
>需【投票管理】权限


| 接口名称 | *新增投票* |
| -- | -- |
| **接口地址** | */votes* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|投票标题|<code>string</code>|是|唯一|无|
|content|投票描述|<code>string</code>|是|暂无|无|
|type|投票类型|<code>digit</code>|是|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|options|选项字符串|<code>string</code>|是|多个由英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***







#修改投票
>只需传入需要修改的资料项即可，需【投票管理】权限

| 接口名称 | *修改投票* |
| -- | -- |
| **接口地址** | */votes/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|投票标题|<code>string</code>|否|唯一|无|
|content|投票描述|<code>string</code>|否|暂无|无|
|status|投票状态|<code>digit</code>|否|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|否|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|否|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|否|yyyy-MM-dd|无|
|options|选项字符串|<code>string</code>|否|多个由英文逗号分隔，请提供所有选项|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***









#我要投票
>暂无

| 接口名称 | *我要投票* |
| -- | -- |
| **接口地址** | */votes/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|投票标题|<code>string</code>|否|唯一|无|
|content|投票描述|<code>string</code>|否|暂无|无|
|status|投票状态|<code>digit</code>|否|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|否|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|否|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|否|yyyy-MM-dd|无|
|options|选项字符串|<code>string</code>|否|多个由英文逗号分隔，请提供所有选项|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***





#删除投票
>接口描述

| 接口名称 | *删除投票* |
| -- | -- |
| **接口地址** | */votes/{id}* |
| **请求方式** | <mark>DELETE</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无


```