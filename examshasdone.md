# 已考试卷列表

#### **请求说明**

* 请求方法 findExamsHasDone
* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| userId| 用户id | long | 是 |
| pageIndex| 当前页码 | int | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | res |
| message| 返回说明 | string | 2 | res |
| body | 返回消息体 | 对象 | 1 | - |
| during| 考试时长| int | 2 | examResult|
| examEndTime| 考试结束时间 | string | 2 | examResult|
| examId| 试卷ID | long | 2 | examList|
| examLimitTime| 考试终止时间 | string | 2 | examResult|
| examStartTime| 考试开始时间 | string | 2 | examResult|
| examEndTime| 考试结束时间 | string | 2 | examResult|
| rightCount| 答题正确数| int | 2 | examResult|
| score| 成绩 | int | 2 | examResult|
| totalCount| 用户答题总数 | int| 2 | examResult|
| wrongCount| 用户答题错误数 | int | 2 | examResult|



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
        "during":50
        },
        ...
}
