# 首页内容

#### **请求说明**

* 请求方法 mainPage

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| unitId| 单位ID | long | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| method| 调用方法 | string | 1 | - |
| result | 调用结果 | 对象 | 1 | - |
| code | 返回码| int | 2 | result|
| message| 返回说明 | string | 2 | result|
| body | 返回消息体 | 对象 | 1 | - |
| bannerList | banner模块 | 对象数组 | 2 | body |
| recommandCoursesList| 推荐课程模块 | 对象数组 | 2 | body |
| latestCourseList | 最新课程模块 | 对象数组 | 2 | body |
| topCourseList| 课程排行榜模块 | 对象数组 | 2 | body |
| topVideoList | 视频排行榜模块 | 对象数组 | 2 | body |
| courseDesc| 课程描述 | string | 3 | （课程类通用）|
| courseName| 课程名称 | string | 3 |（课程类通用）|
| courseSrc| 课程来源 | string | 3 |（课程类通用）|
| courseType| 课程分类 | string | 3 | （课程类通用）|
| createTime| 创建时间 | long| 3 |（课程类通用）|
| courseId| ID | long | 3 | （课程类通用）|
| ifRequired | 是否必修 | int | 3 | （课程类通用）|
| imgPath1| 课程介绍图片1 | string | 3 | （课程类通用）|
| imgPath2| 课程介绍图片2 | string | 3 |（课程类通用）|
| imgPath3| 课程介绍图片3 | string | 3 |（课程类通用）|
| learnNum| 学习次数 | long | 3 |（课程类通用）|
| unitId| 单位ID | long | 3 | （课程类通用）|
| ifRequired | 是否必修 | int | 3 |（课程类通用）|
| courseId| 课程ID| long | 3 | topVideoList|
| createTime| 创建时间 | long| 3 | topVideoList|
| filePath | 文件路径 | string | 3 | topVideoList|
| lessonId| ID | long| 3 | topVideoList|
| keyWords | 关键字 | string | 3 | topVideoList|
|lessonDesc| 培训内容概述 | string | 3 | topVideoList|
|lessonMode| 文件格式 | int | 3 | topVideoList|
|lessonSubject | 课件名称 | string | 3 | topVideoList|
|mainPoints | 学习要点 | string | 3 | topVideoList|
|range| 适用范围 | string | 3 | topVideoList|
|teacher | 讲师 | string | 3 | topVideoList|
|trainTime | 培训时长 | int | 3 | topVideoList|
|translateFilePages | 转换后文件路径 | string | 3 | topVideoList|
|unitId| 单位ID | long | 3 | topVideoList|


* 样例返回


      {
        "method":"mainPage",
        "result":
        {
        "code": "1",
        "message": "Operation is successful"
        },
        "body":
        {
           "bannerList":
           [
               {"":""}
               ...
           ],
           "recommandCoursesList":
           [
               {"courseId":123456}
               ...
           ],
           "latestCourseList":
           [
               {"courseId":123456}
               ...
           ],
           "topCourseList":
           {
               {"courseId":123456}
               ...
           },
           "topVideoList":
            [
               {"courseId":123456}
               ...
            ]
        } 
    }