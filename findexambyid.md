# 根据Id获取具体试卷

#### **请求说明**

* 请求方法 findExamById
* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| examId| 用户id | long | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象数组 | 1 | - |
| examName| 试卷名称| string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examType| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|
| examTime| 考试时长 | string | 2 | body|

* 样例返回
 
             
    {
    "method":"findExamById",
    "result":
        {
        "code": "1",
        "message": "Operation is successful"
        },
    "body":
        [
            {"during":50},
        ],
        ...
    }
