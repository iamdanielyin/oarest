#日志数排行
>暂无

| 接口名称 | *日志数排行* |
| -- | -- |
| **接口地址** | */rankinglist/worklogs* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)    
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|user|用户|<code>object</code>|是|暂无|无|
|amount|数量|<code>digit</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /rankinglist/worklogs?tt=1&vn=1.0&access_token=OThlY2MwZTEtOWExMi00NzYxLTlhMTgtNzE0MDM2Y2M0ZGM1 HTTP/1.1
Host: localhost:8080
Cache-Control: no-cache
Postman-Token: 452790a8-2b36-7d00-c1e3-83edb32d6fa1
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"amount":19,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东"
			}
		},
		{
			"amount":3,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/3e566fcb-49a2-4ba4-9d7f-644e4d01d0c2",
				"id":"d47539b3-9820-4086-9582-f629d2ef0630",
				"realname":"王老大"
			}
		},
		{
			"amount":2,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1451289319978.jpg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"赵丽22"
			}
		},
		{
			"amount":1,
			"user":{
				"header":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
				"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
				"realname":"李四"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"fb3cbe8f-09ad-40a2-bc27-798a944c1162",
				"realname":"11哈哈"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"46b61d83-6da1-4b4c-a064-14e6b9be8692",
				"realname":"asdfasd"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"4f093f84-4704-424a-a055-4be6d80332a5",
				"realname":"给你们"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"7d219460-56cd-4d60-a718-cb16c3396893",
				"realname":"飞翔"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"7d67eb45-d4b7-4ac0-84ea-3b3f979e5c28",
				"realname":"源源"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"80f639f8-e998-47fb-8781-7018c6952d54",
				"realname":"miser"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"87556163-f142-42a4-a5dc-50251c6af3ad",
				"realname":"t222"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"8c457eeb-6f28-42d0-a612-95582b34555f",
				"realname":"test8"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"0932ec38-057f-49b9-9550-545b52ba8277",
				"realname":"哈哈王"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/b1976ff6-7b36-46a7-8d55-4288058b6224",
				"id":"8d3cd5a5-d744-49cf-a60b-cfb5374080c5",
				"realname":"林鸿非"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"0b1665d6-ef7f-46ff-b771-dc69924ee50b",
				"realname":"Dghj"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1c9f6fc7-d750-4c8a-bafb-939306a47d72",
				"id":"96f5f7f9-483a-4a43-88b3-d0ad1c629c53",
				"realname":"网名"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"0cd455e1-fa64-4649-ba6b-e064f614bdf1",
				"realname":"成员"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"acfc1ae2-6687-4b14-a147-c0907b283ec2",
				"realname":"龙少"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"b736eefe-ea50-459c-89d5-95c48b5e2702",
				"realname":"123456"
			}
		},
		{
			"amount":0,
			"user":{
				"header":"",
				"id":"109cf0c6-a717-4af9-bb5b-1d588d5f2049",
				"realname":"test5"
			}
		}
	],
	"usermsg":"正常"
}

```

#当月工作量排行
>暂无

| 接口名称 | *当月工作量排行* |
| -- | -- |
| **接口地址** | */rankinglist/monworkload* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)    
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|user|用户|<code>object</code>|是|暂无|无|
|monworkload|工作量|<code>digit</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"fb3cbe8f-09ad-40a2-bc27-798a944c1162",
				"realname":"11哈哈"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"46b61d83-6da1-4b4c-a064-14e6b9be8692",
				"realname":"asdfasd"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"4f093f84-4704-424a-a055-4be6d80332a5",
				"realname":"给你们"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1451289319978.jpg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"我是哈哈哈123123"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"7d219460-56cd-4d60-a718-cb16c3396893",
				"realname":"飞翔"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"7d67eb45-d4b7-4ac0-84ea-3b3f979e5c28",
				"realname":"源源"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"80f639f8-e998-47fb-8781-7018c6952d54",
				"realname":"miser"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"87556163-f142-42a4-a5dc-50251c6af3ad",
				"realname":"t222"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"8c457eeb-6f28-42d0-a612-95582b34555f",
				"realname":"test8"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"0932ec38-057f-49b9-9550-545b52ba8277",
				"realname":"哈哈王"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/b1976ff6-7b36-46a7-8d55-4288058b6224",
				"id":"8d3cd5a5-d744-49cf-a60b-cfb5374080c5",
				"realname":"林鸿非"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"0b1665d6-ef7f-46ff-b771-dc69924ee50b",
				"realname":"Dghj"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1c9f6fc7-d750-4c8a-bafb-939306a47d72",
				"id":"96f5f7f9-483a-4a43-88b3-d0ad1c629c53",
				"realname":"网名"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"0cd455e1-fa64-4649-ba6b-e064f614bdf1",
				"realname":"成员"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"acfc1ae2-6687-4b14-a147-c0907b283ec2",
				"realname":"龙少"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"b736eefe-ea50-459c-89d5-95c48b5e2702",
				"realname":"123456"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"109cf0c6-a717-4af9-bb5b-1d588d5f2049",
				"realname":"test5"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/ba51279e-b5a8-4113-9d84-9275d6c6d055",
				"id":"bc94fe62-e909-4c0e-8627-0479c4017404",
				"realname":"飞翔s"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"176467ad-80ed-49ba-8a8e-5fbe2fbecb8b",
				"realname":"你弄"
			}
		}
	],
	"usermsg":"正常"
}
```


