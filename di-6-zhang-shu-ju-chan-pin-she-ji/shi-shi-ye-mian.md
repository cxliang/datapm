## 秋毫明察，实时数据产品一览 {#activity-name}



> 研究国外数据产品，了解当前实现数据价值的最新思路和实践。这是大数据产品漫游系列的第 **2** 篇文章。

实时数据的展现，是现今很多数据产品的一个重要表现形式。远如 Google Analytics 这种传统的分近如天析工具，猫每年双十一的大屏展示，新兴产品 GrowingIO 也都有实时统计分析的功能。从实时的应用场景来看，主要有以下两种：

> 1. 实时监控类：侧重于短时间内数据呈现，不展示当天的累计数据，如 Google Analytics, Gosquared, Chartbeat, Kissmetric 等
>
> 2. 实时统计类：侧重于当天的累计数据呈现，实时反映数据变化，如 Woopra, Gauges，腾讯云分析，天猫大屏等

  


无论是以哪种目的为主，核心思路都是以用户为分析主体，进行各个维度的对比和细分。接下来与大家分享几款数据产品的实时功能，主要从 **功能亮点，更新频率和指标维度内容** 三个角度进行分析，希望能给大家提供一点灵感。

￼ ￼ ￼ ￼

## 1. Google Analytics

