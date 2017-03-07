# 根据关键字搜索课程

#### **请求说明**

* 请求方法 searchCourse

* 请求参数
**pageIndex不传默认为首页**


| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| unitId| 单位ID | long | 是 |
| query | 关键字 | string | 否 |
| pageIndex| 请求页码 | int | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象数组 | 1 | - |
| courseDesc| 课程描述 | string | 2 |body |
| courseName| 课程名称 | string | 2 |body |
| courseSrc| 课程来源 | string | 2 |body |
| courseType| 课程分类 | string | 2 |body |
| createTime| 创建时间 | long| 2 |body |
| courseid| ID | long | 2 |body |
| ifRequired | 是否必修 | int | 2 |body |
| imgPath1| 课程介绍图片1 | string | 2 |body |
| imgPath2| 课程介绍图片2 | string | 2 |body |
| imgPath3| 课程介绍图片3 | string | 2 |body |
| unitId| 单位ID | long | 2 |body |
| learnNum| 学习次数 | long | 2 |body |
| ifRequired | 是否必修 | int | 2 |body |

* 样例返回

    
    {
        "method":"searchCourse",
        "result":
        {
            "code": "1",
            "message": "Operation is successful"
        },
        "body":
        [
           {"courseName":"语文"},
            ...
        ] 
    }

