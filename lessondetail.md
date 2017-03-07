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
| code | 返回码| int | 2 | res |
| message| 返回说明 | string | 2 | res |
| body | 返回消息体 | 对象 | 1 | - |
| courseId| 课程ID| long | 2 | lesson|
| createTime| 创建时间 | long| 2 | lesson|
| filePath | 文件路径 | string | 2 | lesson|
| lessonId| ID | string | 2 | lesson|
| keyWords | 关键字 | string | 2 | lesson|
|lessonDesc| 培训内容概述 | string | 2 | lesson|
|lessonMode| 文件格式 | int | 2 | lesson|
|lessonSubject | 课件名称 | string | 2 | lesson|
|mainPoints | 学习要点 | string | 2 | lesson|
|range| 适用范围 | string | 2 | lesson|
|teacher | 讲师 | string | 2 | lesson|
|trainTime | 培训时长 | int | 2 | lesson|
|translateFilePages | 转换后文件路径 | string | 2 | lesson|
|unitId| 单位ID | long | 2 | lesson|

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
               "lessonSubject":"语文"
           },
            ...
    }