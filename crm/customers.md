#客户列表
>接口描述

| 接口名称 | *客户列表* |
| -- | -- |
| **接口地址** | */customers* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|keyword|关键字|<code>string</code>|否|暂无|无|
|status|客户状态|<code>string</code>|否|0初步沟通、1见面拜访、2确定意向、3正式招价、4签订,多个用英文逗号分隔|无|
|level|客户分级|<code>string</code>|否|0重要、1紧急、2普通、3重要且紧急,多个用英文逗号分隔|无|
|order|排序字段|<code>string</code>|否|创建时间顺序：createtime;创建时间逆序：-createtime;公司名称顺序：name：-name|createtime|


##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|客户数组|<code>array</code>|是|暂无|无|
|totalpgs|总页数|<code>digit</code>|是|暂无|无|
|totalels|记录总数|<code>digit</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|客户ID|<code>string</code>|是|暂无|无|
|name|公司名称|<code>string</code>|是|暂无|无|
|address|地址|<code>string</code>|否|暂无|无|
|site|网址|<code>string</code>|否|暂无|无|
|contact|联系人名称|<code>string</code>|否|暂无|无|
|tel|电话|<code>string</code>|否|暂无|无|
|status|客户状态|<code>string</code>|是|0初步沟通、1见面拜访、2确定意向、3正式招价、4签订|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|level|客户分级|<code>string</code>|是|0重要、1紧急、2普通、3重要且紧急|无|

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






***

#客户明细
>接口描述


| 接口名称 | *客户明细* |
| -- | -- |
| **接口地址** | */customers/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|客户数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|客户ID|<code>string</code>|是|暂无|无|
|name|公司名称|<code>string</code>|是|暂无|无|
|address|地址|<code>string</code>|否|暂无|无|
|site|网址|<code>string</code>|否|暂无|无|
|contact|联系人名称|<code>string</code>|否|暂无|无|
|tel|电话|<code>string</code>|否|暂无|无|
|status|客户状态|<code>string</code>|是|0初步沟通、1见面拜访、2确定意向、3正式招价、4签订|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|level|客户分级|<code>string</code>|是|0重要、1紧急、2普通、3重要且紧急|无|
|remark|备注|<code>string</code>|是|暂无|无|
|fax|传真|<code>string</code>|是|暂无|无|
|industry|hang|<code>string</code>|是|暂无|无|
|comprofile|备注|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|


参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|username|用户名|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|headportrait|头像链接|<code>string</code>|是|暂无|无|

##接口示例

```
暂无

```

***




#新增客户
>接口描述


| 接口名称 | *新增客户* |
| -- | -- |
| **接口地址** | */customers* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|name|公司名称|<code>string</code>|是|唯一|无|
|address|地址|<code>string</code>|否|暂无|无|
|site|网址|<code>string</code>|否|暂无|无|
|contact|联系人名称|<code>string</code>|否|暂无|无|
|tel|电话|<code>string</code>|否|暂无|无|
|status|客户状态|<code>string</code>|否|0初步沟通、1见面拜访、2确定意向、3正式招价、4签订|0|
|level|客户分级|<code>string</code>|否|0重要、1紧急、2普通、3重要且紧急|2|
|remark|备注|<code>string</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无

```

***




#修改客户
>接口描述


| 接口名称 | *修改客户* |
| -- | -- |
| **接口地址** | */customers/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|name|公司名称|<code>string</code>|否|唯一|无|
|address|地址|<code>string</code>|否|暂无|无|
|site|网址|<code>string</code>|否|暂无|无|
|contact|联系人名称|<code>string</code>|否|暂无|无|
|tel|电话|<code>string</code>|否|暂无|无|
|status|客户状态|<code>string</code>|否|0初步沟通、1见面拜访、2确定意向、3正式招价、4签订|无|
|level|客户分级|<code>string</code>|否|0重要、1紧急、2普通、3重要且紧急|无|
|remark|备注|<code>string</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无

```

***



#删除客户
>接口描述

| 接口名称 | *删除客户* |
| -- | -- |
| **接口地址** | */customers/{id}* |
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