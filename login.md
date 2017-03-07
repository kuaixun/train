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
| res | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | res |
| msg | 返回说明 | string | 2 | res |
| user | 用户信息 | 对象 | 1 | - |
| address | 地址 | string | 2 | user |
| centerId | 所在分中心 | string | 2 | user |
| currentPhoto | 当前照片文件路径 | string | 2 | user |
| departmentId | 所在部门 | long | 2 | user |
| education | 学历 | int | 2 | user |
| email | 邮箱 | string | 2 | user |
| empiricValue | 经验值 | int | 2 | user |
| englishName | 英文名 | string | 2 | user |
| headImg | 头像图片 | string | 2 | user |
| userid | ID | long | 2 | user |
| idCard | 身份证号码 | string | 2 | user |
| imsi | 手机imsi | string | 2 | user |
| linkPhone | 联系电话 | string | 2 | user |
| nickName | 昵称 | string | 2 | user |
| positionId | 岗位id | long | 2 | user |
| sex | 性别 | string | 2 | user |
| teamId | 所在班组 | long | 2 | user |
| unitId | - | long | 2 | user |
| userCode | - | string | 2 | user |
| userLevel | 员工等级 | string | 2 | user |
| userName | - | string | 2 | user |

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



