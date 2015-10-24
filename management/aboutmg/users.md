#用户列表
>按时间逆序排列

| 接口名称 | *用户列表* |
| -- | -- |
| **接口地址** | */users* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|用户数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|username|用户名|<code>string</code>|是|暂无|无|
|isboss|是否老板|<code>boolean</code>|是|暂无|无|
|headportrait|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|sex|性别|<code>digit</code>|是|0男，1女|无|
|dept|部门|<code>object</code>|是|暂无|无|
|profession|职位|<code>string</code>|是|暂无|无|
|mobile|手机号码|<code>string</code>|是|暂无|无|

参数项：dept

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|name|名称|<code>string</code>|是|暂无|无|
|user|姓名|<code>object</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例
```
GET /oa/users?access_token=YzZhNjc0MTEtZWQxZC00ZWM5LTkyZTYtODgyY2ZkMzhlMTk2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"profession":"老板",
			"headportrait":"http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
			"sex":0,
			"isboss":true,
			"mobile":"",
			"id":"d47539b3-9820-4086-9582-f629d2ef0630",
			"dept":{
				"name":"总裁办",
				"id":"7d067826-3126-487e-b6ce-a1e526ba807f",
				"user":{
					"header":"http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
					"id":"d47539b3-9820-4086-9582-f629d2ef0630",
					"realname":"王五"
				}
			},
			"username":"test4",
			"realname":"王五"
		},
		{
			"profession":"部门职员",
			"headportrait":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
			"sex":0,
			"isboss":false,
			"mobile":"",
			"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
			"dept":{
				"name":"生产部",
				"id":"f27780e5-7541-4b68-b731-9e56f61e71b5",
				"user":{
					"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
					"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
					"realname":"张三"
				}
			},
			"username":"test3",
			"realname":"李四"
		},
		{
			"profession":"部门职员",
			"headportrait":"http://img5.duitang.com/uploads/item/201508/12/20150812204032_eiAQk.thumb.224_0.jpeg",
			"sex":1,
			"isboss":false,
			"mobile":"",
			"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
			"dept":{
				"name":"财务部",
				"id":"fcc38255-ab01-4b74-999f-3cddf61c7503",
				"user":{
					"header":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
					"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
					"realname":"李四"
				}
			},
			"username":"test2",
			"realname":"赵丽"
		},
		{
			"profession":"部门职员",
			"headportrait":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
			"sex":0,
			"isboss":false,
			"mobile":"13456789012",
			"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
			"dept":{
				"name":"市场部",
				"id":"8da0fc5f-6542-4166-bf3f-f28310487bd6",
				"user":{
					"header":"http://img5.duitang.com/uploads/item/201508/12/20150812204032_eiAQk.thumb.224_0.jpeg",
					"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
					"realname":"赵丽"
				}
			},
			"username":"test1",
			"realname":"张三"
		}
	],
	"usermsg":"正常"
}

```




#用户详情
>暂无

| 接口名称 | *用户详情* |
| -- | -- |
| **接口地址** | */users/{id}* |
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
|username|用户名|<code>string</code>|是|暂无|无|
|isboss|是否老板|<code>boolean</code>|是|暂无|无|
|headportrait|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|sex|性别|<code>digit</code>|是|0男，1女|无|
|dept|部门|<code>object</code>|是|暂无|无|
|profession|职位|<code>string</code>|是|暂无|无|
|superior|上级领导|<code>object</code>|是|暂无|无|
|mobile1|手机号码1|<code>string</code>|否|暂无|无|
|mobile2|手机号码2|<code>string</code>|否|暂无|无|
|mobile3|手机号码3|<code>string</code>|否|暂无|无|
|qq|QQ|<code>string</code>|否|暂无|无|
|weixin|微信|<code>string</code>|否|暂无|无|
|mail|邮箱|<code>string</code>|否|暂无|无|
|curmcoin|当前M币|<code>digit</code>|是|暂无|无|
|curstarval|当前星值|<code>digit</code>|是|暂无|无|
|totalmcoin|累计M币|<code>digit</code>|是|暂无|无|
|totalstarval|累计星值|<code>digit</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|

参数项：dept

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|name|名称|<code>string</code>|是|暂无|无|
|user|负责人|<code>object</code>|是|暂无|无|

