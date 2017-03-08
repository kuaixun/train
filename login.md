# 用户登录

#### **请求说明**

* 请求方法 userLogin

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| userCode | 工号 | long | 是 |
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
| departmentId | 所在部门 | long | 2 | body |
| email | 邮箱 | string | 2 | body |
| empiricValue | 经验值 | int | 2 | body |
| headImg | 头像图片 | string | 2 | body |
| userid | ID | long | 2 | body |
| idCard | 身份证号码 | string | 2 | body |
| imsi | 手机imsi | string | 2 | body |
| linkPhone | 联系电话 | string | 2 | body |
| nickName | 昵称 | string | 2 | body |
| positionId | 岗位id | long | 2 | body |
| sex | 性别 | string | 2 | body |
| teamId | 所在班组 | long | 2 | body |
| unitId | - | long | 2 | body |
| userCode | - | string | 2 | body |
| userLevel | 员工等级 | string | 2 | body |
| userName | - | string | 2 | body |

* 样例返回

  ```
  {
    "method":"userLogin",
    "result": 
    {
        "code": "1", 
        "message": "Operation is successful"
    },
    "body":
    {
        "userName":"张三",
        "education":"学历"
        ...
    } 
}

    ```