#工作效率排行
>暂无

| 接口名称 | *工作效率排行* |
| -- | -- |
| **接口地址** | */rankinglist/effic* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)    
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|user|用户|<code>object</code>|是|暂无|无|
|effic|工作效率|<code>digit</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```




#新增客户数排行
>暂无

| 接口名称 | *新增客户数排行* |
| -- | -- |
| **接口地址** | */rankinglist/newcusts* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)    
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|user|用户|<code>object</code>|是|暂无|无|
|newcusts|新增客户数|<code>digit</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /rankinglist/newcusts?tt=1&vn=1.0&access_token=OThlY2MwZTEtOWExMi00NzYxLTlhMTgtNzE0MDM2Y2M0ZGM1 HTTP/1.1
Host: localhost:8080
Cache-Control: no-cache
Postman-Token: 6d0ede61-31ae-29f2-3fa7-0f4c6c2b40af
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"newcusts":3,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1451289319978.jpg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"赵丽22"
			}
		},
		{
			"newcusts":1,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"46b61d83-6da1-4b4c-a064-14e6b9be8692",
				"realname":"asdfasd"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"4f093f84-4704-424a-a055-4be6d80332a5",
				"realname":"给你们"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"7d219460-56cd-4d60-a718-cb16c3396893",
				"realname":"飞翔"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"7d67eb45-d4b7-4ac0-84ea-3b3f979e5c28",
				"realname":"源源"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"80f639f8-e998-47fb-8781-7018c6952d54",
				"realname":"miser"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"87556163-f142-42a4-a5dc-50251c6af3ad",
				"realname":"t222"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"8c457eeb-6f28-42d0-a612-95582b34555f",
				"realname":"test8"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/b1976ff6-7b36-46a7-8d55-4288058b6224",
				"id":"8d3cd5a5-d744-49cf-a60b-cfb5374080c5",
				"realname":"林鸿非"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1c9f6fc7-d750-4c8a-bafb-939306a47d72",
				"id":"96f5f7f9-483a-4a43-88b3-d0ad1c629c53",
				"realname":"网名"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"acfc1ae2-6687-4b14-a147-c0907b283ec2",
				"realname":"龙少"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"0932ec38-057f-49b9-9550-545b52ba8277",
				"realname":"哈哈王"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"b736eefe-ea50-459c-89d5-95c48b5e2702",
				"realname":"123456"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"0b1665d6-ef7f-46ff-b771-dc69924ee50b",
				"realname":"Dghj"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"0cd455e1-fa64-4649-ba6b-e064f614bdf1",
				"realname":"成员"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/ba51279e-b5a8-4113-9d84-9275d6c6d055",
				"id":"bc94fe62-e909-4c0e-8627-0479c4017404",
				"realname":"飞翔s"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"109cf0c6-a717-4af9-bb5b-1d588d5f2049",
				"realname":"test5"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/3e566fcb-49a2-4ba4-9d7f-644e4d01d0c2",
				"id":"d47539b3-9820-4086-9582-f629d2ef0630",
				"realname":"王老大"
			}
		},
		{
			"newcusts":0,
			"user":{
				"header":"",
				"id":"176467ad-80ed-49ba-8a8e-5fbe2fbecb8b",
				"realname":"你弄"
			}
		}
	],
	"usermsg":"正常"
}

```





#M币排行
>暂无

