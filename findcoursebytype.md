# 课程详情

#### **请求说明**

* 请求方法 findCourseByType

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| unitId| 单位ID | long | 是 |
| courseTypeId| 课程类别ID | long | 是 |
| pageIndex| 请求页码 | int| 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| res | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | res |
| msg| 返回说明 | string | 2 | res |
| courseList| 课程列表 | 对象数组 | 1 | - |
| courseDesc| 课程描述 | string | 2 |courseList|
| courseName| 课程名称 | string | 2 |courseList|
| courseSrc| 课程来源 | string | 2 |courseList|
| courseType| 课程分类 | string | 2 |courseList|
| createTime| 创建时间 | long| 2 |courseList|
| courseid| 课程ID | long | 2 |courseList|
| ifRequired | 是否必修 | int | 2 |courseList|
| imgPath1| 课程介绍图片1 | string | 2 |courseList|
| imgPath2| 课程介绍图片2 | string | 2 |courseList|
| imgPath3| 课程介绍图片3 | string | 2 |courseList|
| learnNum| 学习次数 | long | 2 |courseList|
| unitId| 单位ID | long | 2 |courseList|
| ifRequired | 是否必修 | int | 2 |courseList|

* 样例返回

    
    {
        "res": 
        {
            "resCode": "1", 
            "resMessage": "Operation is successful"
        },
        "courseList":
        [
           { "courseName":"语文"},
            ...
        ] 
    }

