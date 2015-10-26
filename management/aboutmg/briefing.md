#我
>暂无

| 接口名称 | *我* |
| -- | -- |
| **接口地址** | */briefing/me* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|synergy|协同|<code>object</code>|是|暂无|无|
|attendance|考勤|<code>object</code>|是|暂无|无|
|others|其他|<code>object</code>|是|暂无|无|

参数项：synergy

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|logsno|日志数|<code>digit</code>|是|暂无|无|
|currmcoin|M币|<code>digit</code>|是|暂无|无|
|totalmcoin|历史M币|<code>digit</code>|是|暂无|无|
|curstarval|星值|<code>digit</code>|是|暂无|无|
|totalstarval|历史星值|<code>digit</code>|是|暂无|无|
|logindays|登录天数|<code>digit</code>|是|暂无|无|

参数项：attendance

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|ontime|准时率|<code>string</code>|是|百分比，如30%|无|
|attend|出勤率|<code>string</code>|是|百分比，如30%|无|

参数项：others

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|monworkload|当月工作量|<code>string</code>|是|暂无|无|
|effic|工作效率|<code>string</code>|是|百分比，如30%|无|
|newcusts|新增客户量|<code>digit</code>|是|暂无|无|

##接口示例

```
暂无
```


#公司
>暂无

| 接口名称 | *项目详情* |
| -- | -- |
| **接口地址** | */records* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|userid|员工ID|<code>string</code>|是|暂无|无|
|mcoin|M币|<code>digit</code>|否|暂无|无|
|starval|星值|<code>digit</code>|否|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```


#荣誉墙
>暂无

| 接口名称 | *项目详情* |
| -- | -- |
| **接口地址** | */records* |
| **请求方式** | <mark>POST</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|userid|员工ID|<code>string</code>|是|暂无|无|
|mcoin|M币|<code>digit</code>|否|暂无|无|
|starval|星值|<code>digit</code>|否|暂无|无|

##返回参数
[<公共返回参数>](../README.md)

##接口示例

```
暂无
```


