#登录
>接口描述


| 接口名称 | *登录* |
| -- | -- |
| **接口地址** | */users/login* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|username|用户名|<code>string</code>|是|暂无|无|
|password|密码|<code>string</code>|是|暂无|无|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|access_token|访问令牌|<code>string</code>|是|暂无|无|
|id|用户ID|<code>string</code>|是|暂无|无|
|username|用户名|<code>string</code>|是|暂无|无|
|isboss|是否老板|<code>boolean</code>|是|暂无|无|
|headportrait|头像链接|<code>string</code>|否|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|
|sex|性别|<code>digit</code>|否|0男,1女|无|
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
|remark|备注|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|


参数项：superior、dept.user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
GET /oa/users/login?username=test1&password=123456 HTTP/1.1
Host: localhost:7778
Content-Type: application/json;charset=UTF-8
Accept: application/json;
Accept-Charset: utf-8
Cache-Control: no-cache
——————————————————————————————————————————————————————————————————————————————————————————
{
    "statuscode": "0000",
    "access_token": "ZDM4OWNlNWYtNzhkMy00OTk1LWIwMDctYjRhNWVhNzUyMDcy",
    "statusmsg": "ok",
    "data": {
        "profession": "",
        "qq": "",
        "createtime": "2015-09-29 11:39:54",
        "mail": "",
        "modifytime": "",
        "sex": 0,
        "mobile1": "",
        "totalmcoin": 0,
        "remark": "",
        "dept": {},
        "totalstarval": 0,
        "realname": "",
        "curstarval": 0,
        "password": "123456",
        "superior": "",
        "weixin": "",
        "mobile3": "",
        "headportrait": "",
        "mobile2": "",
        "isboss": false,
        "curmcoin": 0,
        "id": "5d772756-3b06-4b75-9de1-f9c07310ec06",
        "user": {},
        "username": "test1"
    }
}

```




