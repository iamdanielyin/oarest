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
|starttime|开始时间|<code>string</code>|否|yyyy-MM-dd HH:mm|当前时间|
|endtime|结束时间|<code>string</code>|否|yyyy-MM-dd HH:mm|明天的当前时间|



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
|starttime|开始时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|endtime|结束时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|

##接口示例

```
GET /oa/schedule?tt=1&vn=1.0&access_token=N2IyNjg5MGQtYmY3Zi00ODk4LWEyOTEtNTQ5MTcwYTk5YTcz&starttime=2015-10-20 00:00&password=123456&endtime=2015-10-20 23:59 HTTP/1.1
Host: 112.74.131.85
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"endtime":"2015-10-20 16:18",
			"id":"b8d15f74-9545-4dc2-9bd2-c1ce040f1354",
			"starttime":"2015-10-20 16:18",
			"title":"111"
		},
		{
			"endtime":"2015-10-20 16:19",
			"id":"8979e379-2be4-440b-9e75-a176bab60f77",
			"starttime":"2015-10-20 16:18",
			"title":"222"
		}
	],
	"usermsg":"正常"
}
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


##接口示例

```
GET /oa/schedule/663bc4ea-c0ea-4a70-acc6-59a707d02f5b?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz&starttime=2015-10-25 17:50&endtime=2015-10-26 18:30 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"createtime":"2015-10-25 16:29:39",
		"modifytime":"",
		"endtime":"2015-10-25 18:40",
		"remark":"",
		"id":"663bc4ea-c0ea-4a70-acc6-59a707d02f5b",
		"starttime":"2015-10-25 18:30",
		"title":"新增日程接口2",
		"isremind":false,
		"content":"日程内容222"
	},
	"usermsg":"正常"
}

```





#新增日程
>暂无


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
|starttime|开始时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|endtime|结束时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|isremind|是否提醒|<code>boolean</code>|否|暂无|false|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/schedule?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

title=新增日程接口2&content=日程内容222&starttime=2015-10-25 18:30&endtime=2015-10-25 18:40
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}
```

***







#修改日程
>只需传入需要修改的资料项即可

| 接口名称 | *修改日程* |
| -- | -- |
| **接口地址** | */schedule/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|否|唯一|无|
|content|内容|<code>string</code>|否|暂无|无|
|starttime|开始时间|<code>string</code>|否|yyyy-MM-dd HH:mm|无|
|endtime|结束时间|<code>string</code>|否|yyyy-MM-dd HH:mm|无|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
PATCH /oa/schedule/663bc4ea-c0ea-4a70-acc6-59a707d02f5b?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz&title=修改日程111222 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"usermsg":"正常"
}
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
DELETE /oa/schedule/663bc4ea-c0ea-4a70-acc6-59a707d02f5b?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"usermsg":"正常"
}
```