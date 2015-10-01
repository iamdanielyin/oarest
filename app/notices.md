#公告列表
>按时间逆序排列

| 接口名称 | *公告列表* |
| -- | -- |
| **接口地址** | */notices* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|公告数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|公告标题|<code>string</code>|是|暂无|无|
|content|公告内容|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|

##接口示例

```
GET /oa/tasks?tt=1&vn=1.0&access_token=MTgxOWI5MzMtYTcwMy00ZDQ1LWEwN2YtN2Y1ZGIxYWFhYjJm HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"creator":{
				"header":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
				"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
				"realname":"李四"
			},
			"createtime":"2015-09-29 17:51:32",
			"enddate":"2015-10-01 00:00:00",
			"operators":[
				{
					"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
					"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
					"isremind":false,
					"realname":"张三"
				},
				{
					"header":"http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
					"id":"d47539b3-9820-4086-9582-f629d2ef0630",
					"isremind":false,
					"realname":"王五"
				}
			],
			"id":"243d6cd4-629b-4da8-98ac-ee1addbee2e6",
			"startdate":"2015-09-29 00:00:00",
			"title":"任务1",
			"content":"任务1内容描述",
			"status":0
		},
		{
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201508/12/20150812204032_eiAQk.thumb.224_0.jpeg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"赵丽"
			},
			"createtime":"2015-09-29 17:51:32",
			"enddate":"2015-10-01 00:00:00",
			"operators":[
				{
					"header":"http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
					"id":"d47539b3-9820-4086-9582-f629d2ef0630",
					"isremind":false,
					"realname":"王五"
				},
				{
					"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
					"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
					"isremind":false,
					"realname":"张三"
				}
			],
			"id":"d78ab909-7994-4fc0-8dc9-9200e749782c",
			"startdate":"2015-09-29 00:00:00",
			"title":"任务2",
			"content":"任务2内容描述",
			"status":0
		}
	],
	"usermsg":"正常"
}
```




#公告详情
>暂无

| 接口名称 | *公告详情* |
| -- | -- |
| **接口地址** | */notices/{id}* |
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
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|


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





#新增公告
>接口描述


| 接口名称 | *新增公告* |
| -- | -- |
| **接口地址** | */notices* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)


##接口示例

```
暂无

```

***







#删除公告
>接口描述

| 接口名称 | *删除公告* |
| -- | -- |
| **接口地址** | */notices/{id}* |
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
