# 用户登录

#### **请求说明**

* 请求方法 userLogin

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| userCode | 工号 | string| 是 |
| password | 密码 | string | 是 |
| imsi | 设备号 | string | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result|
| message| 返回说明 | string | 2 | result|
| body | 返回消息体 | 对象 | 1 | - |
| headImg | 头像图片 | string | 2 | body |
| uid | ID | long | 2 | body |
| imsi | 手机imsi | string | 2 | body |
| unitId | - | long | 2 | body |
| userCode | - | string | 2 | body |
| userName | - | string | 2 | body |

* 样例返回

  ```
{
    "method": "login", 
    "body": {
        "uid": "636588", 
        "imsi": "181822510717764", 
        "userCode": "636588", 
        "userName": "美洲德文", 
        "unitId": "5180"
    }, 
    "result": {
        "code": "0", 
        "message": "SUCCESS"
    }
}

    ```



