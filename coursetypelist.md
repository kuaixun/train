# 课程类别列表

#### **请求说明**

* 请求方法 findCourseType

* 请求参数
**注意：courseTypeId如果不传，则返回整颗树**

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| courseTypeId| 课程类别ID | long | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| courseTypeId| 课程类别ID| long | 2 | body|
| pid| 父节点ID | string | 2 | body|
| sort| 文件路径 | int| 2 | body|
| sons| 子节点 | 对象数组| 2 | body|
| typeName| 课程类别名称 | string | 2 | body|


* 样例返回


    {
    "method":"userLogin",
    "result":
        {
        "code": "1",
        "message": "Operation is successful"
        },
    "body":
       { 
           "typeName":"语文"
           “sons”:
           [
               {
               "courseType":
                   {...}
               }
               ...
           ]
       },
            ...
    }
