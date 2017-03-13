# 课程详情

#### **请求说明**

* 请求方法 findCourseInfoByIds

* 请求参数
**courseIds若为多个，中间以英文字符逗号隔开**


| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| courseIds| 课程id列表 | string| 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| courseDesc| 课程描述 | string | 2 |body|
| courseName| 课程名称 | string | 2 |body|
| courseId| ID | long | 2 |body|
| imgPath1| 课程介绍图片1 | string | 2 |body|
| lessonList| 课件列表 | 对象数组 | 2 |body|


* 样例返回

    
    {
    "method":"findCourseInfoByIds",
    "result":
        {
        "code": "1",
        "message": "Operation is successful"
        },
    "body":
        [
           { "courseName":"语文"},
            ...
        ]
    }