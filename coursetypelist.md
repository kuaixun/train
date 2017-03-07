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
| res | 调用结果 | 对象 | 1 | - |
| code| 返回码| int | 2 | res |
| msg| 返回说明 | string | 2 | res |
| courseType| 课程类别 | 对象| 1 | - |
| courseTypeId| 课程类别ID| long | 2 | courseType|
| pid| 父节点ID | string | 2 | courseType|
| sort| 文件路径 | int| 2 | courseType|
| sons| 子节点 | 对象数组| 2 | courseType|
| typeName| 课程类别名称 | string | 2 | courseType|


* 样例返回


    {
    "res": 
        {
            "code": "1", 
            "msg": "Operation is successful"
        },
    "courseType":
        [
           { "lessonSubject":"语文"},
            ...
        ] 
    }
