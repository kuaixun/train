# 试卷列表(包含已考与未考)

#### **请求说明**

* 请求方法 findExamList
* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| uid| 用户id | long | 是 |
| unitId| 单位ID | long | 是 |
| pageIndex| 当前页码 | int | 否 |

* 返回参数

**body里面的notDoList和doneList分别为未考列表和已考列表**

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| notDoList| 未考试卷列表 | 对象数组 | 2 | body |
| doneList | 已考试卷列表 | 对象数组 | 2 | body |
| examTime| 考试时长| int| 3 | notDoList|
| examId | ID | long | 3 | notDoList|
| judgeNum| 判断题数量 | int | 3 | notDoList|
| questionNum | 简答题数量 | int | 3 | notDoList|
| selectManyNum | 多选题数量 | int | 3 | notDoList|
| selectOneNum | 单选题数量 | int | 3 | notDoList|
| standardScore | 达标分数线 | int | 3 | notDoList|
| during| 考试时长| int | 3 | doneList|
| examUserLogId| 已答试卷ID | long | 3 | doneList|
| examLimitTime| 考试终止时间 | string | 3 | doneList|
| examStartTime| 考试开始时间 | string | 3 | doneList|
| examEndTime| 考试结束时间 | string | 3 | doneList|
| rightCount| 答题正确数| int | 3 | doneList|
| score| 成绩 | int | 3 | doneList|
| totalCount| 用户答题总数 | int| 3 | doneList|
| wrongCount| 用户答题错误数 | int | 3 | doneList|

* 样例返回


    {
    "method":"findExamList",
        "result":
        {
        "code": "0",
        "message": "SUCCESS"
        },
    "body":
        {
        "notDoList":[
            {
                "examTime":"36",
                "examId":"10000151",
                "judgeNum":"9",
                "questionNum":"1",
                "selectManyNum":"6",
                "selectOneNum":"7",
                "standardScore":"100"
            },
            {
                "examTime":"57",
                "examId":"10000150",
                "judgeNum":"9",
                "questionNum":"0",
                "selectManyNum":"5",
                "selectOneNum":"7",
                "standardScore":"100"
            },
            {
                "examTime":"52",
                "examId":"10000189",
                "judgeNum":"7",
                "questionNum":"1",
                "selectManyNum":"8",
                "selectOneNum":"6",
                "standardScore":"100"
            }
        ],
        "doneList":[

        ]
    }
    }

