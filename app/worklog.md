#日志列表
>按时间逆序排列

| 接口名称 | *日志列表* |
| -- | -- |
| **接口地址** | */worklogs* |
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
|data|合同数组|<code>array</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|任务ID|<code>string</code>|是|暂无|无|
|user|发表人|<code>object</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|暂无|无|
|enddate|结束日期|<code>string</code>|是|暂无|无|
|createtime|创建时间|<code>string</code>|是|暂无|无|
|status|任务状态|<code>string</code>|是|暂无|无|
|title|任务标题|<code>string</code>|是|暂无|无|
|content|任务内容|<code>string</code>|是|暂无|无|
|operators|协同人|<code>array</code>|是|暂无|无|

参数项：user

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：operators

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像|<code>string</code>|是|暂无|无|


##接口示例

```
暂无

```