参数项：superior、dept.user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/users/d9a5648a-65dd-46ef-add8-4837795ce8b4?access_token=YzZhNjc0MTEtZWQxZC00ZWM5LTkyZTYtODgyY2ZkMzhlMTk2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":{
		"profession":"部门职员",
		"qq":"",
		"createtime":"2015-09-29 13:40:18",
		"mail":"",
		"modifytime":"2015-10-01 19:55:02",
		"sex":0,
		"mobile1":"",
		"totalmcoin":20,
		"remark":"",
		"dept":{
			"name":"生产部",
			"id":"f27780e5-7541-4b68-b731-9e56f61e71b5",
			"user":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三"
			}
		},
		"totalstarval":239,
		"realname":"李四",
		"curstarval":23,
		"superior":{
			"header":"http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
			"id":"d47539b3-9820-4086-9582-f629d2ef0630",
			"realname":"王五"
		},
		"weixin":"",
		"mobile3":"",
		"headportrait":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
		"mobile2":"",
		"isboss":false,
		"curmcoin":2,
		"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
		"username":"test3"
	},
	"usermsg":"正常"
}
```





#新增用户
>需具备【组织架构】权限


| 接口名称 | *新增用户* |
| -- | -- |
| **接口地址** | */users* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|username|用户名|<code>string</code>|是|唯一|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|dept|部门ID|<code>string</code>|是|暂无|无|
|profession|职位|<code>string</code>|是|暂无|无|
|superior|上级领导ID|<code>string</code>|是|暂无|无|
|password|密码|<code>string</code>|否|暂无|123456|
|isboss|是否老板|<code>boolean</code>|否|暂无|false|
|headportrait|头像链接|<code>string</code>|否|暂无|无|
|sex|性别|<code>digit</code>|否|0男，1女|无|
|mobile1|手机号码1|<code>string</code>|否|唯一|无|
|mobile2|手机号码2|<code>string</code>|否|唯一|无|
|mobile3|手机号码3|<code>string</code>|否|唯一|无|
|qq|QQ|<code>string</code>|否|唯一|无|
|weixin|微信|<code>string</code>|否|唯一|无|
|mail|邮箱|<code>string</code>|否|唯一|无|
|curmcoin|当前M币|<code>digit</code>|否|暂无|0|
|curstarval|当前星值|<code>digit</code>|否|暂无|0|
|totalmcoin|累计M币|<code>digit</code>|否|暂无|0|
|totalstarval|累计星值|<code>digit</code>|否|暂无|0|

##返回参数
[<公共返回参数>](../README.md)


##接口示例

```
———————————————————————————————————————————————————————————
```

***







#修改用户
>需具备【用户管理】权限，只需提供需要修改的资料项即可

| 接口名称 | *修改用户* |
| -- | -- |
| **接口地址** | */users/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|username|用户名|<code>string</code>|否|唯一|无|
|realname|姓名|<code>string</code>|否|暂无|无|
|dept|部门ID|<code>string</code>|否|暂无|无|
|profession|职位|<code>string</code>|否|暂无|无|
|superior|上级领导ID|<code>string</code>|否|暂无|无|
|isboss|是否老板|<code>boolean</code>|否|暂无|false|
|headportrait|头像链接|<code>string</code>|否|暂无|无|
|sex|性别|<code>digit</code>|否|0男，1女|无|
|mobile1|手机号码1|<code>string</code>|否|唯一|无|
|mobile2|手机号码2|<code>string</code>|否|唯一|无|
|mobile3|手机号码3|<code>string</code>|否|唯一|无|
|qq|QQ|<code>string</code>|否|唯一|无|
|weixin|微信|<code>string</code>|否|唯一|无|
|mail|邮箱|<code>string</code>|否|唯一|无|
|curmcoin|当前M币|<code>digit</code>|否|暂无|0|
|curstarval|当前星值|<code>digit</code>|否|暂无|0|
|totalmcoin|累计M币|<code>digit</code>|否|暂无|0|
|totalstarval|累计星值|<code>digit</code>|否|暂无|0|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
PATCH /oa/users/d47539b3-9820-4086-9582-f629d2ef0630?access_token=OTgxMGVlMzctYjdkNC00MDcwLTlhMjUtNzE4MTM5MjllMmU5&realname=王五2 HTTP/1.1
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




#删除用户
>需具备【用户管理】权限且要删除的用户

| 接口名称 | *删除用户* |
| -- | -- |
| **接口地址** | */users/{id}* |
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
