#审批列表
>先按审批状态排序，未审的在前面；再按创建时间逆序排列；每个用户只能查询到和自己相关的审批信息

| 接口名称 | *审批列表* |
| -- | -- |
| **接口地址** | */approvals/contracts* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|是|0我的申请，1我的审批|无|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|审批数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|customer|客户|<code>string</code>|是|暂无|无|
|totalamount|总金额|<code>string</code>|是|暂无|无|
|signdate|签约日期|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|headcontractor|合同负责人|<code>string</code>|是|暂无|无|
|ourcontractor|我方签约人|<code>string</code>|是|暂无|无|
|custcontractor|客户签约人|<code>string</code>|是|暂无|无|
|paymethod|支付方式|<code>string</code>|是|暂无|无|
|cno|合同编号|<code>string</code>|是|暂无|无|
|content|合同正文|<code>string</code>|是|暂无|无|
|approver|审批人|<code>object</code>|是|暂无|无|
|status|审批状态|<code>digit</code>|是|0未审，1通过，2不通过|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|images|合同图片|<code>object</code>|否|暂无|无|

参数项：approver、creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：images

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|image|图片链接|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```



#审批详情
>暂无

| 接口名称 | *审批详情* |
| -- | -- |
| **接口地址** | */approvals/contracts/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|审批详情|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|customer|客户|<code>object</code>|是|暂无|无|
|totalamount|总金额|<code>number</code>|是|暂无|无|
|signdate|签约日期|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|headcontractor|合同负责人|<code>object</code>|否|暂无|无|
|ourcontractor|我方签约人|<code>object</code>|否|暂无|无|
|custcontractor|客户签约人|<code>object</code>|否|暂无|无|
|paymethod|支付方式|<code>string</code>|是|0支票，1现金，2网上转账，3其他|无|
|cno|合同编号|<code>string</code>|是|暂无|无|
|content|合同正文|<code>string</code>|是|暂无|无|
|approver|审批人|<code>object</code>|是|暂无|无|
|status|审批状态|<code>digit</code>|是|0未审，1通过，2不通过|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|images|合同图片|<code>object</code>|否|暂无|无|

参数项：customer

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|客户ID|<code>string</code>|是|暂无|无|
|name|公司名称|<code>string</code>|是|暂无|无|

参数项：approver、creator、headcontractor、ourcontractor、custcontractor

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：images

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|image|图片链接|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```





#新增审批
>审批人不能为自己


| 接口名称 | *新增审批* |
| -- | -- |
| **接口地址** | */approvals/contracts* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|customer|客户ID|<code>string</code>|是|暂无|无|
|totalamount|总金额|<code>number</code>|是|暂无|无|
|signdate|签约日期|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|headcontractor|合同负责人ID|<code>string</code>|否|暂无|无|
|ourcontractor|我方签约人ID|<code>string</code>|否|暂无|无|
|custcontractor|客户签约人ID|<code>string</code>|否|暂无|无|
|paymethod|支付方式|<code>digit</code>|是|0支票，1现金，2网上转账，3其他|无|
|cno|合同编号|<code>string</code>|是|暂无|无|
|content|合同正文|<code>string</code>|是|暂无|无|
|approver|审批人ID|<code>string</code>|是|暂无|无|
|images|合同图片链接|<code>string</code>|否|图片链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***







#删除审批
>接口描述

| 接口名称 | *删除审批* |
| -- | -- |
| **接口地址** | */approvals/contracts/{id}* |
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





#执行审批
>只有审批指定审批人且该用户拥有审批权限才能审批审批，具有该审批权限的人必须同时具有新建任务的权限，因为合同审批通过后，会推送一个任务让合同的发起人去执行。

| 接口名称 | *审批审批* |
| -- | -- |
| **接口地址** | */approvals/contracts/{id}* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|isfinish|是否通过|<code>boolean</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***
