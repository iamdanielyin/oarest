#日志列表
>按时间逆序排列

| 接口名称 | *日志列表* |
| -- | -- |
| **接口地址** | */worklogs* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|合同数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|公告标题|<code>string</code>|是|暂无|无|
|content|公告内容|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|

##接口示例

```
暂无

```




#日志详情
>暂无

| 接口名称 | *日志详情* |
| -- | -- |
| **接口地址** | */worklogs/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|approver|审批人|<code>object</code>|否|暂无|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|customer|关联客户|<code>object</code>|否|暂无|无|
|mcoin|M币|<code>digit</code>|是|暂无|无|
|starval|星值|<code>digit</code>|是|暂无|无|
|status|审批状态|<code>digit</code>|是|0未审，1通过，2不通过|无|
|type|日志类型|<code>digit</code>|是|0日报，1周报，2月报|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|


参数项：creator、approver

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：customer

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|name|公司名称|<code>string</code>|是|暂无|无|

##接口示例

```
暂无

```





#新增日志
>接口描述


| 接口名称 | *新增任务* |
| -- | -- |
| **接口地址** | */tasks* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|mcoin|任务M币|<code>digit</code>|否|暂无|0|
|starval|任务星值|<code>digit</code>|否|暂无|0|
|operators|执行人|<code>string</code>|是|用户ID，多个用英文逗号分隔|无|
|attachs|任务附件|<code>string</code>|否|文件链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)


##接口示例

```
暂无

```

***







#删除任务
>接口描述

| 接口名称 | *删除任务* |
| -- | -- |
| **接口地址** | */tasks/{id}* |
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

***
