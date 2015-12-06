#消息列表
>统一消息动作：跳转到相关详情页

| 接口名称 | *消息列表* |
| -- | -- |
| **接口地址** | */messages* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)


##返回参数
[<公共返回参数>](../README.md)


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|消息数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|消息ID|<code>string</code>|是|暂无|无|
|title|消息标题|<code>string</code>|是|暂无|无|
|content|消息内容|<code>string</code>|否|暂无|无|
|type|消息类型|<code>digit</code>|是|0协同通知，1任务指派通知，2审批提醒通知，3审批结果通知，4新公告通知|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|recever|接收者ID|<code>string</code>|是|暂无|无|
|status|消息状态|<code>digit</code>|是|0已读，1未读，有回调的消息，以回调结果为准|无|
|custdata|额外数据信息|<code>object</code>|是|每种消息可不同|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|

参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：custdata

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|数据ID|<code>string</code>|是|相关数据的ID信息，如任务指派，则该项为任务ID，新公告通知，该项为公告ID|无|
|type|审批类型|<code>digit</code>|是|当消息类型为2或3时，该项有值：0请假审批、1报销审批、2加班审批、3其他审批、4财务审批、5日志审批、6任务审批、7项目审批、8合同审批|无|

##接口示例

```
暂无

```




#请求协同
>暂无


| 接口名称 | *请求协同* |
| -- | -- |
| **接口地址** | */tasks/{id}/request* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)
|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|status|合同状态|<code>digit</code>|是|0执行中，1执行结束，2意外终止|无|


##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/tasks/d78ab909-7994-4fc0-8dc9-9200e749782c/operators?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
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



#确认协同
>调用该接口后，执行人会被正式添加到任务执行人中。该接口应该在用户收到协同消息并同意协同后调用，所以当前登录用户即为协同人。   
如果选择的协同人是同部门下的，那么会推送一条消息给协同人，然后协同人收到消息并确认同意协同后，会调用该接口，然后他就会被添加到任务的执行人中；如果要找不同部门的人参与任务协同，那么首先也会推送消息，只不过是推送给那个协同人的上级，上级如果同意了，那么协同人会被加入到任务执行人中


| 接口名称 | *确认协同* |
| -- | -- |
| **接口地址** | */tasks/{id}/operators* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
POST /oa/tasks/d78ab909-7994-4fc0-8dc9-9200e749782c/operators?tt=1&vn=1.0&access_token=OWMxNzIxMGQtN2ZiMC00N2RjLWEzNjgtZjU1YjFkMWUxMTRh HTTP/1.1
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