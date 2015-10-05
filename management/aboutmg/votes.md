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


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|starttime|开始时间|<code>string</code>|否|yyyy-MM-dd HH:mm|当前时间|
|endtime|结束时间|<code>string</code>|否|yyyy-MM-dd HH:mm|明天的当前时间|



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
|content|投票描述|<code>string</code>|是|暂无|无|
|status|投票状态|<code>string</code>|是|暂无|无|
|type|投票类型|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|creator|创建人|<code>string</code>|是|暂无|无|
|remark|备注|<code>string</code>|是|暂无|无|
|createtime|更新时间|<code>string</code>|是|暂无|无|
|modifytime|最近修改时间|<code>string</code>|是|暂无|无|
|participants|参与人|<code>string</code>|是|暂无|无|

参数项：participants

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
|title|标题|<code>string</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|
|starttime|开始时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|endtime|结束时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|


##接口示例

```
暂无

```





#新增投票
>暂无


| 接口名称 | *新增投票* |
| -- | -- |
| **接口地址** | */votes* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|
|starttime|开始时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|endtime|结束时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|isremind|是否提醒|<code>boolean</code>|否|暂无|false|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***







#修改投票
>只需传入需要修改的资料项即可

| 接口名称 | *投票提醒* |
| -- | -- |
| **接口地址** | */votes/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|否|唯一|无|
|content|内容|<code>string</code>|否|暂无|无|
|starttime|开始时间|<code>string</code>|否|yyyy-MM-dd HH:mm|无|
|endtime|结束时间|<code>string</code>|否|yyyy-MM-dd HH:mm|无|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|

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