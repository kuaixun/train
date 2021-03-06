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
    "method":"startPractice",
    "result":
        {
        "code": "0",
        "message": "SUCCESS"
        },
    "body":
        {
    "subjectList":[
            {
                "answer":"C",
                "degree":"3",
                "subjectId":"10098706",
                "score":"3",
                "subjectTitle":"'军力同年：",
                "subjectType":"2",
                "options":[
                    {
                        "optionId":"10285204",
                        "optionDesc":"949",
                        "optionFlag":"A",
                        "sort":"0"
                    },
                    {
                        "optionId":"10285205",
                        "optionDesc":"242",
                        "optionFlag":"B",
                        "sort":"1"
                    },
                    {
                        "optionId":"10285206",
                        "optionDesc":"索契",
                        "optionFlag":"C",
                        "sort":"2"
                    },
                    {
                        "optionId":"10285207",
                        "optionDesc":"300",
                        "optionFlag":"D",
                        "sort":"3"
                    }
                ]
            },
            {
                "answer":"C",
                "degree":"1",
                "subjectId":"10098708",
                "score":"1",
                "subjectTitle":"'暴力迷信：",
                "subjectType":"2",
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



