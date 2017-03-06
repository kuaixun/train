# 用户登录

#### **请求说明**

* 请求方法 _findInfoNByCoid5_

* 请求参数

| 字段 | 说明 | 类型 | 必须 |
| :--- | :--- | :--- | :--- |
| userCode | 工号 | long | 是 |
| password | 密码 | string | 是 |
| imsi | 设备号 | string | 是 |

* 返回参数

| 字段 | 说明 | 类型 | 级别 | 父节点 |
| :--- | :--- | :--- | :--- | :--- |
| res | 调用结果 | 对象 | 1 | - |
| code | 返回码：（1：成功；0：失败） | int | 2 | res |
| msg | 返回说明 | string | 2 | res |
|  |  |  |  |  |

* 一般频道响应示例

  ```
  {
    "res": {
        "code": "1", 
        "msg": "Operation is successful"
    }, 
    "picNews": [
        {
            "title": "壮观！数万只鹦鹉聚集饮水遮天蔽日", 
            "time": 1455775831928, 
            "source": "新华网", 
            "content_url": "http://go.10086.cn/surfnews/images/4061/20160218/5369992/5369992.html", 
            "imgUrl": "http://go.10086.cn/surfnews/images/4061/20160218/back/1454034002240.jpg", 
            "newsUrl": "http://news.xinhuanet.com/photo/2016-02/18/c_128730012.htm", 
            "isTop": 0, 
            "type": 2, 
            "bannerUrl": "http://go.10086.cn/surfnews/images/4061/20160218/back/1454034002240.jpg", 
            "open_type": 0, 
            "ctype": 0, 
            "is_energy": 1, 
            "positive_energy": 18412, 
            "negative_energy": 0, 
            "isComment": 0, 
            "comment_count": 0, 
            "updateTime": 1455775478000, 
            "rssId": 59322631, 
            "rssName": "网事联播", 
            "rssIcon": "http://go.10086.cn/hotpic/201506/01/source59322631.jpg", 
            "rssSource": "1", 
            "showType": 1003, 
            "newsId": 5369992, 
            "channelId": 4061, 
            "webView": 0, 
            "bigImg": "1", 
            "content_type": 1
        }
    ], 
    "news": [
        {
            "title": "微信提现收费动了谁的奶酪？", 
            "time": 1455762554000, 
            "source": "快讯", 
            "imgUrl": "http://go.10086.cn/surfnews/images/4061/20160218/back/1454034002186.jpg", 
            "dm":"600*800",
            "newsUrl": "http://go.10086.cn/surfnews/usr/surf/special/20160218/1323.html", 
            "isTop": 1, 
            "type": 1, 
            "open_type": 1, 
            "iconPath": "http://go.10086.cn/surfnews/usr/surf/icon/20151209174953.png", 
            "ctype": 0, 
            "multiImgUrl": [
                {
                    "imgUrl": "http://go.10086.cn/surfnews/images/4061/20160218/back/1454034002186.jpg"
                }, 
                {
                    "imgUrl": "http://go.10086.cn/surfnews/images/4061/20160218/back/1454034002188.jpg"
                }, 
                {
                    "imgUrl": "http://go.10086.cn/surfnews/images/4061/20160218/back/1454034002189.jpg"
                }
            ], 
            "is_energy": 0, 
            "isComment": 0, 
            "comment_count": 0, 
            "updateTime": 1455776734000, 
            "showType": 1002, 
            "newsId": 5363474, 
            "channelId": 4061, 
            "webView": 1, 
            "content_type": 1,
            "rssId": 59322631, 
            "rssName": "网事联播", 
            "rssIcon": "http://go.10086.cn/hotpic/201506/01/source59322631.jpg", 
            "rssSource": "1"
        }
    ]
  }
  ```

* 段子频道响应示例

```
{
    "res": {
        "reCode": "1", 
        "resMessage": "Operation is successful"
    }, 
    "picNews": [ ], 
    "news": [
        {
            "title": "老婆：老公我去隆胸吧？老公：好啊...", 
            "desc": "老婆：老公我去隆胸吧？
                老公：好啊。
                老婆：哼！你果然嫌我胸小。
                老公：......
                老婆：老公我去隆胸吧？
                老公：别去了。
                老婆：哼！你就是舍不得我花钱。
                老公：......", 
            "time": 1455678900000, 
            "source": "手机冲浪", 
            "content_url": "http://go.10086.cn/surfnews/images/4648023/20160217/5341892/5341892.html", 
            "isTop": 0, 
            "type": 1, 
            "open_type": 0, 
            "ctype": 0, 
            "isComment": 1, 
            "showType": 1003, 
            "newsId": 5341892, 
            "channelId": 4648023, 
            "webView": 0, 
            "upCount": 1286, 
            "downCount": 207, 
            "shareCount": 120, 
            "content": "老婆：老公我去隆胸吧？
                老公：好啊。
                老婆：哼！你果然嫌我胸小。
                老公：......
                老婆：老公我去隆胸吧？
                老公：别去了。
                老婆：哼！你就是舍不得我花钱。
                老公：......"
        }
    ]
}
```



