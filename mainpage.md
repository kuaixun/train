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
| res | 调用结果 | 对象 | 1 | - |
| code | 返回码：（1：成功；0：失败） | int | 2 | res |
| msg | 返回说明 | string | 2 | res |
* 样例返回

  ```
  {
    "res": {
        "resCode": "1", 
        "resMessage": "Operation is successful"
    },
    "user":{
        "userName":"张三",
        "education":"学历"
        ...
    } 
}

