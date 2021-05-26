# 🏛 关于我们 @ 淘宝架构与基础服务团队

最重要与广泛的业务场景，位于阿里最有价值最大的业务 淘宝，并支撑整个集团。为淘系、整个集团提供基础核心能力、产品与解决方案：

- 面向业务价值的精细化流量管控解决方案
- 自适应业务高可用的解决方案与核心能力（为业务提供的限流、隔离与熔断的柔性高可用解决方案）
- 下一代网络协议`QUIC`实现与落地
- 新一代的业务研发模式`Gaia`平台（一站式函数研发`FaaS`平台）
- 支撑着整个阿里集团的移动中间件体系：
    - 流量套件：`API`网关`MTop`、接入层`AServer`、`APP`流量调度/切流
    - 移动文件上传服务（支撑内容化业务）
    - 推送/消息、移动配置中心

## ✨ 团队产品的介绍

1. **面向业务价值的精细化流量管控**的平台解决方案
    - 2021上海 ArchSummit全球架构师峰会 分享 —— 面向业务价值的端到端全链路自适应流控实践 2021-04-25
        - [大会议题的介绍页](https://archsummit.infoq.cn/2021/shanghai/presentation/3321)，有PPT的`PDF`文件
    - [淘系面向业务价值的精细化流量管控实战](https://mp.weixin.qq.com/s/P3R2E44mjTrj7HnMAh-TyQ) - 淘系技术公众号 2020-11-23
        - 随着淘系业务系统演进，沉淀了大量公共能力的业务平台（即平台型应用），如直播、权益、大促会场、互动、聊天消息、导购（招选搭投）、首页等等，支撑其上的众多的业务场景或流量来源方（如不同App、投放），形成了 横向平台+垂直业务的架构模式。各个业务平台会需要支撑大型的业务流量（峰值会数十万QPS甚至百万QPS）。
        - 业务平台模式解决了诸多难题，比如解决了业务能力重复建设引起的交付效率低的问题，便于沉淀且利于创新；面向终端用户提供一致的体验等等。同时也带来了新的问题/诉求：
            - 面向业务价值的精细化业务流量管控（如限流/服务分级/隔离）
            - 业务平台自建网关的系统稳定性与成本问题
            - 突发大流量的稳定性保障
1. **业务高可用的解决方案与自适应核心能力**（为业务提供自适应的限流、隔离与熔断的柔性高可用解决方案）
    - 2021上海 ArchSummit全球架构师峰会 分享 —— 阿里千万级 QPS API 网关的演进之路 2021-04-25
        - [大会议题的介绍页](https://archsummit.infoq.cn/2021/shanghai/presentation/3344)，有PPT的`PDF`文件
    - [阿里亿级长连网关的云原生演进之路](https://mp.weixin.qq.com/s/hTUaswESTBMbeqyIZQlBSw) - 淘系技术公众号 2020-11-24
        - AServer接入网关承载整个阿里集团的入口流量，负责亿级用户的长链保活，支持上万路由策略转发，是连接上亿用户与后端几十万服务节点的桥梁，在今年双十一需要支撑亿级在线用户、千万级QPS、生效上万条API管控策略，做到了安全可靠的转发路由，并保障了用户体验如丝般顺滑。在大规模业务流量与管控支撑的背后，需要对系统每一个细节的精确把控，消除每一个潜在的风险点。
        - 借助云原生架构可以极大地简化运维操作，降低了潜在的风险，今年双十一阿里AServer接入网关上千台规模的Pod平稳扛过峰值。本文主要介绍阿里AServer接入网关如何从上一代架构拥抱变化，全面云原生的演进之路。
    - [淘宝业务 稳定性保障实战——诺亚(Noah)自适应流控](https://mp.weixin.qq.com/s/eHtc5qKmIbi3hsb0jqr5TQ) - 淘系技术公众号 2020-05-21
    - [实力为2019年双11而战！稳！ — 自适应限流技术](https://mp.weixin.qq.com/s/q3kSWp5DTgo6i6vp3p9MuQ) - 淘系技术公众号 2019-11-12
    - [淘宝 如何保障业务稳定性——诺亚(Noah)自适应流控](https://mp.weixin.qq.com/s/ePWqUiZcEy52mUHb4WbcSA) - 淘系技术公众号 2019-11-27
    - [淘宝 应用柔性架构的探索](https://mp.weixin.qq.com/s/uW8gNGCI-oj4NitU9dHZjQ) - 淘系技术公众号 2019-08-12
    - 2019北京 TOP100全球软件案例研究峰会 分享：面向流量的自适应高可用架构 —— 淘宝应用架构升级实践 2019-11-16
        - [PPT的`PDF`文件](https://github.com/oldratlee/reactive-practice-at-taobao/blob/master/%E9%9D%A2%E5%90%91%E6%B5%81%E9%87%8F%E7%9A%84%E8%87%AA%E9%80%82%E5%BA%94%E9%AB%98%E5%8F%AF%E7%94%A8%E6%9E%B6%E6%9E%84-%E6%B7%98%E5%AE%9D%E5%BA%94%E7%94%A8%E6%9E%B6%E6%9E%84%E5%8D%87%E7%BA%A7%E5%AE%9E%E8%B7%B5-%E6%9D%8E%E9%BC%8E-20191116-Top100.pdf)，[大会议题的介绍页](https://www.top100summit.com/detail?id=14331)
        - 分享过去一年多的思考、实现 与 2019双11实践落地及其收益效果。
        - 高可用(HA) 不单是 **应对资源失效的高可用**，还有 **面向流量的高可用**。在今天对于应用架构来说，后者更是痛点，但业界的关注、思路、实践要落后很多。让我们一起更多地关注、正面思考与解决这只房间里的大象：流量不确定性带来的稳定性问题！
1. **下一代网络协议`QUIC`实现与落地**
    - [The Road to `multipath QUIC`: 阿里自研多路径传输技术`XLINK`](https://mp.weixin.qq.com/s?__biz=MzAxNDEwNjk5OQ==&mid=502945646&idx=1&sn=009a04fa4d36caf8493c58c7e9dc7ef1&chksm=03969f7634e11660fc6e7feb63cbdb3cd8054e4bf58506489a73790ecf7b3db8b0e91089d741#rd) - 淘系公众号 2021-05-11
        - 阿里巴巴淘系技术部淘系架构团队与达摩院XG实验室共同研发的`XLINK`多路传输技术，相关论文「XLINK: QoE-driven multi-path QUIC transport in large-scale video services」已经被顶级学术会议`SIGCOMM 2021`正式接收， 这也是`SIGCOMM`会议历史上第一篇关于多路径`QUIC`的论文。
    - [面向`5G`的阿里自研标准化协议库`XQUIC`](https://mp.weixin.qq.com/s/CbdlTq1xb2N1WSnmGfmEQQ) - 淘系公众号 2020-8-11
      - `XQUIC`是阿里巴巴淘系架构团队自研的`IETF QUIC`标准化协议库实现，在手机淘宝上进行了广泛的应用，并在多个不同类型的业务场景下取得明显的效果提升，为手机淘宝APP的用户带来丝般顺滑的网络体验：
        - 在`RPC`请求场景，网络耗时降低 15%
        - 在直播高峰期场景，卡顿率降低 30%、秒开率提升 2%
        - 在短视频场景，卡顿率降低 20%
    - [阿里`XQUIC`：标准`QUIC`实现自研之路](https://mp.weixin.qq.com/s/pBv_DnG05YWl4ZYRHThaTw) - LiveVideoStack 2020-8-12
    - [阿里淘系自研标准化协议库`XQUIC`首次公开：直播高峰期卡顿可降低 30%](https://mp.weixin.qq.com/s/-nOEzOwGcckptjkxozw1mw) - InfoQ 2020-8-15
1. **淘宝`Reactive`架构升级**
    - [全面异步化：淘宝反应式架构升级探索](https://mp.weixin.qq.com/s/MLqBhgUCkEX1ARPmZPHChQ) - 淘系技术公众号 2019-01-15
    - [与十俱进 2018双11狂欢看淘宝技术创新力 — 技术架构全面革新](https://mp.weixin.qq.com/s/Ks-p67BoddNQB74yMz7YpQ) - 淘系技术公众号 2018-11-12
    - QCon2018北京 分享：Reactive架构升级实践 —— 淘宝全站业务的全异步流式架构升级 2018-4-21
        - [PPT的`PDF`文件](https://github.com/oldratlee/reactive-practice-at-taobao/blob/master/Reactive%E6%9E%B6%E6%9E%84%E5%8D%87%E7%BA%A7%E5%AE%9E%E8%B7%B5-%E6%9D%8E%E9%BC%8E-20180421-QCon%E5%8C%97%E4%BA%AC.pdf)，[大会议题的介绍页](https://2018.qconbeijing.com/presentation/462)
    - 更多说明详见 [这里](https://github.com/oldratlee/reactive-practice-at-taobao)
1. **新一代的业务研发模式`Gaia`平台**（一站式函数研发`FaaS`平台）
    - [阿里业务研发平台的新利器——GAIA横空出世](https://mp.weixin.qq.com/s/mD0URwb3tV1MZ14GYJ1zrQ) - 淘系技术公众号 2019-07-02
    - [“一次编码、到处运行”，淘宝云端一体化探索](https://mp.weixin.qq.com/s/NSWhgJ132qbaCudIsJt7xw) - 淘系技术公众号 2019-08-22
    - [PPT分享|闲鱼Flutter+GAIA(Serverless)一体化研发](https://mp.weixin.qq.com/s/RjlMp22mlZRnPGoFvMhsgQ) - 淘系技术公众号 2020-3-26
    - [Swift 在 GAIA 平台云端一体化的探索](https://mp.weixin.qq.com/s/7B2FDBZ_vnvswiYWjLih4Q) - 淘系技术公众号 2019-11-15
