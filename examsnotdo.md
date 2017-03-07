# 未考试卷列表

#### **请求说明**

* 请求方法 findExamsNotDo
* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| userId| 用户id | long | 是 |
| unitId| 单位ID | long | 是 |
| pageIndex| 当前页码 | int | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | res |
| message| 返回说明 | string | 2 | res |
| body | 返回消息体 | 对象数组 | 1 | - |
| createTime| 创建时间| long| 2 | body|
| createUser| 创建人 | string | 2 | body|
| examTime| 考试时长| int| 2 | body|
| examType| 试卷类别 | string | 2 | body|
| examId | ID | long | 2 | body|
|judgeNum| 判断题数量 | int| 2 | body|
|questionNum| 简答题数量 | int | 2 | body|
|remark | 备注 | string | 2 | body|
|selectManyNum| 多选题数量 | string | 2 | body|
|selectOneNum| 单选题数量 | string | 2 | body|
|standardScore| 达标分数线 | string | 2 | body|


* 样例返回


    {
    "method":"findExamsNotDo",
        "result":
        {
        "code": "1",
        "message": "Operation is successful"
        },
    "body":
        [
           { "lessonSubject":"语文"},
            ...
        ] 
    }

