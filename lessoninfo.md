# 课件详情

#### **请求说明**

* 请求方法 findLessonInfoByIds

* 请求参数
**courseIds若为多个，中间以英文字符逗号隔开**

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| courseIds| 课程id列表 | string | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | res |
| message| 返回说明 | string | 2 | res |
| body | 返回消息体 | 对象 | 1 | - |
| courseId| 课程ID| long | 2 | lessonList|
| createTime| 创建时间 | long| 2 | lessonList|
| filePath | 文件路径 | string | 2 | lessonList|
| lessonId| ID | string | 2 | lessonList|
| keyWords | 关键字 | string | 2 | lessonList|
|lessonDesc| 培训内容概述 | string | 2 | lessonList|
|lesson| 文件格式 | int | 2 | lessonList|
|lessonSubject | 课件名称 | string | 2 | lessonList|
|mainPoints | 学习要点 | string | 2 | lessonList|
|range| 适用范围 | string | 2 | lessonList|
|teacher | 讲师 | string | 2 | lessonList|
|trainTime | 培训时长 | int | 2 | lessonList|
|translateFilePages | 转换后文件路径 | string | 2 | lessonList|
|unitId| 单位ID | long | 2 | lessonList|

* 样例返回


    {
    "method":"userLogin",
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
