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
| questionNum| 简答题数量 | int | 2 | body |
| selectManyNum | 多选题数量 | int | 2 | body |
| selectOneNum | 单选题数量 | int | 2 | body |
| standardScore | 达标分数线 | int | 2 | body |
| totalNum | 试题总数 | int | 2 | body |
| examTime | 考试时长 | string | 2 | body |
| subjectList | 试题信息 | 对象数组 | 2 | body |
| examId | 试卷Id | long | 3 | subjectList|
| examSubjectId | 试卷习题ID | 对象数组 | 3 | subjectList|
| answer| 正确答案 | string| 3 | subjectList|
| degree| 难度系数 | int| 3 | subjectList|
| subjectId| ID | long| 3 | subjectList|
| score| 默认分数 | int| 3 | subjectList|
| subjectTitle| 题干 | string| 3 | subjectList|
| subjectType| 1-判断题，2-单选，3-多选，4-简答题 | int| 3 | subjectList|
| options| 选项| 对象数组| 3 | subjectList|
| optionId| 选项ID | long| 4 | options|
| optionDesc| 描述 | string| 4 | options|
| optionFlag|选项标识| string| 4 | options|
| sort| 排序 | int| 4 | options|
| score| 分数 | int| 4 | options|

* 样例返回

```
{
"method":"findExamById",
"result":
    {
    "code": "1",
    "message": "Operation is successful"
    },
"body":
    {
        "examName":"攻势萨迈拉情态",
        "examTime":"36",
        "examId":"10000151",
        "judgeNum":"9",
        "totalNum":"23",
        "questionNum":"1",
        "selectManyNum":"6",
        "selectOneNum":"7",
        "standardScore":"100",
        "subjectList":[
            {
                "answer":"1",
                "degree":"1",
                "subjectId":"10000151",
                "score":"3",
                "subjectTitle":"'迪克西意思吗？",
                "subjectType":"1",
                "options":[
                    {
                        "optionId":"10285208",
                        "optionDesc":"665",
                        "optionFlag":"A",
                        "sort":"0"
                    },
                    {
                        "optionId":"10285209",
                        "optionDesc":"210",
                        "optionFlag":"B",
                        "sort":"1"
                    },
                    {
                        "optionId":"10285210",
                        "optionDesc":"三一神",
                        "optionFlag":"C",
                        "sort":"2"
                    },
                    {
                        "optionId":"10285211",
                        "optionDesc":"336",
                        "optionFlag":"D",
                        "sort":"3"
                    }
                ]
            },
            {
                "answer":"1",
                "degree":"1",
                "subjectId":"10000151",
                "score":"3",
                "subjectTitle":"'迪克西的意思吗？",
                "subjectType":"1",
                "options":[
                    {
                        "optionId":"10285208",
                        "optionDesc":"665",
                        "optionFlag":"A",
                        "sort":"0"
                    },
                    {
                        "optionId":"10285209",
                        "optionDesc":"210",
                        "optionFlag":"B",
                        "sort":"1"
                    },
                    {
                        "optionId":"10285210",
                        "optionDesc":"三一神",
                        "optionFlag":"C",
                        "sort":"2"
                    },
                    {
                        "optionId":"10285211",
                        "optionDesc":"336",
                        "optionFlag":"D",
                        "sort":"3"
                    }
                ]
            },
            {
                "answer":"1",
                "degree":"1",
                "subjectId":"10000151",
                "score":"3",
                "subjectTitle":"'迪克西意思吗？",
                "subjectType":"1",
                "options":[
                    {
                        "optionId":"10285208",
                        "optionDesc":"665",
                        "optionFlag":"A",
                        "sort":"0"
                    },
                    {
                        "optionId":"10285209",
                        "optionDesc":"210",
                        "optionFlag":"B",
                        "sort":"1"
                    },
                    {
                        "optionId":"10285210",
                        "optionDesc":"三一神",
                        "optionFlag":"C",
                        "sort":"2"
                    },
                    {
                        "optionId":"10285211",
                        "optionDesc":"336",
                        "optionFlag":"D",
                        "sort":"3"
                    }
                ]
            }
        ]
    }
}
```



