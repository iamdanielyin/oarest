#任务列表
>按时间逆序排列

| 接口名称 | *任务列表* |
| -- | -- |
| **接口地址** | */tasks* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|是|0全部，1上级任务，2协同工作，3下属工作，4未汇报，5提醒|0|

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|任务数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|任务ID|<code>string</code>|是|暂无|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|startdate|计划开始日期|<code>string</code>|是|暂无|无|
|enddate|计划结束日期|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|暂无|无|
|status|任务状态|<code>digit</code>|是|0进行中，1已汇报，2已完成|无|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|operators|执行人|<code>array</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：operators

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|

##接口示例

```
GET /oa/tasks?access_token=YTRiYjVlMGEtNjQ3Yy00M2NjLWJjNTYtM2E3YTZhOGNmMzNl&flag=0&page=0&size=10 HTTP/1.1
Host: localhost:7778
Content-Type: application/json;charset=UTF-8
Accept: application/json;
Accept-Charset: utf-8
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "data": [
        {
            "createtime": "2015-09-29 17:51:32",
            "enddate": "2015-10-01 00:00:00",
            "operators": [
                {
                    "header": "http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
                    "id": "d47539b3-9820-4086-9582-f629d2ef0630",
                    "realname": "王五"
                },
                {
                    "header": "http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
                    "id": "5d772756-3b06-4b75-9de1-f9c07310ec06",
                    "realname": "张三"
                }
            ],
            "id": "d78ab909-7994-4fc0-8dc9-9200e749782c",
            "startdate": "2015-09-29 00:00:00",
            "title": "任务2",
            "user": {
                "header": "http://img5.duitang.com/uploads/item/201508/12/20150812204032_eiAQk.thumb.224_0.jpeg",
                "id": "51c58245-1921-44a2-8aed-60fc3b85cc3c",
                "realname": "赵丽"
            },
            "content": "任务2内容描述",
            "status": 0
        },
        {
            "createtime": "2015-09-29 17:51:32",
            "enddate": "2015-10-01 00:00:00",
            "operators": [
                {
                    "header": "http://img5.duitang.com/uploads/item/201504/21/20150421H4340_uv24P.thumb.224_0.jpeg",
                    "id": "5d772756-3b06-4b75-9de1-f9c07310ec06",
                    "realname": "张三"
                },
                {
                    "header": "http://img5.duitang.com/uploads/item/201503/26/20150326161657_aL8FW.jpeg",
                    "id": "d47539b3-9820-4086-9582-f629d2ef0630",
                    "realname": "王五"
                }
            ],
            "id": "243d6cd4-629b-4da8-98ac-ee1addbee2e6",
            "startdate": "2015-09-29 00:00:00",
            "title": "任务1",
            "user": {
                "header": "http://cdn.duitang.com/uploads/item/201504/21/20150421H4327_3eRXN.thumb.224_0.jpeg",
                "id": "d9a5648a-65dd-46ef-add8-4837795ce8b4",
                "realname": "李四"
            },
            "content": "任务1内容描述",
            "status": 0
        }
    ],
    "usermsg": "正常"
}

```






***

#任务详细
>接口描述


| 接口名称 | *任务详细* |
| -- | -- |
| **接口地址** | */tasks/{id}* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|status|任务状态|<code>string</code>|是|0未审，1通过，2不通过|无|
|startdate|计划开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|计划结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|reportdate|汇报时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|finishdate|完成时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|mcoin|任务M币|<code>digit</code>|是|暂无|无|
|starval|任务星值|<code>digit</code>|是|暂无|无|
|isdailytask|是否日常任务|<code>boolean</code>|是|暂无|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|
|operators|执行人|<code>array</code>|是|暂无|无|
|attachs|任务附件|<code>array</code>|是|暂无|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：operators

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|

参数项：attachs

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|file|文件链接|<code>string</code>|是|暂无|无|


##接口示例

```
暂无

```

***




#新增任务
>接口描述


| 接口名称 | *新增任务* |
| -- | -- |
| **接口地址** | */tasks* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|startdate|计划开始日期|<code>string</code>|是|暂无|无|
|enddate|计划结束日期|<code>string</code>|是|暂无|无|
|mcoin|任务M币|<code>digit</code>|否|暂无|0|
|starval|任务星值|<code>digit</code>|否|暂无|0|
|operators|执行人|<code>string</code>|是|用户ID，多个用英文逗号分隔|无|
|attachs|任务附件|<code>string</code>|否|文件链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)


##接口示例

```
暂无

```

***







#删除任务
>接口描述

| 接口名称 | *删除任务* |
| -- | -- |
| **接口地址** | */tasks/{id}* |
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






#新增协同
>调用该接口后，执行人会被正式添加到任务执行人中。该接口应该在用户收到协同消息并同意协同后调用

| 接口名称 | *新增协同* |
| -- | -- |
| **接口地址** | */tasks/{id}/operators* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|operator|执行人ID|<code>string</code>|是|用户ID|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无

```

***






#任务提醒
>接口描述

| 接口名称 | *任务提醒* |
| -- | -- |
| **接口地址** | */tasks/{id}/reminder* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|isremind|是否提醒|<code>boolean</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无

```

***






#任务汇报
>接口描述

| 接口名称 | *任务汇报* |
| -- | -- |
| **接口地址** | */tasks/{id}/reports* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|content|汇报内容|<code>string</code>|是|暂无|无|
|images|汇报图片|<code>string</code>||图片链接，多个用英文逗号分隔|无|
|attachs|汇报附件|<code>string</code>|否|文件链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无

```

***






#任务审批
>接口描述

| 接口名称 | *任务审批* |
| -- | -- |
| **接口地址** | */tasks/{id}/approvals* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|isfinish|是否通过|<code>boolean</code>|是|为true时operators不能为空；为false时任务会被重置回完成中状态|无|
|operators|执行人|<code>string</code>|否|用户ID:M币:星值，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无

```

***
