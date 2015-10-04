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
|sex|性别|<code>string</code>|是|暂无|无|
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
GET /oa/users?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh&page=0&size=20 HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache 
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "data": [
        {
            "createtime": "2015-10-01 17:42:44",
            "id": "25b4c3f3-b8b6-4f3f-afb0-35caca43d252",
            "title": "用户2",
            "content": "用户内容2用户内容2用户内容2"
        },
        {
            "createtime": "2015-10-01 17:42:44",
            "id": "93d24bcd-5f6b-45e0-b691-208594b95d12",
            "title": "用户1",
            "content": "用户内容1用户内容1用户内容1用户内容1"
        }
    ],
    "usermsg": "正常"
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
GET /oa/users/93d24bcd-5f6b-45e0-b691-208594b95d12?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "data": {
        "creator": {
            "header": "http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
            "id": "d47539b3-9820-4086-9582-f629d2ef0630",
            "realname": "王五"
        },
        "createtime": "2015-10-01 17:42:44",
        "modifytime": "2015-10-01 17:43:10",
        "remark": "",
        "id": "93d24bcd-5f6b-45e0-b691-208594b95d12",
        "title": "用户1",
        "content": "用户内容1用户内容1用户内容1用户内容1"
    },
    "usermsg": "正常"
}
```





#新增用户
>需具备【用户管理】权限


| 接口名称 | *新增用户* |
| -- | -- |
| **接口地址** | */users* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|标题|<code>string</code>|是|标题在系统内唯一不能重复|无|
|content|内容|<code>string</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)


##接口示例

```
POST /oa/users?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

title=用户标题&content=用户内容
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "data": {
        "creator": {
            "header": "http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
            "id": "d47539b3-9820-4086-9582-f629d2ef0630",
            "realname": "王五"
        },
        "createtime": "2015-10-01 17:42:44",
        "modifytime": "2015-10-01 17:43:10",
        "remark": "",
        "id": "93d24bcd-5f6b-45e0-b691-208594b95d12",
        "title": "用户1",
        "content": "用户内容1用户内容1用户内容1用户内容1"
    },
    "usermsg": "正常"
}
```

***







#删除用户
>需具备【用户管理】权限

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
DELETE /oa/users/ebba0834-e5b6-4fec-b01f-1a9d4e2b3f7f?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}
```

***
