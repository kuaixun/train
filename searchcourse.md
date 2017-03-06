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
| res | 调用结果 | 对象 | 1 | - |
| reCode | 返回码| int | 2 | res |
| resMessage| 返回说明 | string | 2 | res |
| courseList| 课程列表 | 对象数组 | 1 | - |
| courseDesc| 课程描述 | string | 2 |courseList|
| courseName| 课程名称 | string | 2 |courseList|
| courseSrc| 课程来源 | string | 2 |courseList|
| courseType| 课程分类 | string | 2 |courseList|
| createTime| 创建时间 | string | 2 |courseList|
| id| ID | long | 2 |courseList|
| ifRequired | 是否必修 | int | 2 |courseList|
| imgPath1| 课程介绍图片1 | string | 2 |courseList|
| imgPath2| 课程介绍图片2 | string | 2 |courseList|
| imgPath3| 课程介绍图片3 | string | 2 |courseList|
| unitId| 单位ID | long | 2 |courseList|
| ifRequired | 是否必修 | int | 2 |courseList|

* 样例返回

  ```
  {
    "res": {
        "resCode": "1", 
        "resMessage": "Operation is successful"
    },
    "courseList":
    [
       {"courseName":"语文"},
        ...
    ] 
}

