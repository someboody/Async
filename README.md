# Async
Asynchrouous task queue
## <a id ="379a3e8f5ebf32448aadf437a8427f78" name="379a3e8f5ebf32448aadf437a8427f78"></a> 1.10 获取飞播信息(废弃)

    http://116.62.64.180/dubbo-controller/getfeibomsg2?userId=***

请求方式: GET
| 参数名 | 是否必须 | 参数类型 | 参数说明 | 示例 |
| ------ | -------- | -------- | -------- | ---- |
| userId | 是       | String   | 用户id   |      |
返回数据格式:json
返回参数
| 参数名          | 是否必须 | 参数类型    | 参数说明                                                     |
| -------------- | -------- | ----------- | ------------------------------------------------------------ |
| resultCode     | 是       | int         | 0表示获取成功1 获取失败                                      |
| resultInfo     | 是       | String      | "success"或"failure"                                         |
| admin_username | 是       | String      | 注册飞播时的对应字段值,死数据暂时就返回死数据                |
| admin_password | 是       | String      |                                                              |
| username       | 是       | String      |                                                              |
| password       | 是       | String      |                                                              |
| domain         | 是       | String      |                                                              |
| userinfo       | 可选     | json String | 注册飞播时传递的包含用户信息的json字符串,没有暂时可不返回参数 |

示例

设置成功:

```json
{
  "resultCode": 0,
  "resultInfo": "success",
  "admin_username": "admin",
  "admin_password": "111111",
  "username": "test01",
  "password": "111111",
  "domain": "ORG_221",
  "userinfo": ""
}
```
