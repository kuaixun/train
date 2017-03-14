# 开始练习

#### **请求说明**

* 请求方法 startPractice
* 请求参数

| 字段 | 说明 | 类型 | 必须 |备注 |
| :--- | :--- | :--- | :--- |:--- |
| uid | 用户id | long | 是 |-|
| courseId| 课程id | long | 是 |-|
| uuid | 用户id | string | 是 |客户端自己生成一个唯一编号|
| practiceType|练习方式| int | 是 |1顺序练习 2随机练习|

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method | 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码 | int | 2 | result |
| message | 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| subjectList| 练习题列表 | 对象数组 | 2 | body |
| answer| 题目总数 | int| 3 | subjectList|
| degree| 难度系数 | int| 3 | subjectList|
| subjectId| ID | long| 3 | subjectList|
| score| 默认分数 | int| 3 | subjectList|
| subjectTitle| 题干 | string| 3 | subjectList|
| subjectType| 1-判断题，2-单选，3-多选，4-简答题 | int| 3 | subjectList|
| options| 选项| int| 3 | subjectList|
| optionId| 选项ID | long| 4 | options|
| optionDesc| 描述 | string| 4 | options|
| optionFlag|选项标识| string| 4 | options|
| sort| 排序 | int| 4 | options|
| score| 分数 | int| 4 | options|

* 样例返回

```
{
"method":"startPractice
",
"result":
    {
    "code": "0",
    "message": "SUCCESS"
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



