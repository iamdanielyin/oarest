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
|status|投票状态|<code>digit</code>|是|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|是|0单选，1多选|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/votes?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"id":"7308247c-1497-447d-a750-71acb8cdef0e",
			"title":"公开票选部门优秀代表",
			"type":0,
			"status":0
		},
		{
			"id":"80b6ad0c-4ad9-4d94-9e6b-47479396bd31",
			"title":"优秀员工",
			"type":0,
			"status":1
		},
		{
			"id":"ae61908f-7acd-46ef-8b09-35bfbae65e48",
			"title":"CEO",
			"type":0,
			"status":2
		}
	],
	"usermsg":"正常"
}
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
|title|投票标题|<code>string</code>|是|暂无|无|
|content|投票描述|<code>string</code>|是|暂无|无|
|status|投票状态|<code>digit</code>|是|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|是|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|options|选项数组|<code>array</code>|是|投票的选项数组|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：options

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|option|选项|<code>string</code>|是|暂无|无|
|times|投票人数|<code>digit</code>|是|暂无|无|

##接口示例

```
GET /oa/votes/80b6ad0c-4ad9-4d94-9e6b-47479396bd31?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"creator":{
			"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
			"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
			"realname":"张三东哦哦OK"
		},
		"createtime":"2015-10-25 13:38:49",
		"enddate":"2015-10-25 00:00:00",
		"modifytime":"2015-10-25 13:39:14",
		"options":[
			{
				"times":2,
				"option":"老太太"
			},
			{
				"times":1,
				"option":"习大大"
			},
			{
				"times":0,
				"option":"你妹妹"
			}
		],
		"remark":"",
		"id":"80b6ad0c-4ad9-4d94-9e6b-47479396bd31",
		"title":"优秀员工",
		"type":0,
		"startdate":"2015-10-25 00:00:00",
		"content":"投票",
		"status":1
	},
	"usermsg":"正常"
}

```





#新增投票
>需【投票管理】权限


| 接口名称 | *新增投票* |
| -- | -- |
| **接口地址** | */votes* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|投票标题|<code>string</code>|是|唯一|无|
|content|投票描述|<code>string</code>|是|暂无|无|
|type|投票类型|<code>digit</code>|是|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|options|选项字符串|<code>string</code>|是|多个由英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/votes?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

title=%E6%96%B0%E5%A2%9E%E6%8E%A5%E5%8F%A31&content=%E6%8E%A5%E5%8F%A3%E6%8F%8F%E8%BF%B0&type=0&startdate=2015-10-26&enddate=2015-10-29&options=%E9%80%89%E9%A1%B91%2C%E9%80%89%E9%A1%B92%2C%E9%80%89%E9%A1%B93%2C%E9%80%89%E9%A1%B94
```

***







#修改投票
>只需传入需要修改的资料项即可，需【投票管理】权限

| 接口名称 | *修改投票* |
| -- | -- |
| **接口地址** | */votes/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|投票标题|<code>string</code>|否|唯一|无|
|content|投票描述|<code>string</code>|否|暂无|无|
|status|投票状态|<code>digit</code>|否|0未开始，1进行中，2已结束|无|
|type|投票类型|<code>digit</code>|否|0单选，1多选|无|
|startdate|开始日期|<code>string</code>|否|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|否|yyyy-MM-dd|无|
|options|选项字符串|<code>string</code>|否|多个由英文逗号分隔，请提供所有选项|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

***









#我要投票
>不能重复投票，投票后也不能再取消，只能参与状态为进行中的投票

| 接口名称 | *我要投票* |
| -- | -- |
| **接口地址** | */votes/{id}/action* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|options|选项字符串|<code>string</code>|否|如果是单选投票，这里是单个字符串；如果是多选投票，这里是多个字符串，由英文逗号分隔|无|

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