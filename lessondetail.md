# 课件详情

#### **请求说明**

* 请求方法 findLessonById

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| lessonId| 课件id| long | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| courseId| 课程ID| long | 2 | body|
| createTime| 创建时间 | long| 2 | body|
| filePath | 文件路径 | string | 2 | body|
| lessonId| ID | string | 2 | body|
| keyWords | 关键字 | string | 2 | body|
|lessonDesc| 培训内容概述 | string | 2 | body|
|lessonMode| 文件格式 | int | 2 | body|
|lessonSubject | 课件名称 | string | 2 | body|
|mainPoints | 学习要点 | string | 2 | body|
|range| 适用范围 | string | 2 | body|
|teacher | 讲师 | string | 2 | body|
|trainTime | 培训时长 | int | 2 | body|
|translateFilePages | 转换后文件路径 | string | 2 | body|
|unitId| 单位ID | long | 2 | body|

* 样例返回


    {
        "method":"findLessonById",
            "result":
            {
            "code": "1",
            "message": "Operation is successful"
            },
        "body":
           { 
               "lessonSubject":"语文"
           },
            ...
    }