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
暂无
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
|user|姓名|<code>object</code>|是|暂无|无|

参数项：superior、dept.user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
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
暂无
```

***







#修改用户
>需具备【用户管理】权限

| 接口名称 | *删除用户* |
| -- | -- |
| **接口地址** | */users/{id}* |
| **请求方式** | <mark>PATCH</mark> |
| **数据格式** | <code>JSON</code> |

##请求参数
[<公共传入参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|username|用户名|<code>string</code>||唯一|无|
|realname|姓名|<code>string</code>|否|暂无|无|
|dept|部门ID|<code>string</code>|否|暂无|无|
|profession|职位|<code>string</code>|否|暂无|无|
|superior|上级领导ID|<code>string</code>|否|暂无|无|
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
暂无
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
暂无
```

***
