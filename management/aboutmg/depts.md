#部门列表
>按时间逆序排列

| 接口名称 | *部门列表* |
| -- | -- |
| **接口地址** | */depts* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|部门数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|name|名称|<code>string</code>|是|暂无|无|
|user|负责人|<code>object</code>|是|暂无|无|
|mems|成员数组|<code>array</code>|是|暂无|web|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：mems

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|profession|职位|<code>string</code>|是|暂无|无|
|mobile|手机号码1|<code>string</code>|否|暂无|无|

##接口示例

```
GET /oa/depts?access_token=YzZhNjc0MTEtZWQxZC00ZWM5LTkyZTYtODgyY2ZkMzhlMTk2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"data":[
		{
			"name":"总裁办",
			"id":"7d067826-3126-487e-b6ce-a1e526ba807f",
			"user":{
				"header":"http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
				"id":"d47539b3-9820-4086-9582-f629d2ef0630",
				"realname":"王五"
			}
		},
		{
			"name":"财务部",
			"id":"fcc38255-ab01-4b74-999f-3cddf61c7503",
			"user":{
				"header":"http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
				"id":"d9a5648a-65dd-46ef-add8-4837795ce8b4",
				"realname":"李四"
			}
		},
		{
			"name":"市场部",
			"id":"8da0fc5f-6542-4166-bf3f-f28310487bd6",
			"user":{
				"header":"http://img5.duitang.com/uploads/item/201508/12/20150812204032_eiAQk.thumb.224_0.jpeg",
				"id":"51c58245-1921-44a2-8aed-60fc3b85cc3c",
				"realname":"赵丽"
			}
		},
		{
			"name":"生产部",
			"id":"f27780e5-7541-4b68-b731-9e56f61e71b5",
			"user":{
				"header":"http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
				"id":"5d772756-3b06-4b75-9de1-f9c07310ec06",
				"realname":"张三"
			}
		}
	],
	"deptmsg":"正常"
}
```


#部门检索
>查询部门下成员信息，按时间逆序排列

| 接口名称 | *部门检索* |
| -- | -- |
| **接口地址** | */depts/{id}/users* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|否|0全部，1成员关键字检索|0|
|keyword|关键字|<code>string</code>|否|当flag为1时需指定该项，模糊匹配用户姓名或用户名|无|

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|成员数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|profession|职位|<code>string</code>|是|暂无|无|
|mobile|手机号码1|<code>string</code>|否|暂无|无|

##接口示例

```
GET /oa/depts/7d067826-3126-487e-b6ce-a1e526ba807f/users?access_token=YzZhNjc0MTEtZWQxZC00ZWM5LTkyZTYtODgyY2ZkMzhlMTk2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "data": [
        {
            "header": "http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
            "id": "d47539b3-9820-4086-9582-f629d2ef0630",
            "realname": "王五"
        }
    ],
    "deptmsg": "正常"
}
```



#部门详情
>暂无

| 接口名称 | *部门详情* |
| -- | -- |
| **接口地址** | */depts/{id}* |
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
|name|名称|<code>string</code>|是|暂无|无|
|user|负责人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/depts/7d067826-3126-487e-b6ce-a1e526ba807f?access_token=YzZhNjc0MTEtZWQxZC00ZWM5LTkyZTYtODgyY2ZkMzhlMTk2 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "data": {
        "createtime": "2015-09-29 18:25:00",
        "modifytime": "",
        "name": "总裁办",
        "remark": "",
        "id": "7d067826-3126-487e-b6ce-a1e526ba807f",
        "user": {
            "header": "http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
            "id": "d47539b3-9820-4086-9582-f629d2ef0630",
            "realname": "王五"
        }
    },
    "usermsg": "正常"
}
```





#新增部门
>需具备【组织架构】权限


| 接口名称 | *新增部门* |
| -- | -- |
| **接口地址** | */depts* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|name|名称|<code>string</code>|是|暂无|无|
|user|负责人ID|<code>string</code>|否|暂无|无|

##返回参数
[<公共返回参数>](../README.md)


##接口示例

```
POST /oa/depts?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

user=d47539b3-9820-4086-9582-f629d2ef0630&name=测试接口新增部门
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"usermsg":"正常"
}

```

***







#修改部门
>需具备【组织架构】权限，只需提供需要修改的资料项即可

| 接口名称 | *修改部门* |
| -- | -- |
| **接口地址** | */depts/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|name|名称|<code>string</code>|否|暂无|无|
|user|负责人ID|<code>string</code>|否|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
PATCH /oa/depts/3a0ddcd9-2112-4ef2-8364-9b70c96c0fe5?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz&name=测试接口修改部门 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"usermsg":"正常"
}
```

***





#添加成员
>需具备【组织架构】权限，只需提供需要修改的资料项即可

| 接口名称 | *添加成员* |
| -- | -- |
| **接口地址** | */depts/{id}/users* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|users|用户ID|<code>string</code>|是|用户ID，多个英文逗号分隔|无|
|users|用户ID|<code>string</code>|是|用户ID，多个英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/depts/3a0ddcd9-2112-4ef2-8364-9b70c96c0fe5/users?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

users=87556163-f142-42a4-a5dc-50251c6af3ad%2Cacfc1ae2-6687-4b14-a147-c0907b283ec2
———————————————————————————————————————————————————————————
{
	"statuscode":"0000",
	"statusmsg":"ok",
	"usermsg":"正常"
}
```

***








#删除部门
>需具备【组织架构】权限且要删除的部门

| 接口名称 | *删除部门* |
| -- | -- |
| **接口地址** | */depts/{id}* |
| **请求方式** | <mark>DELETE</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
DELETE /oa/depts/309c51e0-387c-4c40-8acd-3bbd37fa214a?access_token=MmViNThiNWUtZDliZS00MTdjLWE2YzAtY2M2MTgyYjgwMmMz HTTP/1.1
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
