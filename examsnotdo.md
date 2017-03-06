# 未考试卷列表

#### **请求说明**

* 请求方法 findExamsNotDo
* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| userId| 用户id | long | 是 |
| unitId| 单位ID | long | 是 |
| pageIndex| 当前页码 | int | 否 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| res | 调用结果 | 对象 | 1 | - |
| reCode | 返回码| int | 2 | res |
| resMessage| 返回说明 | string | 2 | res |
| examList| 课程列表 | 对象数组 | 1 | - |
| createTime| 创建时间| string | 2 | examList|
| createUser| 创建人 | string | 2 | examList|
| filePath | 文件路径 | string | 2 | examList|
| id| ID | string | 2 | examList|
| keyWords | 关键字 | string | 2 | examList|
|lessonDesc| 培训内容概述 | string | 2 | examList|
|lesson| 文件格式 | int | 2 | examList|
|lessonSubject | 课件名称 | string | 2 | examList|
|mainPoints | 学习要点 | string | 3 | lesson|
|range| 适用范围 | string | 3 | lesson|
|teacher | 讲师 | string | 3 | lesson|
|trainTime | 培训时长 | int | 3 | lesson|
|translateFilePages | 转换后文件路径 | string | 3 | lesson|
|unitId| 单位ID | long | 3 | lesson|

* 样例返回

  ```
  {
    "res": {
        "resCode": "1", 
        "resMessage": "Operation is successful"
    },
    "lesson":
    [
       { "lessonSubject":"语文"},
        ...
    ] 
}

