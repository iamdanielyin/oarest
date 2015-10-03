#审批列表
>先按审批状态排序，未审的在前面；再按创建时间逆序排列；每个用户只能查询到和自己相关的审批

| 接口名称 | *审批列表* |
| -- | -- |
| **接口地址** | */approvals/leaves* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|flag|查询标识|<code>digit</code>|是|0我的申请，1我的审批|无|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|审批数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|stime|开始时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|etime|结束时间|<code>string</code>|是|yyyy-MM-dd HH:mm|无|
|reason|请假理由|<code>string</code>|是|暂无|无|
|leavetype|请假类型|<code>digit</code>|是|0病假，1事假，2其他|无|
|approver|审批人|<code>object</code>|是|暂无|无|
|status|审批状态|<code>digit</code>|是|0未审，1通过，2不通过|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|


参数项：approver、creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```







#新增审批
>接口描述


| 接口名称 | *新增审批* |
| -- | -- |
| **接口地址** | */leave* |
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
|type|审批类型|<code>digit</code>|是|0日报，1周报，2月报|无|
|customers|关联客户|<code>string</code>|否|客户ID，多个用英文逗号分隔|无|
|tasks|关联任务|<code>string</code>|否|任务ID，多个用英文逗号分隔|无|
|images|审批图片|<code>string</code>|否|图片链接，多个用英文逗号分隔|无|
|files|审批附件|<code>string</code>|否|文件链接，多个用英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/leave?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
Content-Type: application/x-www-form-urlencoded

title=审批接口5&content=审批接口内容&approver=d9a5648a-65dd-46ef-add8-4837795ce8b4&startdate=2015-10-01&enddate=2015-10-01&mcoin=1&starval=2&type=0&customers=2282a40e-c7eb-4b34-81a6-aa2efa1e6ad1%2C9005997f-8468-4f96-8e6a-06907dfb2038&tasks=243d6cd4-629b-4da8-98ac-ee1addbee2e6%2Cd78ab909-7994-4fc0-8dc9-9200e749782c&images=http%3A%2F%2Fp3.gexing.com%2Fshaitu%2F20120922%2F1519%2F505d6699e4347.jpg%2Chttp%3A%2F%2Fhiphotos.baidu.com%2F1985129%2Fpic%2Fitem%2Fd05c8ed3cc27b16e970a16b1.jpg&files=http%3A%2F%2Fimgsrc.baidu.com%2Fforum%2Fw%253D580%2Fsign%3Da574eb9cb07eca80120539efa1229712%2F16ff201f95cad1c8b0e3b1987f3e6709c83d5161.jpg

———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}
```

***







#删除审批
>接口描述

| 接口名称 | *删除审批* |
| -- | -- |
| **接口地址** | */leave/{id}* |
| **请求方式** | <mark>DELETE</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
DELETE /oa/leave/235e711c-5a04-40d8-b07f-b4ac2d0f8e64?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
Host: localhost:7778
Cache-Control: no-cache
———————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "statusmsg": "ok",
    "usermsg": "正常"
}


```





#审批审批
>只有审批指定审批人且该用户拥有审批权限才能审批审批

| 接口名称 | *审批审批* |
| -- | -- |
| **接口地址** | */leave/{id}/approvals* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|isfinish|是否通过|<code>boolean</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/leave/d7374cfa-4b43-4264-ac8a-4dd6e86af020/approvals?tt=1&vn=1.0&access_token=NTNkNjE4NGMtM2NjMy00YWRkLTkzMzctNWI3ZTVhZTNlNDZj HTTP/1.1
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
