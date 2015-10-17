#员工加分
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

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|数据详细|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|name|项目名称|<code>string</code>|是|暂无|无|
|idesc|项目描述|<code>string</code>|是|暂无|无|
|startdate|开始日期|<code>string</code>|是|yyyy-MM-dd|无|
|enddate|结束日期|<code>string</code>|是|yyyy-MM-dd|无|
|sum|项目金额|<code>number</code>|是|暂无|无|
|mcoin|项目M币|<code>digit</code>|是|暂无|无|
|starval|项目星值|<code>digit</code>|是|暂无|无|
|creator|创建人|<code>object</code>|是|暂无|无|
|task|关联任务|<code>object</code>|否|暂无|无|
|remark|备注|<code>string</code>|否|暂无|无|
|createtime|创建时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
|modifytime|最近修改时间|<code>string</code>|否|yyyy-MM-dd HH:mm:ss|无|


参数项：creator

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|header|头像链接|<code>string</code>|是|暂无|无|
|realname|姓名|<code>string</code>|是|暂无|无|

参数项：task

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|id|ID|<code>string</code>|是|暂无|无|
|title|任务标题|<code>string</code>|是|暂无|无|

##接口示例

```
暂无
```


