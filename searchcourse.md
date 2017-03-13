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
| body | 返回消息体 | 对象 | 1 | - |
| courseDesc| 课程描述 | string | 2 |body |
| courseName| 课程名称 | string | 2 |body |
| courseId| ID | long | 2 |body |
| imgPath1| 课程介绍图片1 | string | 2 |body |
| learnNum| 学习次数 | long | 2 |body |

* 样例返回

    
    {
        "method":"searchCourse",
        "result": 
        {
            "code": "0", 
            "message": "SUCCESS"
        }, 
        "body":
        [
            {
            "courseId": "10004501", 
            "courseName": "年之前赫兹一院", 
            "courseDesc": "不不不不不不不不不不", 
            "learnNum": "951"
            },
            {
            "courseId": "10004795", 
            "courseName": "产量医药水蒸气星宿章", 
            "courseDesc": "啊啊啊啊啊啊啊", 
            "learnNum": "809"
            }
            ...
        ] 
    }

