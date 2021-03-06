# 4年估值20亿美元的大数据公司：Domo的神秘国度

> 研究国外业内前沿数据产品，了解当前实现数据价值的最新思路和实践。这是大数据产品漫游系列的第**1**篇文章。

# CEO：数据创业的领衔人物

![](josh-james-domo.jpg)

创始人 Josh James 在 1996 年创立风靡一时的网站统计产品 Omniture，后在 2009 年以 $18亿 的高价卖给了 Adobe。2011 年，他创立了现有的公司 Domo，4 年后估值已达 $20亿，并在今年三月份再次融资 $1.3亿。James 是数据领域创业的先驱，从 Domo 的产品理念上看，他在企业如何利用数据上已经洞察入微，驾轻就熟。

之所以称之为神秘，是因为在 2015 年宣布新一轮融资前，Domo 没有介绍过自己的功能特性，而且购买产品的客户必须签署保密协议，不得像第三方泄露 Domo 的产品信息，保密功能做得十分到位。即使到了今天，依然只能从一些介绍视频和博客上窥得一二。

# 产品：直击国外企业痛点

Domo 的核心功能是将公司内各种来源的数据汇总起来，提供给管理层及一线员工使用。一方面，国外企业倾向使用各种办公自动化的软件或服务，如人力资源管理用 Workday，销售管理用 Salesforce等，数据散落的情况十分普遍。另一方面，企业中因精细化运营的理念，经常需要用数据说话。 因此 Domo 的功能可谓直击客户痛点，解决了他们实实在在的需求。

DOMO 现在有 1000+ 个签约客户，包括 Master Card，国家地理，日产，及施乐等。据福布斯报告，Domo 按使用用户收费，年费最低为 2.5 万美元，按 12 人的最小规模团队计算，每用户约 2,000 美元。有些公司每年在其中投入 100 多万美元。即便如此高价，它的年复合增长率也超过了 100% 。

跑题一句，目前国内也有类似的产品出现。但因为国内数据运营的理念尚未普及，能提供数据接口的企业软件或服务也并不多见。这种情况将会严重限制此类产品的发展。只有在 SaaS 市场已经足够成熟的环境，才能诞生这样的独角兽。

# 功能：让数据更简单地被企业使用

Domo的功能分为五层，涵盖了数据整个链条。

> 1. Connect\(数据清洗\)：提供多数据源接入，实时更新（对 CEO 来讲十分重要）
> 2. Prepare（数据计算）：提供了现成的 ETL 工具，DataFusion调取数据，DataFlows 支持普通 SQL 语句来修改现有数据
> 3. Visualize（数据呈现）：提供拖拽式设计的Card Builder，再用Pages来组织Card，以及利用Domo APP默认生成图表；根据角色和行业提供对应方案
> 4. Engage（数据协作）：Domo Buzz可针对数据开展讨论，且只有和你相关的指标变动都会通知到你。Domo Profiles 提供个人在组织内的位置和行为。支持数据在组织内和组织外的分享。结论会形成任务，分派到人身上。
> 5. Optimize（数据驱动）：关心真正反映业务的指标。提供多样的分析工具（Analyzer）和提醒（Alert），Domo 平台提供洞见来驱动更好的结果。

这 5 个特点分拆到每个功能上，就是以下的流程图：

![](DraggedImage.png)

其中，多数据源的接入是 Domo 的基础，基于数据的协作则是 Domo 将数据落实为Action 的关键。只有当数据结论落实到人身上并且可追踪的时候，数据才能真正发挥价值。而提供各种分析 APP 的 AppStore 则真正让 Domo 具备成为新一代商业大平台的可能。它通过连接开发者与企业，来满足更多企业个性化的需求。

以上这些特性汇总成一句话，就是：**让数据更简单地被企业使用**。在以下详细介绍几个重点功能时，我们会发现，这种理念渗透在产品的每个细节里，令人叹为观止。

## 1. Connector：多数据源的接入

![](DraggedImage-1.png)

Domo 提供当前各种主流数据来源的接入库（Connector Library）。当接入完成后，会有现成的模板提供分析思路，避免重新做图分析。

可供接入的内容分为：

1. 广告后台，如 Google，Bing
2. 分析产品，如 GA，Adobe Analytics
3. 表格软件，如 Excel，Google Sheet
4. 数据库，如 MySQL 等
5. 提供接口的 SaaS 产品，如 New Relic，Salesforce，SurveyMonkey，Jira等APM，CRM，调查类，协同类产品
6. 社交产品，如 Twitter

接入后的内容会有专门针对此类的内容的模板生成。这也印证了 Domo 让数据变得更简单的产品理念，帮客户自动完成了作图这个繁琐的过程，直接将一盘美味佳肴端到你的面前。以下是产品截图

