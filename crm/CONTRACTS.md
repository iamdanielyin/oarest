#合同列表
>接口描述

| 接口名称 | *合同列表* |
| -- | -- |
| **接口地址** | */contracts* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
* [<公共传入参数>](../README.md)
* [<公共翻页参数>](../README.md)

##返回参数
* [<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|合同数组|<code>array</code>|是|暂无|无|
|monthtarget|本月目标|<code>string</code>|是|暂无|无|
|monthback|本月回款|<code>string</code>|是|暂无|无|


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|合同数组|<code>array</code>|是|暂无|无|
|monthtarget|本月目标|<code>string</code>|是|暂无|无|
|monthback|本月回款|<code>string</code>|是|暂无|无|
##接口示例

```
暂无

```






***

#合同明细
>接口描述


| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */crm/efficiency* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
* [<公共传入参数>](../README.md)
* [<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|year|年份|<code>string</code>|是|暂无|无|
|month|月份|<code>string</code>|是|暂无|无|
|flag|查询标识|<code>int</code>|是|0个人，1部门，2部门或个人|无|

##返回参数
* [<公共返回参数>](../README.md)

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




#新增合同
>接口描述


| 接口名称 | *效率统计* |
| -- | -- |
| **接口地址** | */crm/efficiency* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
* [<公共传入参数>](../README.md)
* [<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|year|年份|<code>string</code>|是|暂无|无|
|month|月份|<code>string</code>|是|暂无|无|
|flag|查询标识|<code>int</code>|是|0个人，1部门，2部门或个人|无|

##返回参数
* [<公共返回参数>](../README.md)

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
* [<公共传入参数>](../README.md)
* [<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|year|年份|<code>string</code>|是|暂无|无|
|month|月份|<code>string</code>|是|暂无|无|
|flag|查询标识|<code>int</code>|是|0个人，1部门，2部门或个人|无|

##返回参数
* [<公共返回参数>](../README.md)

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
* [<公共传入参数>](../README.md)
* [<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|year|年份|<code>string</code>|是|暂无|无|
|month|月份|<code>string</code>|是|暂无|无|
|flag|查询标识|<code>int</code>|是|0个人，1部门，2部门或个人|无|

##返回参数
* [<公共返回参数>](../README.md)

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