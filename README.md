# Async
Asynchrouous task queue
看看GitHub怎么显示Markdown
## <a id ="379a3e8f5ebf32448aadf437a8427f78" name="379a3e8f5ebf32448aadf437a8427f78"></a> 1.10 查询信息

    /getInfo?uid=***

请求方式: GET
| 参数名 | 是否必须 | 参数类型 | 参数说明 | 示例 |
| ------ | -------- | -------- | -------- | ---- |
| uid    | 是        | String   | 用户id   |      |

返回数据格式:json
返回参数
| 参数名       | 是否必须  | 参数类型     | 参数说明               |
| ----------- | -------- | ----------- | -------------------- |
| resultCode  | 是       | int         | 0表示获取成功1 获取失败  |
| resultInfo  | 是       | String      | "success"或"failure"  |
| username    | 是       | String      | 用户名                |
| nickname    | 是       | String      |      昵称             |
| profile     | 是       | String      | 头像                  |
| level       | 是       | String      |      等级             |
| telephone   | 是       | String      |   电话                |
| born        | 是       | String      | 生日                  |

示例

设置成功:

```json
{
  "resultCode": 0,
  "resultInfo": "success",
  "username": "admin",
  "admin_password": "111111",
  "username": "test01",
  "nickname": "111111",
  "profile": "221221",
  "level": "",
  "telephone": "",
  "born": ""
}
```
