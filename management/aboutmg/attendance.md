#指定日期查询考勤记录
>按时间逆序排列

| 接口名称 | *指定日期查询考勤记录* |
| -- | -- |
| **接口地址** | */attendance/days* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|day|日期|<code>string</code>|是|yyyy-MM-dd|今日|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|signintime|签到时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signingps|签到gps|<code>string</code>|是|格式为"经度,纬度"，英文逗号分隔|无|
|signouttime|签退时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signoutgps|签退gps|<code>string</code>|是|yyyy格式为"经度,纬度"，英文逗号分隔|无|

##接口示例

```
暂无
```


#查询月记录
>按时间逆序排列

| 接口名称 | *查询月记录* |
| -- | -- |
| **接口地址** | */attendance/months* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|month|年月|<code>string</code>|否|yyyy-MM|当前月|


##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|signintime|今日签到时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signingps|今日签到gps|<code>string</code>|是|格式为"经度,纬度"，英文逗号分隔|无|
|signouttime|今日签退时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signoutgps|今日签退gps|<code>string</code>|是|yyyy格式为"经度,纬度"，英文逗号分隔|无|
|actwork|考勤次数|<code>digit</code>|是|暂无|无|
|overtime|加班（小时；次数）|<code>string</code>|是|暂无|无|
|lates|迟到（分钟；次数）|<code>string</code>|是|暂无|无|
|leavearly|早退（分钟；次数）|<code>string</code>|是|暂无|无|
|askleave|请假（小时；次数）|<code>string</code>|是|暂无|无|
|onbus|外出考勤次数|<code>string</code>|是|暂无|无|
|overtime|加班（小时；次数）|<code>string</code>|是|暂无|无|
|overtime|加班（小时；次数）|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```



#权限分配
>需【权限管理】权限

| 接口名称 | *权限分配* |
| -- | -- |
| **接口地址** | */permis/users* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|userid|用户ID|<code>string</code>|是|暂无|无|
|permis|权限|<code>string</code>|是|权限ID，多个由英文逗号分隔|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```




