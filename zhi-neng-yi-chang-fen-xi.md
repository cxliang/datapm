# 如何搭建企业数据平台

## 0. 文章大纲

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaicibwlUhGqdwnLjgOmNBCET4NGxt5ialye0JgSydDnia3F9Ft9HkbP6KyVg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

## 1. 什么是企业数据平台产品

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaicPD3DkZ1zhFTB3odAV1jfib2kcIvJjgzIUCib8QV2ccpa59iagVwk21c6Q/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

个人定义「数据产品」为：数据产品是指利用数据辅助用户了解客观世界，做出决策甚至行动的一种产品形式。

首先从整体数据产品的分类讲起，划分的依据是使用者所属群体，分为 ToC，ToB 和企业内部三种，划分过程具体可见[在数据产品这个行业里，你需要知道这些内幕](http://mp.weixin.qq.com/s?__biz=MjM5NjcxMzIwMQ==&mid=2649861357&idx=1&sn=0a674a2b1d259da912c3ee8258768870&chksm=bee00b7389978265dd55eb8975cf18d0511e3b796ab1a488399028058a5f2a6b09a59fd52176&scene=21#wechat_redirect)。而在企业内部，又可细分为「业务型」和「平台型」。业务型的企业数据产品，更加专注于解决某个具体的业务问题或者部门问题，如客服数据监控系统和建立在集团平台的事业部决策分析系统。而平台型的目的，就是为前者提供更好的支撑。

在明确了宏观的定义后，我们再细拆下「企业数据平台」六个字。窃以为，重要性应按「数据」，「平台」和「企业」三个排列。

1. 数据，界定了产品的边界。我们思考的是怎么利用数据去优化业务，去推动业务，**数据组不产生数据，只是数据的搬运工，要和非常底层的业务逻辑保持适当距离。**对于日志的打印，业务库的设计等这些数据原料，我们可以根据经验提出更优的方案，但不适合去做具体的落地和执行。很多数据 PM 在一些业务需求的实现过程中会觉得非常低效和别扭，部分原因就是参与业务需求太深，导致在数据聚合层次掺杂了太多业务逻辑，业务方稍微更改下 PM 就会非常痛苦。

2. 平台，强调的是**面向各个业务提供服务，这要求产品具备较高的标准化和抽象化。** 标准化指的是主动出击，定下一些关键的数据资产规范，方便在企业中流通使用，如埋点管理，指标管理和数据库表管理等等。抽象化则指的是**不能只关注于解决一两个具体的需求点，而是关注整个面的抽象和满足，是一个由点及面的过程。**

3. 企业，在企业内部，会决定了反馈回路短，种类繁多，相对琐碎的需求特征。很多需求可能就是业务方走到你工位旁说一句话的事情。另外一方面，企业内用户层级价值明显，越到高层越能体现数据的价值，即以前我介绍过数据产品两大原则之一：「数据价值体现在数据使用者手中」。最后，市场竞争激烈，数据安全及权限也是头等大事。常见的权限模型为 RBAC（Role-Based Access Control，基于角色的访问控制\)。它抽象出「用户-角色-权限」三个概念，通过角色控制菜单权限，再为用户赋予相应角色。角色一般根据业务部门和领导层级综合划定。

## 2. 企业数据平台的目标

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2Xvaicx2CVFWPP2AhuD9LCJVjeo7lyCZjicHpnWKQt4Nf4vaPDvTZU5ibib0jUQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

借用 GrowingIO CEO Simon 的理念，企业如同人类建立的水资源使用系统，而数据如水。企业数据平台的建设目标，应当是让数据像水资源一样在企业中流动。这意味着数据要像水一样做到：

> 1. 干净无毒
>
> 2. 随用随取
>
> 3. 场景丰富

这恰好对应数据** 准确，全面，及时，易用**四个衡量维度。

进入人类资源使用系统的水资源需要经过一定的清洗和沉淀，确保「干净无毒」，然后根据不同的水用途存储，进入不同的管道，这对应于数据的「准确」。而「随用随取」对应着在人类社会中，拧开水龙头就能来水，及时，易用。「场景丰富」则意味着在不同场景里，水会有不同用途，饮用水，清洁用水，灌溉用水各取所需。即使饮用水，也分城市用水，矿泉水，纯净水等不同使用方式，通过挖掘和丰富数据的使用场景，深化数据本身的「全面」涵义。

