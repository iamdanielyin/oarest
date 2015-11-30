#签到签退
>暂无

| 接口名称 | *签到签退* |
| -- | -- |
| **接口地址** | */attendance* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|clockintype|打卡类型|<code>digit</code>|是|0签到，1签退|无|
|attentype|考勤类型|<code>digit</code>|是|0普通考勤，1外出考勤|无|
|gps|gps|<code>string</code>|是|格式为"经度,纬度"，英文逗号分隔|无|
|address|详细地址|<code>string</code>|是|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```

#指定日期查询考勤记录
>暂无

| 接口名称 | *指定日期查询考勤记录* |
| -- | -- |
| **接口地址** | */attendance/days* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|day|日期|<code>string</code>|否|yyyy-MM-dd|今日|


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
|data|本月数据|<code>array</code>|是|暂无|已按日期从小到大排列|

参数项：data


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|signintime|签到时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signingps|签到gps|<code>string</code>|是|格式为"经度,纬度"，英文逗号分隔|无|
|signouttime|签退时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signoutgps|签退gps|<code>string</code>|是|格式为"经度,纬度"，英文逗号分隔|无|

##接口示例

```
暂无
```




#考勤统计
>暂无

| 接口名称 | *考勤统计* |
| -- | -- |
| **接口地址** | */attendance* |
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
|data|本月数据|<code>object</code>|是|暂无|无|

参数项：data


|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|actwork|实际工作(打卡次数)|<code>digit</code>|是|暂无|无|
|overdays|加班天数|<code>digit</code>|是|暂无|无|
|overdays|加班天数|<code>digit</code>|是|暂无|无|
|signouttime|签退时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|signoutgps|签退gps|<code>string</code>|是|格式为"经度,纬度"，英文逗号分隔|无|

##接口示例

```
暂无
```




