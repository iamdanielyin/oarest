#M币记录
>暂无

| 接口名称 | *M币记录* |
| -- | -- |
| **接口地址** | */integralcenter/mcoin* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|records|得分记录|<code>array</code>|是|暂无|无|
|currcoin|当前M币|<code>digit</code>|是|暂无|无|
|currcoin|历史M币|<code>digit</code>|是|暂无|无|

参数项：records

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|mcoin|M币|<code>digit</code>|是|暂无|无|
|createtime|时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
##接口示例

```
暂无
```


#星值记录
>暂无

| 接口名称 | *星值记录* |
| -- | -- |
| **接口地址** | */integralcenter/starval* |
| **请求方式** | <mark>GET</mark> |
| **数据格式** | <code>JSON</code> |


##请求参数
[<公共传入参数>](../README.md)  
[<公共翻页参数>](../README.md)

##返回参数
[<公共返回参数>](../README.md)

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|data|返回数据|<code>object</code>|是|暂无|无|

参数项：data

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|records|得分记录|<code>array</code>|是|暂无|无|
|currstarval|当前星值|<code>digit</code>|是|暂无|无|

参数项：records

|编码|名称|类型|必输|说明|默认值|
|:---|:---|:---|:--:|:---|:-----|
|starval|星值|<code>digit</code>|是|暂无|无|
|createtime|时间|<code>string</code>|是|yyyy-MM-dd HH:mm:ss|无|
##接口示例

```
暂无
```