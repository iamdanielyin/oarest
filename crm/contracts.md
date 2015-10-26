#合同列表
>接口描述

| 接口名称 | *合同列表* |
| -- | -- |
| **接口地址** | */contracts* |
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
|id|合同ID|<code>string</code>|是|暂无|无|
|name|合同名称|<code>array</code>|是|暂无|无|
|amount|合同总额|<code>string</code>|是|暂无|无|
|status|合同状态|<code>string</code>|是|暂无|无|


##接口示例

```
暂无

```






***

#合同明细
>接口描述


| 接口名称 | *合同明细* |
| -- | -- |
| **接口地址** | */contracts/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|合同数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|customer|客户|<code>object</code>|是|暂无|无|
|totalamount|总金额|<code>number</code>|是|暂无|无|
|signdate|签约日期|<code>string</code>|是|yyyy-MM-dd|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|headcontractor|合同负责人|<code>object</code>|是|暂无|无|
|ourcontractor|我方签约人|<code>object</code>|是|暂无|无|
|custcontractor|客户签约人|<code>object</code>|是|暂无|无|
|paymethod|支付方式|<code>digit</code>|是|0支票，1现金，2网上转账，3其他|无|
|cno|合同编号|<code>string</code>|是|暂无|无|
|content|合同正文|<code>string</code>|是|暂无|无|
|status|合同状态|<code>digit</code>|是|0执行中，1执行中结束，2意外终止|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|

参数项：customer

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|name|名称|<code>string</code>|是|暂无|无|

参数项：headcontractor、ourcontractor、custcontractor、creator

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




#新增合同
>接口描述


| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */contracts* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|是|唯一|无|
|customer|客户|<code>string</code>|是|客户ID|无|
|totalamount|总金额|<code>number</code>|是|暂无|无|
|signdate|签约日期|<code>string</code>|是|yyyy-MM-dd|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|headcontractor|合同负责人|<code>string</code>|是|用户ID|无|
|ourcontractor|我方签约人|<code>string</code>|是|用户ID|无|
|custcontractor|客户签约人|<code>string</code>|是|用户ID|无|
|paymethod|支付方式|<code>digit</code>|是|暂无|无|
|cno|合同编号|<code>string</code>|是|暂无|无|
|content|合同正文|<code>string</code>|是|暂无|无|
|approver|审批人|<code>string</code>|是|暂无|无|
|images|合同图片|<code>string</code>|是|暂无|无|


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




#修改合同
>接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */crm/efficiency* |
| **请求方式** | <mark>GET</mark> |
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




#删除合同
>接口描述

| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */crm/efficiency* |
| **请求方式** | <mark>GET</mark> |
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


#合同回款列表
>接口描述

| 接口名称 | *合同回款列表* |
| -- | -- |
| **接口地址** | */contracts/{id}/receiving* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|回款数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|sum|金额|<code>number</code>|是|暂无|无|
|dbilldate|回款日期|<code>string</code>|是|yyyy-MM-dd|无|
|period|期次|<code>string</code>|是|暂无|无|



##接口示例

```
暂无

```


#合同支出列表
>接口描述

| 接口名称 | *合同支出列表* |
| -- | -- |
| **接口地址** | */contracts/{id}/spending* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|支出数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|sum|金额|<code>number</code>|是|暂无|无|
|dbilldate|支出日期|<code>string</code>|是|yyyy-MM-dd|无|
|period|期次|<code>string</code>|是|暂无|无|




##接口示例

```
暂无

```






#新增合同回款
>接口描述

| 接口名称 | *新增合同回款* |
| -- | -- |
| **接口地址** | */contracts/{id}/receiving* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|sum|金额|<code>number</code>|是|暂无|无|
|dbilldate|回款日期|<code>string</code>|是|yyyy-MM-dd|无|
|period|期次|<code>string</code>|是|期次不能重复且连续|无|

##返回参数
[<公共返回参数>](../README.md)



##接口示例

```
暂无

```


#新增合同支出
>接口描述

| 接口名称 | *新增合同支出* |
| -- | -- |
| **接口地址** | */contracts/{id}/spending* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|sum|金额|<code>number</code>|是|暂无|无|
|dbilldate|回款日期|<code>string</code>|是|yyyy-MM-dd|无|
|period|期次|<code>string</code>|是|期次不能重复且连续|无|

##返回参数
[<公共返回参数>](../README.md)



##接口示例

```
暂无

```