# Meta Learnings: GTD and PKM

最近看了两个文章，一个是 ThoughtWorks 洞见上的[没有了老师，你该如何学习？](http://insights.thoughtworkers.org/how-to-study-without-teacher/)，它提到了四个点，把我散乱的困惑全串起来了：

* 学什么：注重底层原理和高层解决方案的学习，因为它们相对稳定，变动不大；中层变动频繁的知识，项目用什么学什么
* 怎么学：快速反馈、实践、反馈
* 如何执行：GTD：收集、分类、计划、执行、反馈总结
* 广度：PKM

这解决了我一个长期的困惑，明白了要学习什么，定出了一个短期的目标，终于决定准备好了可以找熊节来聊 sponsor 的事情。目标制定出来了，也落实到长期、中期和短期的计划了，怎么解决执行的问题呢？总结了一下，原则十分简单：

* 2分钟内能做完的事马上做
* 1天内能做完的事记录下来，当天完成
* 短期目标，细化到 calendar 中，制定成 task 加以跟踪，使用番茄工作法辅助执行
* 中期目标，利用“21天习惯”原理，细化成每天重复任务，分解成短期任务加以实现
* 长期目标，使用“愿望清单”法进行管理，进一步拆分成中期和短期目标加以跟踪和执行

## PKM：高效的知识管理

PKM 是较早解决的一个问题，它主要目标是利用有限的时间，以尽可能低的成本筛选出价值高的信息并转化成知识，以达到高效学习的目的。这里价值如何算高，因人和时期而异，但如何以尽可能低的成本，在互联网茫茫的信息之网中筛选出高价值的信息，并转化成知识呢？

### 筛选

筛选信息有一个过程，它基本与 GTD 遵循一个类似的过程，即搜集、归类、计划的过程。首先我们希望有一个集中的地点获取所有的信息，并实现对它们的自动归类（通过 label/tag 系统）；其次通过每天小量固定时间的粗阅读，快速进一步筛出自己觉得“有价值”的信息，转存到另一个地点；最后是细阅读的阶段。综上，这两个阶段，我们分别是通过两个工具来辅助实现：

* 信息搜集：Feedly/Reeder/Gmail/Wechat Official/Youtube/Twitter/Weibo（Reeder后面所有渠道应该整合）
* 细阅读：Instapaper/Pocket

### 信息 -> 知识

最后进入到细阅读阶段的知识，有更大的可能是对自己有益的信息。那么，如何将这些信息尽可能多地转化成成体系的知识呢？这里就不得不提到吕立青的一个点：标注胜于收藏。高效学习的方法，永远是**带着问题阅读**、**实践与快速反馈**、**整理成体系**，而不是一键收藏然后再也不会打开这个书签或者网页。基于此主动阅读标注的学习方法，我们同时也需要一个工具来进行标注、归类、整理体系化的知识。综上，目前我用到的工具有两个：

* diigo，用于标注，其 outliner 完美结合了带着问题阅读 -> 整理成体系这样的学习路径
* evernote，用于归档部分技术知识，仅用于存档

diigo 和 evernote 还能将资料库中相关的内容显示在 Google 搜索的侧边栏，从而让你优先浏览已经阅读、归档、整理过的知识，使知识的学习和流通成为闭环。

![](diigo-evernote-right-hand-side.png)

## GTD：计划与执行的分离

目标和规划有了，PKM 也有了，可以说，[这篇文章](http://www.mifengtd.cn/articles/runningcheese-gtd-system.html)则解决了剩下的唯一一个问题：如何分类任务并执行。前面提到，GTD 的几个核心的步骤为：

* 搜集。工具方面，需要一个可以快速记录、随手可及、可以设定日期、可以可视化任务完成与否、与 calendar 集成的 todo 工具，我用的是[ticktick](https://ticktick.com/)
* 分类、计划。四象限原则、时间资源进行任务裁剪
* 执行。工具方面，需要一个可以将细化后的 task 自动化监督执行的工具，我用的是[pomotodo](https://pomotodo.com/app/)
* 反馈总结。retrospective

总结下来，当已经确定下一个中短期的目标，并且已经将其按四象限原则、时间资源等成本综合考虑进行了裁剪后，要将它们 **细化成 task** 并 **自动化执行** 的步骤为：

1. 将细化后的 task 固定到每天的时段去，并且保证 ticktick 与 calendar 端的**实时**集成
2. pomotodo 实时拉取 calendar 上的任务，并**自动化**地根据时段设定的任务启动 pomo

## 痛点

1. [GTD] ticktick/calendar/pomotodo 的自动化系统(现在觉得是个伪需求，不需要自动开始 pomo 周期，而且也是无益的。人自身有情绪周期)。
2. [GTD] Pomotodo 还只能单向推送到 Gmail，无法订阅 Gmail，也就无法自动根据 calendar 上的 task 安排执行 pomos
3. [GTD] 没有中长期目标的可视化支持。我希望它能在 ticktick 上体现出来：我中长期要做这个事，在短期上体现为哪个时间安排哪个计划。目前短期任务是零散的，而 workaround 也只能是我在这个 README 写下长期目标，通过 Github issue/project 管理我的中期目标。手动的方式既不灵活，也容易遗漏
4. [GTD] Pomotodo Mac版慢成💩了。其实只需要一个 start pomo/break 的功能，附带时间归类分析功能，必须找 alternatives。(目前，使用了它的网页版。虽限制但能用。)
5. [PKM] 中心化订阅：微信公众号、微博动态、twitter 动态、youtube 待看视频等都希望能订阅成 RSS 到 Reeder 中
6. [PKM] IFTTT 上的 evernote channel 没有开放保存全文的 API，一些 memo 类的文章无法从 Instapaper/Evernote 归档到 evernote，只能手动使用 Evernote Web Clipper 插件
7. [PKM] Troubleshooting 类资源：多来自 stackoverflow，我想保存待以后取用。但不想保存到 diigo 污染标注型的知识体系，保存到 evernote 又无法标注。应有专门的工具来做这个事
8. [PKM] 我现在也不止学技术了，有其他的资源，要怎么整理呢？也用 diigo 吗？会不会污染技术空间？用 evernote 那没有 markdown 的环境想想都口怕
9. [GTD&PKM] 忘了

## 2016.11 - 2017.7 计划

项目地址：[https://github.com/linesh-simplicity/meta-learnings/projects/3?fullscreen=true](https://github.com/linesh-simplicity/meta-learnings/projects/3?fullscreen=true)

关于具体的方向，大熊说年轻可以不用纠结，心就定了一些。那么中期的目标，则在邱俊涛的[这篇文章](http://icodeit.org/2015/06/do-we-really-short-for-front-end-developer/)中得到了解答：作为 developer，你要对开发以外的上下游，即整个软件工程的流程都涉足，如此才能更系统地思考和解决问题。[这篇文章](http://insights.thoughtworkers.org/how-to-study-without-teacher/)则指出，首要学习底层和高层等稳定的知识，中层的项目用啥学啥。综上，得出我需要去了解**开发的上游和下游**。

但这个计划出来半个月后，我意识到这还是为了计划而计划，根本不 make sense。细思下来，当下最重要的是培养强大的技术统治力，什么上下游都还不触及核心。我认为当前最重要的，是后端 Java 的 TDD，以及前端 JavaScript 和 React。这是在一个构建企业级应用的上下文中来讲的。因此，调整计划：

### Top Priority

* [ ] React
* [ ] JavaScript/ES6
* [ ] TDD
* [ ] 重构&设计模式

### Upstream

* [ ] 需求来源与分析
* [ ] 用户体验（HTML/CSS/UI Design）
* [ ] 保险业务了解

### Downstream

* [ ] 持续集成
  * [ ] git 
  * [ ] github/stash
  * [ ] jira/trello
  * [ ] Jenkins/Travis
* [ ] 持续部署
  * [ ] API：Axway
  * [ ] 负载均衡：F5/nginx
  * [ ] 安全验证：OAuth/2FA
  * [ ] 部署：AWS/S3/Cloud
  
以上主要不是了解技术多么深的细节，而是了解技术在流程中的作用。

### Kore Developer Skills

* [ ] 项目需求
* [ ] Backend
  * [ ] 经典的MVC：Spring MVC
  * [ ] API：REST
  * [ ] 测试体系与策略
* [ ] Core
  * [ ] Shell
* [ ] Elegant MAC
* [ ] Creativity: Painpoint resolving
* [ ] 英语

## Thoughts

出于某些不可描述的原因，这个板被我当成了重要想法的登记来源。最近在想法上，有为数不多但是值得好好吸收的输入：

**Real control is surgical 大道无形**

这个想法来源有很多，对我影响最大的恐怕还是两台人工智能了：Samaritan/AlphaGo。有时候，人由于固有计算能力和思维能力的局限，无法排除一些固有思维的禁锢。这是作为人这个物种的局限，但可以意识并克服一些。主要是，人作为个体的情感、风格不可避免并且非常美丽，但是要注重从事物和时间的**广度**上来**深入**地思考一些事。李世石败战后也感慨，不可以靠感觉，要靠计算。

对了，我也是一名棋手。

**使用付费的服务**

领域里真正专业的人才、服务能大幅地提高你的学习速度、学习效率，从而让你更有钱去购买其他更好的服务，从而变得更好。这是我正在学习的思维方式，手上的金钱、资源要从投资的角度来更好地使用它。

**思维与真心**

真相是知道了会有感应的东西，不要害怕，不要思维。
