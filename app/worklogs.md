#日志列表
>按时间逆序排列

| 接口名称 | *日志列表* |
| -- | -- |
| **接口地址** | */worklogs* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|是|0我的日志，1下属日志|无|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|日志数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|标题|<code>string</code>|是|暂无|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/worklogs?tt=1&vn=1.0&access_token=Y2U0MmRhODctYmEyMi00YjFjLTkwNDQtYWRhOWM0OGE1NTcy&flag=0 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Postman-Token: 969b1cef-f221-1823-33a7-e2663a09a427

———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"createtime":"2015-11-18 00:08:56",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"76d00c70-e3af-484d-b04c-b8cfb3631620",
			"title":"Hhgg",
			"content":"Hh"
		},
		{
			"createtime":"2015-11-17 23:24:02",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"0a580d20-60d1-4070-aa81-eff42df1dff4",
			"title":"Hh",
			"content":"Hh"
		},
		{
			"createtime":"2015-11-07 23:24:35",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"45558b7c-c7bd-49f2-89c9-500f22c9c1da",
			"title":"噢你噢",
			"content":"童言无忌哟"
		},
		{
			"createtime":"2015-11-07 23:22:27",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"e98e139d-3f05-4406-9c0b-c1f9dc00cf2e",
			"title":"Jjjj",
			"content":"空咯喔"
		},
		{
			"createtime":"2015-10-23 11:54:44",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"4ae24351-ec7b-4b35-ac81-0669e59f233f",
			"title":"龙年",
			"content":"来咯"
		},
		{
			"createtime":"2015-10-17 19:04:05",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"9993d1ac-a026-48b2-a60e-3e2539044495",
			"title":"呵呵呵呵呵呵",
			"content":"大哭大哭开发开放分开可否"
		},
		{
			"createtime":"2015-10-14 20:10:51",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"655f0d9b-847d-4678-84dc-26361d0a79d0",
			"title":"魔域",
			"content":"来咯"
		},
		{
			"createtime":"2015-10-14 19:52:54",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"7a9a5a74-aa00-4a48-bc93-936cb2516338",
			"title":"你妹",
			"content":"你妹妹"
		},
		{
			"createtime":"2015-10-14 19:46:08",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"0d1c5df0-9f15-4d0e-aa32-59cffb2e9961",
			"title":"Cgv",
			"content":"Ccc"
		},
		{
			"createtime":"2015-10-14 19:39:06",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"8d5cbb12-3713-4ffd-ba29-2ac3d75943ef",
			"title":"Ghj",
			"content":"Gbb"
		},
		{
			"createtime":"2015-10-13 20:33:46",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"6b9742c6-b7e0-46a8-9369-926e3474184b",
			"title":"Vbb",
			"content":"Gvgh"
		},
		{
			"createtime":"2015-10-01 19:55:58",
			"creator":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东哦哦OK"
			},
			"id":"ec8f2320-c4f4-43e3-bae1-bf9d0294896f",
			"title":"日志1",
			"content":"日志1内容"
		}
	],
	"usermsg":"正常"
}
```




#日志详情
>暂无

| 接口名称 | *日志详情* |
| -- | -- |
| **接口地址** | */worklogs/{id}* |
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
|creator|创建人|<code>object</code>|是|暂无|无|
|approver|审批人|<code>object</code>|否|暂无|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|mcoin|M币|<code>digit</code>|是|暂无|无|
|starval|星值|<code>digit</code>|是|暂无|无|
|status|审批状态|<code>digit</code>|是|0未审，1通过，2不通过|无|
|type|日志类型|<code>digit</code>|是|0日报，1周报，2月报|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|customers|关联客户|<code>array</code>|否|暂无|无|
|tasks|关联任务|<code>array</code>|否|暂无|无|
|images|日志图片|<code>array</code>|否|暂无|无|
|files|日志附件|<code>array</code>|否|暂无|无|


参数项：creator、approver

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：customers

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|客户ID|<code>string</code>|是|暂无|无|
|name|公司名称|<code>string</code>|是|暂无|无|

参数项：tasks

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|任务ID|<code>string</code>|是|暂无|无|
|title|任务名称|<code>string</code>|是|暂无|无|

参数项：images

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|image|图片链接|<code>string</code>|是|暂无|无|


参数项：files

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|file|附件链接|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/worklogs/ec8f2320-c4f4-43e3-bae1-bf9d0294896f?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh&flag=1 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"approver":{
			"header":"http://img5.duitang.com/uploads/item/201508/12/20150812204032_eiAQk.thumb.224_0.jpeg",
			"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
			"realname":"赵丽"
		},
		"creator":{
			"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
			"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
			"realname":"张三"
		},
		"createtime":"2015-10-01 19:55:58",
		"images":[
			{
				"image":"http://img5.imgtn.bdimg.com/it/u=3572074785,265614668&fm=21&gp=0.jpg"
			},
			{
				"image":"http://img6.faloo.com/Picture/0x0/0/747/747488.jpg"
			},
			{
				"image":"http://pic1.nipic.com/2009-02-20/2009220135032130_2.jpg"
			}
		],
		"starval":"",
		"modifytime":"",
		"remark":"",
		"title":"日志1",
		"startdate":"2015-10-01 00:00:00",
		"type":0,
		"content":"日志1内容",
		"mcoin":"",
		"enddate":"2015-10-01 00:00:00",
		"files":[
			{
				"file":"http://p1.gexing.com/G1/M00/5E/34/rBACFFPd-YvQXYp1AALWXgyPrbM950_600x.jpg"
			},
			{
				"file":"http://p4.gexing.com/shaitu/20120922/1520/505d66aac9e7b.jpg"
			},
			{
				"file":"http://img.pconline.com.cn/images/upload/upc/tx/wallpaper/1307/10/c6/23169101_1373445265040.jpg"
			}
		],
		"id":"ec8f2320-c4f4-43e3-bae1-bf9d0294896f",
		"customers":[
			{
				"name":"公司1",
				"id":"2282a40e-c7eb-4b34-81a6-aa2efa1e6ad1"
			},
			{
				"name":"客户2",
				"id":"9005997f-8468-4f96-8e6a-06907dfb2038"
			}
		],
		"tasks":[
			{
				"id":"243d6cd4-629b-4da8-98ac-ee1addbee2e6",
				"title":"任务1"
			},
			{
				"id":"d78ab909-7994-4fc0-8dc9-9200e749782c",
				"title":"任务2"
			}
		],
		"status":0
	},
	"usermsg":"正常"
}

```