达成这个目标的企业数据平台，便能通过**丰富场景，赋能业务**，提升整个企业使用数据的意愿和效率，赋予业务方高效使用和挖掘数据的能力。在使用场景上，个人归结为以下主要场景，其他还待继续补充：

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2Xvaicvp1ulI3zP8rzcgUcXicRogUPs4S8tZtHFWHMXQnkMiaicRib8lBCSfJwicw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

建立数据流程，从产品上，是帮助业务方更好地完成使用数据的流程，包括采集存储，展示分析到最后的挖掘落地三个层次。从需求上，即建立一个比较完善的需求分流解决机制，将零散需求，常规需求，业务需求等等分类处理完毕，并能将进展和结果及时反馈给需求方。优化用户体验，是通过掌握用户数据，为用户提供更加顺畅的使用体验，更加精准的营销等等。挖掘数据资产，包括标准化数据资产，以及不断挖掘回馈原有数据，丰富数据维度，即车老师在《决战大数据》中提到的「养数据」概念。

在转转的发展过程中，我们曾经利用各种数据猜测出用户的身份后进行定向业务推广，通过推广活动的反馈再回过头来修正用户身份，也是「挖掘数据资产」的一个例子。

## 3. 如何搭建企业数据平台

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaicxkePpfBJBhQPnk5O7ZS7jNk9Z3Kd2iciaI0fFK0TBHGOEPbe2XhoMcwg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

一个完善的平台应该由以上三个框架组成。其中技术框架非我所长，暂且略过。数据框架主要是在数据模型，安全及质量模块。其中，数据模型主要是先对所属业务出现出对应的领域模型，然后定下来对应的主题域划分和维度模型。产品框架上，依然遵循 What-Why-How 的划分方式，最先解决的是采集存储，「是什么」的问题，先把数据采集后清洗存储下来。其次解决「为什么」的问题，利用分析架构和数据可视化展示，帮助用户寻找原因。最后解决「怎么做」，通过价值的深入挖掘，和业务紧密结合等方式，来确定具体的内容和方向。

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaicoJZZ9yVmuNmuJusFmwy6xUSTICIpB5LWCtpic0OC8aAhTrdyalQvic4A/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

接下来简单介绍下产品框架中的每个步骤要解决的问题和对应的方案。

3.1 采集存储

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaiciaVYvQXKEeliaQtYHoUr4DxbmSrk2pa1cFrdRibueRlUBWxMSdUhL9EXg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

相应以上问题很多做数据的同学都遇到过，在此不一一赘述。元数据即数据的数据，意在管理企业的数据资产。实践的过程比较复杂，足以单独写一本书，这里挑一两个转转用得较多的功能给大家介绍下。数据字典，即存储和显示每个指标的定义，算法及对应的创建人及更新人，解决企业内指标定义不一致的问题。每次上线新指标就会定期更新该字典，确保内容及时性。数据血缘，即以数据表为点，以任务为线来显示表间关系，便于追踪数据来源和判断问题。数据地图，则是为了更方便寻找对应的数据表，每张表都有清晰的说明，注释及来源，仿佛一张地图帮你定位某个具体的「地点」和「路径」。此外，还有数据生命周期管理等等话题，在此就不一一展开。

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2Xvaic7C3hdUEXlFIZicdqLzUFbv4vXbpmMKv5FXFU3uFohicn12DNibSpmt1YQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaickK038JicqNxOg26EPBibBtpc9NxqwJtdY2xTBKicYCc97I4mg2opadSWA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

3.2 分析展示

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2Xvaick8PGvm8Fud0G00Fj0F4ODHJASGLlqItW3ibMtsJOp0xpH3TTq1GAA9g/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