![](DraggedImage-2.png)

## 2. Magic：多数据源的融合

以 “Magic” 命名这个功能，可以想见 Domo 对这个功能的喜爱。这是 Domo 产品逻辑的底层基础，包含了三个功能，为 ETL，DataFlows 和 DataFusion。旨在提供极其简单易懂的工具，将不同来源的各种数据以可视化的方法整合到一起。如图所示，将两个产品的某一列内容作为主键关联起来。

![](DraggedImage-3.png)

### 2.1 ETL

以可视化的方法，让小白用户也可以进行数据清洗，转换和加载的高级工作，连 SQL 都不用写了。

![](DraggedImage-4.png)

### 2.2 DataFlows

这是 Domo 为高端用户们贴心提供的 SQL 查询工具，满足更多自助化的提数和

### 2.3 DataFusion

甚至你可以直接在数据源中进行增删合并，生成新的内容。

![](DraggedImage-5.png)

ETL 在很多大公司里，都会有专门的数据工程师负责。而 Domo 竟然用这么一款简单的产品，节省了这些工程师们大部分的工作量。当然，完全取代是不可能的，毕竟存在效率问题和更深层次的聚合表和主题表的创建过程。不过能够做到这一点，已经大大降低了很多数据的使用门槛。

## Card & Analyzer：数据可视化和分析

Card Builder 属于制图部分，而 Analyzer 是针对已做单图的分析。

### 3.1 多样的数据可视化

在可视化数据部分，支持拖拽方式建立单图，并且提供了超过 50+ 图标样式。**一个值得注意的细节是，添加数据源后会提供默认单图，而非一片空白**。在创建完图标后，会以一种固定的格式罗列在页面上，便于用户查看和整理。

![](DraggedImage-6.png)

### 3.2 针对行业的呈现模式

在 Domo 的菜单里，可以看到顶栏按照各职业做了区分。其实 Domo 在产品设计上，会根据不同行业，不同角色和不同数据来源提供默认 Card。在通用性数据平台解决深入性业务问题的这个方向上，迈出了重要一步。

### 3.3 分析功能

Analyzer 提供了过滤，下钻，提醒和变更图标形式等方式进行分析的方法。下钻可以层层下探到数据源，帮助用户了解各种颗粒度上的问题。

![](DraggedImage-7.png)

## Buzz && Task

![](DraggedImage-8.png)

Buzz 和 Task 这两个功能解决了**数据结论无人落实，无法追踪的问题，完成了一个管理闭环**。使用的场景十分明确，客户先通过 Buzz 对当前某些报表进行讨论，形成结论后再通过 Task 分配到个人身上，时刻可以追踪。这样的设计，实际是扩展了当前 BI 的内涵，从对数据的分析升华到了对数据的使用上，进一步发挥了数据的价值。从这点上来讲，已经比所谓大数据产品不知道高到哪里去了。

![](DraggedImage-9.png)

同时还有移动端的产品，让这种讨论可以更简单地在各种场景里进行。不过，一线员工们可能要多受点难了...

## AppStore

![](DraggedImage-10.png)

**Domo 的 AppStore 让它有成为一个大平台的可能**。首先它满足了更多贴近业务的分析场景。AppStore 里提供了各种行业，职位，部门，活动等方面的数据应用，让数据的使用和分析变得更为简单。其次也支持了更多的信息源，完成了更全面的数据来源覆盖。以一个面向销售的，针对线索参与度分析的分析 APP 为例：

![](DraggedImage-11.png)

类似的分析 APP 还有很多。2016 年的 Domopalooza 大会又发布了一个耗资 5 亿美元，面向移动端的应用商店，致力于打造全球第一个“商务云”的概念。它宣称在其新的 APP 商店中已经拥有 1000 家合作商。借此，Domo 铁蹄铮铮，正一步步地拓宽自己的商业版图。

> ”We didn't make the next great flip phone, we just dropped the iPhone," - Josh James

# 后记：纸上得来终觉浅

本文中所有的产品信息均来自于演示视频和官方博客，难免失之偏颇。若读者中有使用 Domo 的经验或者有更深入了解的同学，欢迎斧正，不甚感激。

硬币皆有两面。相比于同类竞品，如 GoodData，BIME 等，Domo 的缺点也很明显：价格昂贵。这点让诸多 SMB 们望而却步。这种定价策略见仁见智。不过无论是出于成本还是战略定位的考虑，产品本身的优秀都不可抹杀。Quora 上有个问题十分有趣，大家可做延伸阅读：

最后奉上一个移动端的产品 Gif 图，让大家从一个侧面感受下他们的产品。

> "Of course we were thinking big," James says. "Of course we want to change the world!" — Josh James6

![](DraggedImage-12.png)

