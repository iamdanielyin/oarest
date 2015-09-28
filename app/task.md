#任务列表
>按时间逆序排列

| 接口名称 | *任务列表* |
| -- | -- |
| **接口地址** | */tasks* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|是|0全部，1上级任务，2协同工作，3下属工作，4未汇报，5提醒|0|

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|合同数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|任务ID|<code>string</code>|是|暂无|无|
|user|发表人|<code>object</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|暂无|无|
|status|任务状态|<code>string</code>|是|暂无|无|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|operators|执行人|<code>array</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：operators

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像|<code>string</code>|是|暂无|无|


##接口示例

```
暂无

```






***

#任务明细
>接口描述


| 接口名称 | *任务明细* |
| -- | -- |
| **接口地址** | */tasks/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|status|任务状态|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|reportdate|汇报时间|<code>string</code>|是|暂无|无|
|finishdate|完成时间|<code>string</code>|是|暂无|无|
|mcoin|任务M币|<code>string</code>|是|暂无|无|
|starval|任务星值|<code>string</code>|是|暂无|无|
|isremind|是否提醒|<code>string</code>|是|暂无|无|
|isdailytask|是否日常任务|<code>string</code>|是|暂无|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|暂无|无|
|modifytime|最近修改时间|<code>string</code>|是|暂无|无|
|operators|执行人|<code>array</code>|是|暂无|无|
|attachs|任务附件|<code>array</code>|是|暂无|无|

参数项：creator、operators

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：attachs

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|file|文件链接|<code>string</code>|是|暂无|无|


##接口示例

```
暂无

```

***




#新增任务
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
|mcoin|任务M币|<code>string</code>|否|暂无|0|
|starval|任务星值|<code>digit</code>|否|暂无|0|
|operators|执行人|<code>string</code>|是|用户ID，多个用英文逗号分隔|无|
|attachs|任务附件|<code>string</code>|否|文件ID，多个用英文逗号分隔|无|

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
[<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|year|年份|<code>string</code>|是|暂无|无|
|month|月份|<code>string</code>|是|暂无|无|
|flag|查询标识|<code>int</code>|是|0个人，1部门，2部门或个人|无|

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|totalamount|合同总合计|<code>string</code>|是|暂无|无|
|contracts|合同数组|<code>array</code>|是|暂无|无|

>contracts

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|合同ID|<code>string</code>|是|暂无|无|
|name|合同名称|<code>array</code>|是|暂无|无|
|amount|合同总额|<code>string</code>|是|暂无|无|
|totalin|总收款|<code>string</code>|是|暂无|无|
|totalout|总支出|<code>array</code>|是|暂无|无|
|status|合同状态|<code>string</code>|是|暂无|无|

##接口示例

```
暂无

```

***