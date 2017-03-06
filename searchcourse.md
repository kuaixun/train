# 根据关键字搜索课程

#### **请求说明**

* 请求方法 searchCourse

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| unitId| 单位ID | long | 是 |
| query | 关键字 | string | 否 |
| pageIndex| 当前页码 | int | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| courseDesc| 课程描述 | string | 3 | （课程类通用）|
| courseName| 课程名称 | string | 3 |（课程类通用）|
| courseSrc| 课程来源 | string | 3 |（课程类通用）|
| courseType| 课程分类 | string | 3 | （课程类通用）|
| createTime| 创建时间 | string | 3 |（课程类通用）|
| id| ID | long | 3 | （课程类通用）|
| ifRequired | 是否必修 | int | 3 | （课程类通用）|
| imgPath1| 课程介绍图片1 | string | 3 | （课程类通用）|
| imgPath2| 课程介绍图片2 | string | 3 |（课程类通用）|
| imgPath3| 课程介绍图片3 | string | 3 |（课程类通用）|
| unitId| 单位ID | long | 3 | （课程类通用）|
| ifRequired | 是否必修 | int | 3 |（课程类通用）|

* 样例返回

  ```
  {
    "res": {
        "resCode": "1", 
        "resMessage": "Operation is successful"
    },
    "user":{
        "userName":"张三",
        "education":"学历"
        ...
    } 
}