需求分散主要体现在时间分散和空间分散。时间分散指的是可能今天提了一次，可能隔个十天半个月再次出现类似的需求。空间分散是指类似的需求可能由不同的部门提出来。需求量弹性大指的是如果没有一个合理的框架或思路去引导用户，可能会导致需求量变得非常庞杂。但有了引导之后，可能一个现有的工具就能满足了。需求实现也是一样的道理，用 A 和 B 方案可能都可以满足，但可能工作量会差别很大。因此根据不同层次的需求，我们通过三种递进的方案来解决。

1. 自定义分析：基本不需要数据和分析部门介入，提供工具就能满足也业务需求。面对这种需求，转转内部有三个解决方案。一是采用开源方案 HUE 搭建的 SQL 查询功能，解决非常零碎且无法产品化的临时需求。二是埋点的自动分析功能，只要按照数据规范进行的埋点，都可以在页面查询并分析数据。三是自定义报表分析界面，支持业务方导入数据表后进行可视化展示。这三种方案解决三种不同层次的需求，帮我们节省了大量人力。

2. 事件分析：需要数据部门一定程度的抽象。常见的就是留存/漏斗分析，这些需求特征是「套路明显」，有一定的培训成本，适用特定场景。

3. 多维交叉分析：需要数据部门根据业务进行规划和设计对应的分析体系，包含合理的维度和指标。一般来说这会是一个部门的基准需求，使用频次高，用于每天监控及分析业务异常原因。

在分析体系建立上，也可以参考我之前写的[数据分析的基本方法论](http://mp.weixin.qq.com/s?__biz=MjM5NjcxMzIwMQ==&mid=2649861486&idx=1&sn=e8c79ae936fc1f04fffed59f6be7e018&chksm=bee00af0899783e64566d7b921b904ba18e5846a3ade62fa48a8ac89d923a517105d6fbc09a0&scene=21#wechat_redirect)。

**3.3 挖掘落地**

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaicFBcx2l8MyyBT0HEDuZrnRNR2Qaw08IUXPRkk7na33d3Mr7cUbFAoCg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

挖掘落地一般着眼于数据和业务更紧密的结合，业务方能够在日常工作中直接使用。这里举我们的画像档案（天枢）和实时报警监测（獬豸）举例。

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaiccpX8emCexGAm6rzswx7axtCyz6dcVtXicbBeyvsfaibAibZJXhfEvh9og/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

画像档案，本质上是根据用户/商品/订单等客体的各种属性进行组合筛选，分析和运营。它汇集了整个转转各个业务产生的用户标签和用户行为数据。这些筛选出来的用户可以进行定向 push 消息推送和活动展示，甚至可以和 APP 的千人千面联系起来，定制某些标签的用户才能看到的入口。同时，该功能也方便了业务方导出具体的清单做分析，为数据组节省了大量人力。

![](https://mmbiz.qpic.cn/mmbiz_jpg/cVia3Ayib6tISNicTJXc1JSNQIS4UE2XvaicJoDRYUONdmzbO204OUcUKTK1K1QSDSVd8yhwKh56aeKAIUs1SzyPIw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)

实时报警预测，则是我们通过时间序列预测算法（Hot-Winters）兼异常维度分析算法（主要是改良版的基尼系数算法），实时监控核心数据。当发生异常时，便能将报警信息通过通讯工具发出来，以及自动分析出可能存在原因。比如某天订单异常升高，自动分析出来是手机品类异常升高导致的，直接询问手机品类的负责人，得知他们开展了一场活动。数据异常监测和定位变得非常迅速。

## 4. 后记

企业数据平台是个比较复杂的数据产品，而且随着公司体量上升复杂度会进一步提升。它的复杂一方面是承接了非常多的业务需求，如何抽象和管理就是一个问题。稍一不慎，不仅部门兄弟事倍功半疲于奔命，而且会产生大量无用的「报表尸体」，整个 BI 平台就变成数据的垃圾场，焚尸堆。第二方面是数据长期来看是个细活、脏活、累活。如何保证数据安全，质量，规范，需要不断地设计各种机制来监测和优化，这无疑又衍生了另外一套系统。最后，如果这个平台还希望能够和业务产生一些互动和助力，更得不断丰富场景，开发工具。但它作为企业管理和挖掘数据资产的抓手，在未来企业竞争中又会显得无比重要。长路漫漫，砥砺前行。

  