| 接口名称 | *M币排行* |
| -- | -- |
| **接口地址** | */rankinglist/mcoin* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)    
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|user|用户|<code>object</code>|是|暂无|无|
|mcoin|M币|<code>digit</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /rankinglist/mcoin?tt=1&vn=1.0&access_token=OThlY2MwZTEtOWExMi00NzYxLTlhMTgtNzE0MDM2Y2M0ZGM1 HTTP/1.1
Host: localhost:8080
Cache-Control: no-cache
Postman-Token: 9f70662b-d457-237d-a821-4df191cf5663
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"mcoin":7398,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东"
			}
		},
		{
			"mcoin":3335,
			"user":{
				"header":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
				"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
				"realname":"李四"
			}
		},
		{
			"mcoin":1543,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/3e566fcb-49a2-4ba4-9d7f-644e4d01d0c2",
				"id":"d47539b3-9820-4086-9582-f629d2ef0630",
				"realname":"王老大"
			}
		},
		{
			"mcoin":1112,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1451289319978.jpg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"赵丽22"
			}
		},
		{
			"mcoin":222,
			"user":{
				"header":"",
				"id":"acfc1ae2-6687-4b14-a147-c0907b283ec2",
				"realname":"龙少"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"0932ec38-057f-49b9-9550-545b52ba8277",
				"realname":"哈哈王"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"0b1665d6-ef7f-46ff-b771-dc69924ee50b",
				"realname":"Dghj"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"0cd455e1-fa64-4649-ba6b-e064f614bdf1",
				"realname":"成员"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"109cf0c6-a717-4af9-bb5b-1d588d5f2049",
				"realname":"test5"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"176467ad-80ed-49ba-8a8e-5fbe2fbecb8b",
				"realname":"你弄"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"19d11f90-6747-4110-9f8c-ebee5645e1a7",
				"realname":"11订单"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"26aaceba-25f8-482e-86f3-c18a41cb0f30",
				"realname":"佛挡杀佛"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"46b61d83-6da1-4b4c-a064-14e6b9be8692",
				"realname":"asdfasd"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"4f093f84-4704-424a-a055-4be6d80332a5",
				"realname":"给你们"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"7d219460-56cd-4d60-a718-cb16c3396893",
				"realname":"飞翔"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"7d67eb45-d4b7-4ac0-84ea-3b3f979e5c28",
				"realname":"源源"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"80f639f8-e998-47fb-8781-7018c6952d54",
				"realname":"miser"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"87556163-f142-42a4-a5dc-50251c6af3ad",
				"realname":"t222"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"",
				"id":"8c457eeb-6f28-42d0-a612-95582b34555f",
				"realname":"test8"
			}
		},
		{
			"mcoin":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/b1976ff6-7b36-46a7-8d55-4288058b6224",
				"id":"8d3cd5a5-d744-49cf-a60b-cfb5374080c5",
				"realname":"林鸿非"
			}
		}
	],
	"usermsg":"正常"
}

```





#星值排行
>暂无

| 接口名称 | *星值排行* |
| -- | -- |
| **接口地址** | */rankinglist/starval* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)    
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|user|用户|<code>object</code>|是|暂无|无|
|starval|星值|<code>digit</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /rankinglist/starval?tt=1&vn=1.0&access_token=OThlY2MwZTEtOWExMi00NzYxLTlhMTgtNzE0MDM2Y2M0ZGM1 HTTP/1.1
Host: localhost:8080
Cache-Control: no-cache
Postman-Token: a4892e5e-cda8-5af1-3222-efa10af8c87d
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"starval":8453,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/dce172a4-62fc-42c9-9305-c1595d02eec3",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三东"
			}
		},
		{
			"starval":1196,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/3e566fcb-49a2-4ba4-9d7f-644e4d01d0c2",
				"id":"d47539b3-9820-4086-9582-f629d2ef0630",
				"realname":"王老大"
			}
		},
		{
			"starval":812,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/1451289319978.jpg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"赵丽22"
			}
		},
		{
			"starval":555,
			"user":{
				"header":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
				"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
				"realname":"李四"
			}
		},
		{
			"starval":444,
			"user":{
				"header":"",
				"id":"acfc1ae2-6687-4b14-a147-c0907b283ec2",
				"realname":"龙少"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"0932ec38-057f-49b9-9550-545b52ba8277",
				"realname":"哈哈王"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"0b1665d6-ef7f-46ff-b771-dc69924ee50b",
				"realname":"Dghj"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"0cd455e1-fa64-4649-ba6b-e064f614bdf1",
				"realname":"成员"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"109cf0c6-a717-4af9-bb5b-1d588d5f2049",
				"realname":"test5"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"176467ad-80ed-49ba-8a8e-5fbe2fbecb8b",
				"realname":"你弄"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"19d11f90-6747-4110-9f8c-ebee5645e1a7",
				"realname":"11订单"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"26aaceba-25f8-482e-86f3-c18a41cb0f30",
				"realname":"佛挡杀佛"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"46b61d83-6da1-4b4c-a064-14e6b9be8692",
				"realname":"asdfasd"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"4f093f84-4704-424a-a055-4be6d80332a5",
				"realname":"给你们"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"7d219460-56cd-4d60-a718-cb16c3396893",
				"realname":"飞翔"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"7d67eb45-d4b7-4ac0-84ea-3b3f979e5c28",
				"realname":"源源"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"80f639f8-e998-47fb-8781-7018c6952d54",
				"realname":"miser"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"87556163-f142-42a4-a5dc-50251c6af3ad",
				"realname":"t222"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"",
				"id":"8c457eeb-6f28-42d0-a612-95582b34555f",
				"realname":"test8"
			}
		},
		{
			"starval":0,
			"user":{
				"header":"http://112.74.131.85:80/oa/upload/images/b1976ff6-7b36-46a7-8d55-4288058b6224",
				"id":"8d3cd5a5-d744-49cf-a60b-cfb5374080c5",
				"realname":"林鸿非"
			}
		}
	],
	"usermsg":"正常"
}

```