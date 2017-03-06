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
| res | 调用结果 | 对象 | 1 | - |
| reCode | 返回码| int | 2 | res |
| resMessage| 返回说明 | string | 2 | res |
| examList| 课程列表 | 对象数组 | 1 | - |
| during| 考试时长| int | 2 | examList|
| examEndTime| 考试结束时间 | string | 2 | examList|
| examTime| 考试时长| int| 2 | examList|
| examType| 试卷类别 | string | 2 | examList|
| id | ID | long | 2 | examList|
|judgeNum| 判断题数量 | int| 2 | examList|
|questionNum| 简答题数量 | int | 2 | examList|
|remark | 备注 | string | 2 | examList|
|selectManyNum| 多选题数量 | string | 2 | examList|
|selectOneNum| 单选题数量 | string | 2 | examList|
|standardScore| 达标分数线 | string | 2 | examList|


* 样例返回

  ```
  {
    "res": {
        "resCode": "1", 
        "resMessage": "Operation is successful"
    },
    "lesson":
    [
       { "lessonSubject":"语文"},
        ...
    ] 
}

