#我
>暂无

| 接口名称 | *我* |
| -- | -- |
| **接口地址** | */briefing/me* |
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
|synergy|协同|<code>object</code>|是|暂无|无|
|others|其他|<code>object</code>|是|暂无|无|

参数项：synergy

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|logsno|日志数|<code>digit</code>|是|暂无|无|
|currmcoin|M币|<code>digit</code>|是|暂无|无|
|totalmcoin|历史M币|<code>digit</code>|是|暂无|无|
|curstarval|星值|<code>digit</code>|是|暂无|无|
|totalstarval|历史星值|<code>digit</code>|是|暂无|无|
|logindays|登录天数|<code>digit</code>|是|暂无|无|

参数项：others

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|monworkload|当月工作量|<code>string</code>|是|暂无|无|
|effic|工作效率|<code>string</code>|是|百分比，如30%|无|
|newcusts|新增客户量|<code>digit</code>|是|暂无|无|

##接口示例

```
暂无
```

#公司
>暂无

| 接口名称 | *公司* |
| -- | -- |
| **接口地址** | */briefing/company* |
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
|members|员工总数|<code>digit</code>|是|暂无|无|
|totalogs|日志总数|<code>digit</code>|是|暂无|无|
|monworkload|当月工作量|<code>string</code>|是|暂无|无|
|effic|工作效率|<code>string</code>|是|百分比，如30%|无|
|newcusts|新增客户数|<code>digit</code>|是|暂无|无|

##接口示例

```
GET /oa/briefing/company?tt=1&vn=1.0&access_token=OThlY2MwZTEtOWExMi00NzYxLTlhMTgtNzE0MDM2Y2M0ZGM1 HTTP/1.1
Host: 112.74.131.85
Cache-Control: no-cache
Postman-Token: 0866bbf6-0a03-5300-acc1-17c3b751f157
———————————————————————————————————————————————————————————
```


#荣誉墙
>暂无

| 接口名称 | *荣誉墙* |
| -- | -- |
| **接口地址** | */briefing/honorwall* |
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
|mcoin|当月M币最高|<code>object</code>|是|暂无|无|
|starval|当月星值最高|<code>object</code>|是|暂无|无|
|effic|工作效率最高|<code>object</code>|是|暂无|无|
|sum|签单金额最高|<code>object</code>|是|暂无|无|
|ontime|考勤准时率|<code>object</code>|是|暂无|无|

参数项：mcoin、starval、effic、sum、ontime

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/briefing/honorwall?tt=1&vn=1.0&access_token=OThlY2MwZTEtOWExMi00NzYxLTlhMTgtNzE0MDM2Y2M0ZGM1 HTTP/1.1
Host: 112.74.131.85
Cache-Control: no-cache
Postman-Token: c315c94f-4f9d-5ad8-2eb7-35a0d79aceec
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"mcoin":{
			"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
			"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
			"realname":"张三东"
		},
		"effic":{
			"header":"",
			"id":"46b61d83-6da1-4b4c-a064-14e6b9be8692",
			"realname":"asdfasd"
		},
		"ontime":{
			"header":"http://112.74.131.85:80/oa/upload/images/3e566fcb-49a2-4ba4-9d7f-644e4d01d0c2",
			"id":"d47539b3-9820-4086-9582-f629d2ef0630",
			"realname":"王老大"
		},
		"starval":{
			"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
			"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
			"realname":"张三东"
		},
		"sum":{
			"header":"http://112.74.131.85:80/oa/upload/images/3e566fcb-49a2-4ba4-9d7f-644e4d01d0c2",
			"id":"d47539b3-9820-4086-9582-f629d2ef0630",
			"realname":"王老大"
		}
	},
	"usermsg":"正常"
}
```


