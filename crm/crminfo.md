#本月信息
>CRM主页获取数据的接口

| 接口名称 | *CRM本月信息* |
| -- | -- |
| **接口地址** | */crm/home* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|monthdeal|本月成交|<code>string</code>|是|暂无|无|
|monthtarget|本月目标|<code>string</code>|是|暂无|无|
|monthback|本月回款|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/crm/home?access_token=ZDY3ZjliMDktMjZjZC00NWVhLWFiNGEtMjgxNTkzMGU0YmY2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Postman-Token: db3e5691-149f-6e23-eab6-bc803f927098

———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"monthdeal":2.0E7,
		"monthback":"",
		"monthtarget":2022222
	},
	"usermsg":"正常"
}
```

***




#目标设定
>接口描述


| 接口名称 | *合同统计* |
| -- | -- |
| **接口地址** | */crm/monthplan* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|yearmonth|年月|<code>string</code>|是|yyyy-MM|无|
|targetamount|目标金额|<code>digit</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/crm/monthplan?access_token=ZDY3ZjliMDktMjZjZC00NWVhLWFiNGEtMjgxNTkzMGU0YmY2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Postman-Token: dfaad3cc-0730-70e5-2260-244f3d67963f
Content-Type: application/x-www-form-urlencoded

yearmonth=2015-09&targetamount=123456

———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"monthdeal":2.0E7,
		"monthback":"",
		"monthtarget":2022222
	},
	"usermsg":"正常"
}
```

***




#合同统计
>接口描述


| 接口名称 | *合同统计* |
| -- | -- |
| **接口地址** | */crm/contracts/count* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|year|年份|<code>string</code>|是|暂无|无|
|month|月份|<code>string</code>|是|暂无|无|
|flag|查询标识|<code>digit</code>|是|0个人，1部门，2公司|无|
|ids|ID信息|<code>string</code>|是|如果是按部门查询，那么这里是传部门ID；如果是用户查询，这里是传用户ID，多个用户用英文逗号分隔|无|

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
|totalin|总收款|<code>string</code>|是|暂无|无|
|totalout|总支出|<code>array</code>|是|暂无|无|
|status|合同状态|<code>digit</code>|是|0执行中,1执行中结束,2意外终止|无|

##接口示例

```
暂无

```

***

