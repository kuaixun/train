# 课程类别列表

#### **请求说明**

* 请求方法 findCourseType

* 请求参数
**注意：courseTypeId如果不传，则返回整颗树**

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| courseTypeId| 课程类别ID | long | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result |
| message| 返回说明 | string | 2 | result |
| body | 返回消息体 | 对象 | 1 | - |
| courseTypeId| 课程类别ID| long | 2 | body|
| pid| 父节点ID | long| 2 | body|
| sort| 排序字段 | int| 2 | body|
| sons| 子节点 | 对象数组| 2 | body|
| typeName| 课程类别名称 | string | 2 | body|


* 样例返回


    {
    "method":"findCourseType",
    "result": {
        "code": "0", 
        "message": "SUCCESS"
    },
    "body":
       { 
           "typeName":"语文"
                "sons": [
                    {
                        "courseTypeId": "1001", 
                        "typeName": "客服培训", 
                        "sons": [ ]
                    }, 
                    {
                        "courseTypeId": "1007", 
                        "typeName": "市场营销", 
                        "sons": [ ]
                    }, 
                    {
                        "courseTypeId": "1009", 
                        "typeName": "接听宝典", 
                        "sons": [ ]
                    }, 
                    {
                        "courseTypeId": "1010", 
                        "typeName": "服务指南", 
                        "sons": [ ]
                    }, 
                    {
                        "courseTypeId": "1012", 
                        "typeName": "班主进阶", 
                        "sons": [ ]
                    }, 
                    {
                        "courseTypeId": "1014", 
                        "typeName": "自学资料", 
                        "sons": [
                                    {
                                "courseTypeId": "1015", 
                                "pid": "1014", 
                                "typeName": "自我提升", 
                                "sons": []
                                    }, 
                                    {......}, 
                                    {......}
                                ]
                    }
                ]
       },
            ...
    }
