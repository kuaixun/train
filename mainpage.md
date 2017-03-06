# 首页内容

#### **请求说明**

* 请求方法 mainPage

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| unitId| 工号 | long | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| res | 调用结果 | 对象 | 1 | - |
| reCode | 返回码：（1：成功；其他：失败） | int | 2 | res |
| resMessage| 返回说明 | string | 2 | res |
| content| 首页内容 | 对象 | 1 | - |
| bannerList | banner模块 | 对象数组 | 2 | content |
| recommandCoursesList| 推荐课程模块 | 对象数组 | 2 | content |
| latestCourseList | 最新课程模块 | 对象数组 | 2 | content |
| topCourseList| 课程排行榜模块 | 对象数组 | 2 | content |
| topVideoList | 视频排行榜模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |
| bannerList | banner模块 | 对象数组 | 2 | content |

* 样例返回
  {
    "res": 
    {
        "resCode": "1", 
        "resMessage": "Operation is successful"
    },
    "content":
    {
       "bannerList":
       [
           {"":""}
           ...
       ],
       "recommandCoursesList":
       [
           {"":""}
           ...
       ],
       "latestCourseList":
       [
           {"":""}
           ...
       ],
       "topCourseList":
       {
           {"":""}
           ...
       },
       "topVideoList":
       [
           {"":""}
           ...
       ]
    } 
}

