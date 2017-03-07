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
| res | 调用结果 | 对象 | 1 | - |
| reCode | 返回码| int | 2 | res |
| resMessage| 返回说明 | string | 2 | res |
| lessonList| 课件列表 | 对象 | 1 | - |
| courseId| 课程ID| long | 3 | lessonList|
| createTime| 创建时间 | long| 3 | lessonList|
| filePath | 文件路径 | string | 3 | lessonList|
| lessonId| ID | string | 3 | lessonList|
| keyWords | 关键字 | string | 3 | lessonList|
|lessonDesc| 培训内容概述 | string | 3 | lessonList|
|lesson| 文件格式 | int | 3 | lessonList|
|lessonSubject | 课件名称 | string | 3 | lessonList|
|mainPoints | 学习要点 | string | 3 | lessonList|
|range| 适用范围 | string | 3 | lessonList|
|teacher | 讲师 | string | 3 | lessonList|
|trainTime | 培训时长 | int | 3 | lessonList|
|translateFilePages | 转换后文件路径 | string | 3 | lessonList|
|unitId| 单位ID | long | 3 | lessonList|

* 样例返回


    {
    "res": 
        {
            "code": "1", 
            "msg": "Operation is successful"
        },
    "lessonList":
        [
           { "lessonSubject":"语文"},
            ...
        ] 
    }
