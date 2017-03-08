# 根据Id获取具体试卷

#### **请求说明**

* 请求方法 findExamById
* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| examId | 用户id | long | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method | 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码 | int | 2 | result |
| message | 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| examName | 试卷名称 | string | 2 | body |
| examTime | 考试时长 | string | 2 | body |
| examType | 试卷类别（是否模拟考试） | int | 2 | body |
| examId | ID | long | 2 | body |
| judgeNum | 判断题数量 | int | 2 | body |
| examTime | 简答题数量 | int | 2 | body |
| selectManyNum | 多选题数量 | int | 2 | body |
| selectOneNum | 单选题数量 | int | 2 | body |
| standardScore | 达标分数线 | int | 2 | body |
| totalNum | 试题总数 | int | 2 | body |
| examTime | 考试时长 | string | 2 | body |
| subjectLinks | 试题信息 | 对象数组 | 2 | body |
| examId | 试卷Id | long | 3 | subjectLinks |
| examSubjectId | 试卷习题ID | long | 3 | subjectLinks |
| subjectId | 题目id | long | 3 | subjectLinks |
| subjectIndex | 题目序号 | long | 3 | subjectLinks |

* 样例返回

```
{
"method":"findExamById",
"result":
    {~~~~~~~~
    "code": "1",
    "message": "Operation is successful"
    },
"body":
    {
        "examName":"试卷名称",
        "subjectLinks":
        [
            {"subjectId":123},
            ...
        ]
    },
    ...
}
```



