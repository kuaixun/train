# 课程详情

#### **请求说明**

* 请求方法 findCourseInfoByIds

* 请求参数


| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| courseId| 课程id | long| 是 |

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
| filePath | 文件路径 | string | 3 | lessonList|
| lessonId| ID | string | 3 | lessonList|
|lessonDesc| 培训内容概述 | string | 3 | lessonList|
|lessonMode| 文件格式 | int | 3 | lessonList|
|lessonSubject | 课件名称 | string | 3 | lessonList|
|translateFilePages | 转换后文件路径 | string | 3 | lessonList|



* 样例返回

    
    {
    "method":"courseDetail",
    "result":
        {
        "code": "0",
        "message": "SUCCESS"
        },
    "body": {
        "courseName": "年之前赫兹一院", 
        "courseDesc": "驼鹿, 过程, 副将", 
        "courseId": "10004501", 
        "lessonList": 
            [
                {
                    "lessonId": "10033357", 
                    "lessonDesc": "班尼特乐调", 
                    "lessonMode": "0", 
                    "lessonSubject": "束棒阿依在公元"
                }, 
                {
                    "lessonId": "10033358", 
                    "lessonDesc": "或称为雪梨", 
                    "lessonMode": "0", 
                    "lessonSubject": "银矿女孩旧石"
                }
            ]
    }, 