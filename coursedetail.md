# 课程详情

#### **请求说明**

* 请求方法 findCourseInfoByIds

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| courseIds| 课程id列表 | string(id之间以逗号隔开) | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| res | 调用结果 | 对象 | 1 | - |
| code| 返回码| int | 2 | res |
| msg| 返回说明 | string | 2 | res |
| course| 课程列表 | 对象数组 | 1 | - |
| courseDesc| 课程描述 | string | 2 |course|
| courseName| 课程名称 | string | 2 |course|
| courseSrc| 课程来源 | string | 2 |course|
| courseType| 课程分类 | string | 2 |course|
| createTime| 创建时间 | time| 2 |course|
| courseid| ID | long | 2 |course|
| ifRequired | 是否必修 | int | 2 |course|
| imgPath1| 课程介绍图片1 | string | 2 |course|
| imgPath2| 课程介绍图片2 | string | 2 |course|
| imgPath3| 课程介绍图片3 | string | 2 |course|
| learnNum| 学习次数 | long | 2 |course|
| unitId| 单位ID | long | 2 |course|
| ifRequired | 是否必修 | int | 2 |course|

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

