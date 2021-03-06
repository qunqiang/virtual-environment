# 介绍

KtVirtualEnvironment是一种基于ServiceMesh的微服务环境复用工具，源于阿里内部的“项目环境”实践。

通过识别Pod上的虚拟环境标签，KtVirtualEnvironment能够自动将测试环境网络动态隔离成多个虚拟隔离域，同时以简单规则在隔离域间局部复用Pod实例，从而达到只需很少资源成本即可创建大量不同微服务版本组合的独立测试环境的目的。

阅读[这里](https://yq.aliyun.com/articles/700766)了解更多故事。

![isolation](https://virtual-environment.oss-cn-zhangjiakou.aliyuncs.com/image/diagram-zh-cn.jpg)

在[原理与概念](zh-cn/ve/concept.md)小节将对这种路由规则进行更详细的介绍。

## 特性

- 基于环境标记划分虚拟隔离域
- 隔离域之间复用大部分公共环境服务实例
- 用户随意在隔离环境中部署、调试服务而不会影响其他开发者
- 本地运行服务无需部署到集群，直接加入任意隔离域

## 联系我们

请加入`kt-dev`钉钉群：

<img src="https://virtual-environment.oss-cn-zhangjiakou.aliyuncs.com/image/dingtalk-group-zh-cn.jpg" width="40%"></img>
