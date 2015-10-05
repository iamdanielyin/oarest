#日程列表
>按开始时间顺序排列

| 接口名称 | *日程列表* |
| -- | -- |
| **接口地址** | */schedule* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|是|0本日日程，1本月日程|无|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|日程数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|startdate|开始时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|enddate|结束时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|

##接口示例

```
暂无
```




#日程详情
>暂无

| 接口名称 | *日程详情* |
| -- | -- |
| **接口地址** | */schedule/{id}* |
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


参数项：creator、approver

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：customers

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|客户ID|<code>string</code>|是|暂无|无|
|name|公司名称|<code>string</code>|是|暂无|无|

参数项：tasks

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|任务ID|<code>string</code>|是|暂无|无|
|title|任务名称|<code>string</code>|是|暂无|无|

参数项：images

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|image|图片链接|<code>string</code>|是|暂无|无|


参数项：files

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|file|附件链接|<code>string</code>|是|暂无|无|

##接口示例

```
暂无

```





#新增日程
>日程不能提交给自己审批


| 接口名称 | *新增日程* |
| -- | -- |
| **接口地址** | */schedule* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|
|approver|审批人ID|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|mcoin|M币|<code>digit</code>|是|暂无|无|
|starval|星值|<code>digit</code>|是|暂无|无|
|type|日程类型|<code>digit</code>|是|0日报，1周报，2月报|无|
|customers|关联客户|<code>string</code>|否|客户ID，多个用英文逗号分隔|无|
|tasks|关联任务|<code>string</code>|否|任务ID，多个用英文逗号分隔|无|
|images|日程图片|<code>string</code>|否|图片链接，多个用英文逗号分隔|无|
|files|日程附件|<code>string</code>|否|文件链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***







#删除日程
>接口描述

| 接口名称 | *删除日程* |
| -- | -- |
| **接口地址** | */schedule/{id}* |
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





#日程提醒
>只有日程指定审批人且该用户拥有审批权限才能审批日程

| 接口名称 | *日程提醒* |
| -- | -- |
| **接口地址** | */schedule/{id}/reminder* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***