#新增日志
>日志不能提交给自己审批


| 接口名称 | *新增日志* |
| -- | -- |
| **接口地址** | */worklogs* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|是|暂无|无|
|content|内容|<code>string</code>|是|暂无|无|
|approver|审批人ID|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|mcoin|M币|<code>digit</code>|是|暂无|无|
|starval|星值|<code>digit</code>|是|暂无|无|
|type|日志类型|<code>digit</code>|是|0日报，1周报，2月报|无|
|customers|关联客户|<code>string</code>|否|客户ID，多个用英文逗号分隔|无|
|tasks|关联任务|<code>string</code>|否|任务ID，多个用英文逗号分隔|无|
|images|日志图片|<code>string</code>|否|图片链接，多个用英文逗号分隔|无|
|files|日志附件|<code>string</code>|否|文件链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/worklogs?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

title=日志接口5&content=日志接口内容&approver=d9a5648a-65dd-46ef-add8-4837795ce8b4&startdate=2015-10-01&enddate=2015-10-01&mcoin=1&starval=2&type=0&customers=2282a40e-c7eb-4b34-81a6-aa2efa1e6ad1%2C9005997f-8468-4f96-8e6a-06907dfb2038&tasks=243d6cd4-629b-4da8-98ac-ee1addbee2e6%2Cd78ab909-7994-4fc0-8dc9-9200e749782c&images=http%3A%2F%2Fp3.gexing.com%2Fshaitu%2F20120922%2F1519%2F505d6699e4347.jpg%2Chttp%3A%2F%2Fhiphotos.baidu.com%2F1985129%2Fpic%2Fitem%2Fd05c8ed3cc27b16e970a16b1.jpg&files=http%3A%2F%2Fimgsrc.baidu.com%2Fforum%2Fw%253D580%2Fsign%3Da574eb9cb07eca80120539efa1229712%2F16ff201f95cad1c8b0e3b1987f3e6709c83d5161.jpg

———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}
```

***







#删除日志
>接口描述

| 接口名称 | *删除日志* |
| -- | -- |
| **接口地址** | */worklogs/{id}* |
| **请求方式** | <mark>DELETE</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
DELETE /oa/worklogs/235e711c-5a04-40d8-b07f-b4ac2d0f8e64?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}


```





#日志审批
>只有日志指定审批人且该用户拥有审批权限才能审批日志

| 接口名称 | *日志审批* |
| -- | -- |
| **接口地址** | */worklogs/{id}/approvals* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|isfinish|是否通过|<code>boolean</code>|是|暂无|无|
|mcoin|M币|<code>digit</code>|否|暂无|默认为日志原M币|
|starval|星值|<code>digit</code>|否|暂无|默认为日志原星值|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/worklogs/d7374cfa-4b43-4264-ac8a-4dd6e86af020/approvals?tt=1&vn=1.0&access_token=NTNkNjE4NGMtM2NjMy00YWRkLTkzMzctNWI3ZTVhZTNlNDZj HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

isfinish=true
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}
```

***