￼![](http://mmbiz.qpic.cn/mmbiz_gif/cVia3Ayib6tISWsx8cGytwPJXXHicXsO2K71YLOR9WUP6RMVgyYoHswuqKc4Nia0IHgNOZ6HoErnulZZupGdoicTdBw/0?wx_fmt=gif&tp=webp&wxfrom=5&wx_lazy=1)  


GA 关于用户数量水位式的可视化设计，解决了秒级和分钟级的显示问题，让用户随时间的变化和累计变得一目了然。 它主要通过对实时在线用户的多维度细分，来分析用户来源，用户分布和用户使用情况。

1. 功能亮点:

2. * 分维度细分采用列表的形式，在刷新时通过红绿色显示排名上升下降 ，营造实时的真实感

   * 在细分维度的下钻页面，提供了活跃用户和浏览量\(近30min切换\)， 解决了我们之前讨论的在较长时 间维度上观察投放效果的问题

   * 每个维度细分均提供下钻功能，可在多个维度交叉作用下查看实时在线用户
3. 更新频率10s

4. 指标内容及维度:

5. * 指标:活跃用户数

   * 用户来源：引荐来源，社交流量，关键字

   * 用户分布：设备类型，地理位置

   * 用户使用维度：内容\(活跃网页\) ，事件，转化

￼ ￼

## 2. GoSquared

￼![](http://mmbiz.qpic.cn/mmbiz_gif/cVia3Ayib6tISWsx8cGytwPJXXHicXsO2K7n5NEufTibZKibE0WFoK2oypEhrTuGzl7iaed4YOppZDhniaHxlMzjdl8Uw/0?wx_fmt=gif&tp=webp&wxfrom=5&wx_lazy=1)  


Gosquared 是一个成立于 2006 年的老牌厂商（从它的界面就可以看出来了），主要卖点就是实时功能。它可以追踪到6h内所有用户的访问内容和使用细节， 在及时性和全面性都做得不错。 同时，它在很多细节上可圈可点，如直接将当前访客数显示在网页标签上，这样即使你在浏览其他网页也能监控到自己网站的访客数量。

1. 功能亮点：

2. * 在用户细查上，会不断更新每个有新动作的用户 并在旁边读秒，显示最后更新情况。点击该用户可查看详情，包括Session内动作和用户详情。这里最多包括6h前的用户活动

   * 地图分布可点击放大，在大图上查看数据的变化，不过放大后 在动态性做的不是很好![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfgqcQxmnos3R4KxUjwBf6VLAiaFrGOCK2PCSAiaIPQX0uqoictBWkN4y8A/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)  

   * 可以设定流量提醒，RSS提醒和增加里程碑点来记录数据的变化。订阅提醒支持推特/博客/Github 等内容更新订阅![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfRaiazBicrKpvO3iaIGcfjAayxiasxOZhlb7XHSys4RppuQDFJSBvwFu9YQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)  
3. 更新频率:各模块单独实时更新

4. 指标内容及维度:

5. * 指标：活跃用户数，访问时长/深度\(平均值及分布情况\)，活跃用户占比。通过将活跃用户数与七天内 MIN/MAX 值 和以前的时间进行比较，让用户更容易判断

   * 用户来源：访问来源。每个访问来源，国家和访客都用图标代替，美观度提升很多。点击访问来源/内容，能看到该网站下的详细网址，客户可以直接点击查看该网址内容，确认自己的用户从何而来

     ![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfc28dcjCYMbDcIMib3heic0WqcZ9QgA8FV6WzOH2P4LFzxJNarRm5I5dw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)  

   * 用户分布：设备类型，操作系统，浏览器类型，地理位置，语言，

   * 用户使用：内容\(活跃网页\)，用户细查

   * 用户属性维：回访用户，标签用户

## 3. Kissmetrics

￼ ￼![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfLZZDsEJboTLrajcricd1PRAib10THtlPe9CSnhWIng0ZuCC3EG24MCZQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)  


以实时展现用户活动为主，并对当前使用内容做个简单统计，实时的用户细查是最大特色。这点我在后续的产品设计中借鉴了这点，并结合自身的产品特色，设计了实时展示所有用户行为的功能。

1. 功能亮点

2. * 可以针对某个特殊的用户，动作或分群进行筛选查看，这在其 他产品中是没有的。

   * 点击某个用户 ID 可以下钻查看用户的 Profile

   * 提供 My activity 来查看自己的活动，方便 debug....（这个功能莫名戳中萌点）
3. 更新频率:可以自主调整更新频率

4. 指标内容及维度:

5. * 当天累计用户数，以及 Top5 用户的事件数

   * 当天累计事件数，以及Top5 事件的事件数

   * 当天累计元素数，以及Top5 元素的事件数

￼

## 4. Chartbeat

￼![](http://mmbiz.qpic.cn/mmbiz_gif/cVia3Ayib6tISWsx8cGytwPJXXHicXsO2K7zItZibB0bt9PZbcicziboTcXy0d2YaLpVWL3CBwNyHO4nibIutgiawscfXg/0?wx_fmt=gif&tp=webp&wxfrom=5&wx_lazy=1)  


Chartbeat 是一个主要服务于在线新闻和文章监控的公司，产品定位在口号十分明确：Your audience's attention is worth more than their clicks. 它以实时展现访问内容为主，并根据每条内容显示访问来源及其比例。所以基本上能够锁定住每发一篇文章，效果如何一眼便知，根据数据情况快速修改发布。

1. 功能亮点

2. * 监控功能:Spike Alert 和 Overperforming\(当值超过最大值突出显示\)  
  


     ![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtf3HsMFtmriamyjFjOc5sApAUWSbqExHt7lcabHLibZYSypT4eYSAnkYZA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

     ![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtf2jzqDgqIac9D5ZeEp0v0SwJp9ZmZSdiblMCdnN7V0dtWtfOGFn2V2lQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

   * 多层过滤:可以选择页面中所有维度进行过滤，满足客户分析某个特定来源用户的使用情况
3. 更新频率:实时

4. 指标内容及维度:

5. * 指标：活跃用户数，Recirculation，访问 时长

   * 用户来源：引荐来源，访问来源 ，Distribution，社交来源

   * 用户分布：设备类型，地理位置

   * 用户使用：内容\(活跃网页\)

   * 用户属性：新客户/回访/忠诚 ￼ ￼ ￼ ￼ ￼

## 5.实时统计产品

实时统计方面，主要是是比较明确的累计场景，如当天的总购买用户数，总订单数等等。出彩的产品不多，这里简单给大家介绍下。

* Woopra：主打定制化的图表 Widget，以实现更加灵活的数据分析。实时模块也遵循了这个思路。

![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfRsOoxRQgvf1o9icficJgGdiaO4kuQ44VxjpGwcjfbB6IcqicoSVV5iajiatQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)  


  


* 腾讯云分析：腾讯的分析产品，中规中矩  

![](http://mmbiz.qpic.cn/mmbiz_gif/cVia3Ayib6tISWsx8cGytwPJXXHicXsO2K7vJwHSWsQpQq42mekqfY046ibiaMdDsK4s1loz8q0N3yn8jfpJ1hokaQQ/0?wx_fmt=gif&tp=webp&wxfrom=5&wx_lazy=1)  


  


* 天猫双十一大屏  

![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfWEK4Hp9ciapZTJhYk7UofO4D4vatdV3ia43jXpJ9OKTibcXDSgg5NribnQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)  


## 6. GrowingIO 实时监控统计

最后介绍下我曾经设计的 GrowingIO 实时功能，据后台统计，是当时 GrowignIO 所有功能中停留时长最长的一个，可能是很多人就挂在当前页面不走了吧...

在充分借鉴了实时监控和统计两家所长后，我们确定了**监控为主，统计为辅** 的设计策略，核心在于让客户能够了解当前用户情况，并迅速定位异常。在分析指标和维度上与其他家大同小异，以下是 V1.0 产品动图：（建议横过手机来看😁）

![](http://mmbiz.qpic.cn/mmbiz_gif/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfW0fJFNFMADN5bqlicriaXasA7mOQQR5HpotqAOH6xH2mslFQkSRYlpng/0?wx_fmt=gif&tp=webp&wxfrom=5&wx_lazy=1)  


  


文末附上各家产品在指标和维度上的汇总，从中一窥可各家产品在实时分析上的重点和取舍，供大家参考。![](http://mmbiz.qpic.cn/mmbiz_png/cVia3Ayib6tIQ8F11j9XJyjXEh06vhMKtfpE6Ld6iaK3KibONNOEROT4SliaXmLElO79LXrW0qzpicydZCxdArKNmNRw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1)

