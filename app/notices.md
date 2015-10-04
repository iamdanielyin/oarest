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
GET /oa/notices?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh&page=0&size=20 HTTP/1.1
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
            "title": "公告2",
            "content": "公告内容2公告内容2公告内容2"
        },
        {
            "createtime": "2015-10-01 17:42:44",
            "id": "93d24bcd-5f6b-45e0-b691-208594b95d12",
            "title": "公告1",
            "content": "公告内容1公告内容1公告内容1公告内容1"
        }
    ],
    "usermsg": "正常"
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


参数项：data

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
GET /oa/notices/93d24bcd-5f6b-45e0-b691-208594b95d12?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
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
        "title": "公告1",
        "content": "公告内容1公告内容1公告内容1公告内容1"
    },
    "usermsg": "正常"
}
```





#新增公告
>需具备【公告管理】权限


| 接口名称 | *新增公告* |
| -- | -- |
| **接口地址** | */notices* |
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
POST /oa/notices?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

title=公告标题&content=公告内容
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
        "title": "公告1",
        "content": "公告内容1公告内容1公告内容1公告内容1"
    },
    "usermsg": "正常"
}
```

***







#删除公告
>需具备【公告管理】权限

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
DELETE /oa/notices/ebba0834-e5b6-4fec-b01f-1a9d4e2b3f7f?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
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
