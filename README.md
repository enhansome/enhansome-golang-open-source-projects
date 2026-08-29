# Awesome Golang Open Source Projects with stars

面向中文读者重新整理的 Go 开源项目目录。新版目录不再追求“尽可能全”，而是优先保留仍在维护、社区认知清晰、适合学习和选型的项目，并补充了 AI Agent 相关项目。

当前版本收录 **77** 个项目，分成 **10** 个主题；最近一次维护状态审阅时间为 **2026-03-06**。

* [English version](README_EN.md)
* [分类与维护策略](docs/分类与维护策略.md)
* [移除与迁移记录](docs/移除与迁移记录.md)

## 这次整理做了什么

* 把旧的 17 个松散分类重组为 10 个主题，去掉了难维护的“其它”分类。
* 清理了已归档、仓库已废弃、长期停更且已有明确替代方案的项目。
* 去掉了重复收录，同一个项目只保留一个最合适的入口分类。
* 新增 AI / Agent 分类，覆盖 LLM 应用框架、MCP、推理运行时和向量检索。

## 收录原则

* 优先保留截至 2026-03-06 仍可确认处于维护状态的项目。
* 已归档、仓库消失或长期停更且已有更好替代的项目默认移除。
* 目录强调学习与工程选型价值，不再为了覆盖面保留大量边缘项目。
* 每个项目只收录一次，避免在多个分类中重复出现。

## 分类导航

| 分类         | 关注点                     | 项目数 |
| ---------- | ----------------------- | --- |
| AI / Agent | LLM 应用框架、MCP、模型运行时与向量能力 | 8   |
| 云原生与容器     | 容器运行时、编排、镜像仓库和集群平台      | 8   |
| 服务治理与平台工程  | PaaS、服务治理、CI/CD、消息与异步任务 | 12  |
| 数据存储与搜索    | 数据库、分布式存储、检索与数据访问生态     | 10  |
| 可观测性       | 指标、图表、告警与运行状态检查         | 6   |
| 网络与安全      | 网关、负载均衡、代理、流量调试与网络工具    | 6   |
| Web 开发与应用  | Web 框架、服务端组件与实时交互能力     | 11  |
| 数据处理与机器学习  | ML、NLP、爬虫与数据处理          | 6   |
| 开发者工具与基础库  | 开发效率、测试、终端 UI 和核心基础库    | 8   |
| 区块链        | 仍在维护、影响力最大的 Go 区块链项目    | 2   |

## AI / Agent

LLM 应用框架、MCP、模型运行时与向量能力

| 项目                                                                                                     | 简介                                                |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------- |
| [ollama/ollama](https://github.com/ollama/ollama) ⭐ 179,674 \| 🐛 3,828 \| 🌐 Go \| 📅 2026-08-29      | 本地运行、分发和管理大模型的 Go 运行时。                            |
| [tmc/langchaingo](https://github.com/tmc/langchaingo) ⭐ 9,645 \| 🐛 411 \| 🌐 Go \| 📅 2026-01-11      | Go 版 LLM 应用框架，覆盖 prompt、tool calling、agent 和 RAG。 |
| [cloudwego/eino](https://github.com/cloudwego/eino) ⭐ 12,864 \| 🐛 148 \| 🌐 Go \| 📅 2026-08-28       | CloudWeGo 出品的 Go AI 应用框架，强调组件化编排和生产落地。            |
| [mark3labs/mcp-go](https://github.com/mark3labs/mcp-go) ⭐ 9,036 \| 🐛 42 \| 🌐 Go \| 📅 2026-08-12     | 用 Go 构建 MCP client 和 server 的实用 SDK。              |
| [mudler/LocalAI](https://github.com/mudler/LocalAI) ⭐ 48,727 \| 🐛 222 \| 🌐 Go \| 📅 2026-08-28       | OpenAI 兼容的本地推理服务，适合私有化部署。                         |
| [mudler/LocalAGI](https://github.com/mudler/LocalAGI) ⭐ 1,963 \| 🐛 86 \| 🌐 Go \| 📅 2026-08-25       | 面向本地模型的 Agent 平台，强调工具调用和自治流程。                     |
| [weaviate/weaviate](https://github.com/weaviate/weaviate) ⭐ 16,759 \| 🐛 691 \| 🌐 Go \| 📅 2026-08-29 | Go 编写的向量数据库，可用于 RAG、检索和 Agent memory。             |
| [pardnchiu/Agenvoy](https://github.com/pardnchiu/Agenvoy) ⭐ 474 \| 🐛 0 \| 🌐 Go \| 📅 2026-08-28      | Go 编写的 Agent 平台，提供 Py/Js 工具接口、错误记忆与自动修正能力。        |

## 云原生与容器

容器运行时、编排、镜像仓库和集群平台

| 项目                                                                                                                         | 简介                                 |
| -------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| [moby/moby](https://github.com/moby/moby) ⭐ 72,011 \| 🐛 3,892 \| 🌐 Go \| 📅 2026-08-28                                   | Docker 引擎的上游项目，也是学习容器运行时实现的核心入口。   |
| [kubernetes/kubernetes](https://github.com/kubernetes/kubernetes) ⭐ 125,327 \| 🐛 2,978 \| 🌐 Go \| 📅 2026-08-28          | 事实标准级的容器编排平台。                      |
| [goharbor/harbor](https://github.com/goharbor/harbor) ⭐ 29,253 \| 🐛 869 \| 🌐 Go \| 📅 2026-08-28                         | 企业级 OCI 镜像仓库，带权限、审计和复制能力。          |
| [rancher/rancher](https://github.com/rancher/rancher) ⭐ 25,878 \| 🐛 3,341 \| 🌐 Go \| 📅 2026-08-28                       | 面向多集群场景的 Kubernetes 管理平台。          |
| [quay/clair](https://github.com/quay/clair) ⭐ 11,053 \| 🐛 59 \| 🌐 Go \| 📅 2026-08-25                                    | 容器镜像漏洞分析与扫描服务。                     |
| [moby/swarmkit](https://github.com/moby/swarmkit) ⭐ 3,647 \| 🐛 276 \| 🌐 Go \| 📅 2026-08-28                              | Docker Swarm 的核心编排组件，适合学习调度和集群编排。  |
| [AliyunContainerService/pouch](https://github.com/AliyunContainerService/pouch) ⭐ 4,644 \| 🐛 10 \| 🌐 Go \| 📅 2024-08-22 | 阿里开源的容器引擎项目，聚焦更强的隔离与稳定性。           |
| [hashicorp/nomad](https://github.com/hashicorp/nomad) ⭐ 16,841 \| 🐛 1,638 \| 🌐 Go \| 📅 2026-08-28                       | 轻量级工作负载编排器，适合对比 Kubernetes 的另一条路线。 |

## 服务治理与平台工程

PaaS、服务治理、CI/CD、消息与异步任务

| 项目                                                                                                                 | 简介                                       |
| ------------------------------------------------------------------------------------------------------------------ | ---------------------------------------- |
| [tsuru/tsuru](https://github.com/tsuru/tsuru) ⭐ 5,307 \| 🐛 18 \| 🌐 Go \| 📅 2026-08-25                           | 成熟的开源 PaaS，适合学习应用平台抽象。                   |
| [goodrain/rainbond](https://github.com/goodrain/rainbond) ⭐ 6,255 \| 🐛 55 \| 🌐 Go \| 📅 2026-08-28               | 以应用为中心的云原生平台，覆盖交付、运维和微服务治理。              |
| [harness/harness](https://github.com/harness/harness) ⭐ 38,157 \| 🐛 103 \| 🌐 Go \| 📅 2026-08-28                 | Drone 已并入 Harness 生态后，新的 CI/CD 与开发者平台入口。 |
| [gravitational/teleport](https://github.com/gravitational/teleport) ⭐ 20,857 \| 🐛 3,331 \| 🌐 Go \| 📅 2026-08-28 | 基于零信任模型的远程访问与基础设施入口。                     |
| [istio/istio](https://github.com/istio/istio) ⭐ 38,365 \| 🐛 515 \| 🌐 Go \| 📅 2026-08-28                         | 服务网格代表项目，覆盖流量治理、安全和可观测性。                 |
| [uber/jaeger](https://github.com/uber/jaeger) ⭐ 11 \| 🐛 0 \| 📅 2023-07-06                                        | 分布式追踪系统，适合与 OpenTelemetry 一起理解链路追踪。      |
| [go-kit/kit](https://github.com/go-kit/kit) ⭐ 27,422 \| 🐛 60 \| 🌐 Go \| 📅 2024-07-19                            | Go 微服务开发工具箱，强调可观测性和可测试性。                 |
| [goadesign/goa](https://github.com/goadesign/goa) ⭐ 6,091 \| 🐛 43 \| 🌐 Go \| 📅 2026-08-29                       | 设计优先的 Go 服务开发框架。                         |
| [TykTechnologies/tyk](https://github.com/TykTechnologies/tyk) ⭐ 10,810 \| 🐛 498 \| 🌐 Go \| 📅 2026-08-28         | 成熟的开源 API Gateway。                       |
| [micro/go-micro](https://github.com/micro/go-micro) ⭐ 23,047 \| 🐛 8 \| 🌐 Go \| 📅 2026-08-28                     | Go 微服务框架，适合研究服务抽象与插件化扩展。                 |
| [nsqio/nsq](https://github.com/nsqio/nsq) ⭐ 25,775 \| 🐛 77 \| 🌐 Go \| 📅 2026-08-11                              | 经典的实时分布式消息平台。                            |
| [RichardKnop/machinery](https://github.com/RichardKnop/machinery) ⭐ 7,972 \| 🐛 248 \| 🌐 Go \| 📅 2025-11-15      | Go 异步任务队列，适合替代 Celery 的思路参考。             |

## 数据存储与搜索

数据库、分布式存储、检索与数据访问生态

| 项目                                                                                                               | 简介                                   |
| ---------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| [cockroachdb/cockroach](https://github.com/cockroachdb/cockroach) ⭐ 32,429 \| 🐛 8,418 \| 🌐 Go \| 📅 2026-08-26 | 分布式 SQL 数据库，强调强一致与弹性扩展。              |
| [vitessio/vitess](https://github.com/vitessio/vitess) ⭐ 21,271 \| 🐛 1,092 \| 🌐 Go \| 📅 2026-08-29             | YouTube 开源的 MySQL 水平扩展方案。            |
| [pingcap/tidb](https://github.com/pingcap/tidb) ⭐ 40,478 \| 🐛 6,833 \| 🌐 Go \| 📅 2026-08-29                   | 兼容 MySQL 协议的分布式 HTAP 数据库。            |
| [influxdata/influxdb](https://github.com/influxdata/influxdb) ⭐ 31,726 \| 🐛 2,157 \| 🌐 Rust \| 📅 2026-08-28   | 经典的时序数据库项目。                          |
| [dgraph-io/dgraph](https://github.com/dgraph-io/dgraph) ⭐ 21,781 \| 🐛 96 \| 🌐 Go \| 📅 2026-08-28              | 面向关联查询场景的分布式图数据库。                    |
| [ipfs/kubo](https://github.com/ipfs/kubo) ⭐ 17,115 \| 🐛 874 \| 🌐 Go \| 📅 2026-08-27                           | IPFS 的 Go 实现。                        |
| [chrislusf/seaweedfs](https://github.com/chrislusf/seaweedfs) ⭐ 37 \| 🐛 1 \| 🌐 Go \| 📅 2026-07-21             | 高性能分布式文件系统，覆盖对象、文件和块存储。              |
| [XiaoMi/Gaea](https://github.com/XiaoMi/Gaea) ⭐ 2,765 \| 🐛 67 \| 🌐 Go \| 📅 2026-03-18                         | 小米开源的 MySQL 中间件，聚焦分库分表与代理能力。         |
| [mediocregopher/radix](https://github.com/mediocregopher/radix) ⭐ 637 \| 🐛 6 \| 🌐 Go \| 📅 2026-05-13          | 设计简洁的 Go Redis 客户端。                  |
| [olivere/elastic](https://github.com/olivere/elastic) ⭐ 7,447 \| 🐛 116 \| 🌐 Go \| 📅 2024-08-08                | Go 生态里长期被广泛使用的 Elasticsearch client。 |

## 可观测性

指标、图表、告警与运行状态检查

| 项目                                                                                                             | 简介                                                                |
| -------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| [grafana/grafana](https://github.com/grafana/grafana) ⭐ 76,465 \| 🐛 3,317 \| 🌐 TypeScript \| 📅 2026-08-29   | 最常见的可观测性可视化平台之一。                                                  |
| [prometheus/prometheus](https://github.com/prometheus/prometheus) ⭐ 65,878 \| 🐛 879 \| 🌐 Go \| 📅 2026-08-28 | 事实标准级的监控与时序指标系统。                                                  |
| [influxdata/kapacitor](https://github.com/influxdata/kapacitor) ⭐ 2,375 \| 🐛 833 \| 🌐 Go \| 📅 2026-08-10    | InfluxData 的实时计算、告警与监控处理组件。                                       |
| [sourcegraph/checkup](https://github.com/sourcegraph/checkup) ⭐ 3,458 \| 🐛 29 \| 🌐 Go \| 📅 2026-07-03       | 分布式健康检查工具，适合做站点和服务可用性探测。                                          |
| [rapidloop/rtop](https://github.com/rapidloop/rtop) ⭐ 2,187 \| 🐛 23 \| 🌐 Go \| 📅 2022-06-06                 | 基于 SSH 的轻量级远程服务器监控工具。                                             |
| [kubestellar/console](https://github.com/kubestellar/console) ⭐ 129 \| 🐛 16 \| 🌐 TypeScript \| 📅 2026-08-29 | AI 驱动的多集群 Kubernetes 仪表盘，支持实时可观测性和 30+ CNCF 项目集成。CNCF Sandbox 项目。 |

## 网络与安全

网关、负载均衡、代理、流量调试与网络工具

| 项目                                                                                                         | 简介                         |
| ---------------------------------------------------------------------------------------------------------- | -------------------------- |
| [traefik/traefik](https://github.com/traefik/traefik) ⭐ 64,639 \| 🐛 914 \| 🌐 Go \| 📅 2026-08-28         | 云原生场景里广泛使用的反向代理和负载均衡器。     |
| [google/seesaw](https://github.com/google/seesaw) ⭐ 5,676 \| 🐛 16 \| 🌐 Go \| 📅 2026-07-11               | Google 开源的 Linux 负载均衡系统。   |
| [jpillora/go-tcp-proxy](https://github.com/jpillora/go-tcp-proxy) ⭐ 798 \| 🐛 14 \| 🌐 Go \| 📅 2024-01-08 | 实现简单、非常适合学习 TCP 代理原理。      |
| [probelabs/goreplay](https://github.com/probelabs/goreplay) ⭐ 19,319 \| 🐛 341 \| 🌐 Go \| 📅 2026-01-27   | 把线上 HTTP 流量复制回测试环境的经典工具。   |
| [hidu/pproxy](https://github.com/hidu/pproxy) ⭐ 277 \| 🐛 7 \| 🌐 Go \| 📅 2024-12-20                      | HTTP 抓包代理和调试工具。            |
| [getlantern/lantern](https://github.com/getlantern/lantern) ⭐ 15,917 \| 🐛 40 \| 🌐 Dart \| 📅 2026-08-28  | 长期维护的网络代理项目，可参考跨平台网络客户端设计。 |

## Web 开发与应用

Web 框架、服务端组件与实时交互能力

| 项目                                                                                                                     | 简介                                      |
| ---------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| [gin-gonic/gin](https://github.com/gin-gonic/gin) ⭐ 89,129 \| 🐛 765 \| 🌐 Go \| 📅 2026-08-15                         | Go Web 框架里最常见的高性能选择。                    |
| [labstack/echo](https://github.com/labstack/echo) ⭐ 32,669 \| 🐛 28 \| 🌐 Go \| 📅 2026-08-24                          | API 开发体验成熟的高性能 Web 框架。                  |
| [beego/beego](https://github.com/beego/beego) ⭐ 32,415 \| 🐛 21 \| 🌐 Go \| 📅 2026-08-26                              | 老牌但仍在维护的全功能 Go Web 框架。                  |
| [revel/revel](https://github.com/revel/revel) ⭐ 13,218 \| 🐛 94 \| 🌐 Go \| 📅 2023-10-28                              | 偏完整栈思路的 Go Web 框架。                      |
| [kataras/iris](https://github.com/kataras/iris) ⭐ 25,558 \| 🐛 149 \| 🌐 Go \| 📅 2026-07-27                           | 强调性能和完整生态的 Go Web 框架。                   |
| [go-macaron/macaron](https://github.com/go-macaron/macaron) ⭐ 3,545 \| 🐛 12 \| 🌐 Go \| 📅 2026-02-16                 | 模块化风格明显的 Go Web 框架。                     |
| [andeya/faygo](https://github.com/andeya/faygo) ⭐ 1,591 \| 🐛 9 \| 🌐 Go \| 📅 2023-02-25                              | 面向 API 场景的 Go Web 框架，带参数绑定和文档生成。        |
| [olahol/melody](https://github.com/olahol/melody) ⭐ 4,083 \| 🐛 14 \| 🌐 Go \| 📅 2025-10-28                           | 基于 gorilla/websocket 的轻量级 WebSocket 框架。 |
| [valyala/fasthttp](https://github.com/valyala/fasthttp) ⭐ 23,456 \| 🐛 85 \| 🌐 Go \| 📅 2026-08-28                    | Go 里非常有代表性的高性能 HTTP 实现。                 |
| [tus/tusd](https://github.com/tus/tusd) ⭐ 3,861 \| 🐛 90 \| 🌐 Go \| 📅 2026-08-01                                     | 断点续传文件上传服务端实现。                          |
| [mattermost/mattermost](https://github.com/mattermost/mattermost) ⭐ 38,936 \| 🐛 997 \| 🌐 TypeScript \| 📅 2026-08-29 | 大型 Go Web 应用的代表项目, 适合看真实业务系统的工程组织方式。    |

## 数据处理与机器学习

ML、NLP、爬虫与数据处理

| 项目                                                                                                       | 简介                         |
| -------------------------------------------------------------------------------------------------------- | -------------------------- |
| [gorgonia/gorgonia](https://github.com/gorgonia/gorgonia) ⭐ 5,930 \| 🐛 126 \| 🌐 Go \| 📅 2024-08-12    | Go 生态里最有代表性的深度学习与张量计算项目之一。 |
| [cdipaolo/goml](https://github.com/cdipaolo/goml) ⭐ 1,614 \| 🐛 4 \| 🌐 Go \| 📅 2022-07-15              | 提供在线学习、聚类和回归等算法实现。         |
| [sjwhitworth/golearn](https://github.com/sjwhitworth/golearn) ⭐ 9,439 \| 🐛 89 \| 🌐 Go \| 📅 2024-01-15 | 更偏传统机器学习流程的 Go 库。          |
| [andeya/pholcus](https://github.com/andeya/pholcus) ⭐ 7,577 \| 🐛 3 \| 🌐 Go \| 📅 2026-08-24            | Go 编写的分布式爬虫框架。             |
| [yanyiwu/gojieba](https://github.com/yanyiwu/gojieba) ⭐ 2,646 \| 🐛 0 \| 🌐 Go \| 📅 2026-07-20          | 结巴中文分词的 Go 版本。             |
| [chrislusf/gleam](https://github.com/chrislusf/gleam) ⭐ 3,562 \| 🐛 39 \| 🌐 Go \| 📅 2026-07-25         | Go 风格的数据处理和分布式计算框架。        |

## 开发者工具与基础库

开发效率、测试、终端 UI 和核心基础库

| 项目                                                                                                                       | 简介                    |
| ------------------------------------------------------------------------------------------------------------------------ | --------------------- |
| [gohugoio/hugo](https://github.com/gohugoio/hugo) ⭐ 89,572 \| 🐛 245 \| 🌐 Go \| 📅 2026-08-28                           | 最有代表性的 Go 静态站点生成器。    |
| [grpc/grpc-go](https://github.com/grpc/grpc-go) ⭐ 23,041 \| 🐛 131 \| 🌐 Go \| 📅 2026-08-27                             | gRPC 的 Go 官方实现。       |
| [rakyll/hey](https://github.com/rakyll/hey) ⭐ 20,246 \| 🐛 189 \| 🌐 Go \| 📅 2026-01-10                                 | 轻量级压力测试工具。            |
| [visualfc/liteide](https://github.com/visualfc/liteide) ⭐ 7,767 \| 🐛 413 \| 🌐 C++ \| 📅 2026-08-15                     | 跨平台的 Go IDE。          |
| [mailslurper/mailslurper](https://github.com/mailslurper/mailslurper) ⭐ 1,511 \| 🐛 66 \| 🌐 JavaScript \| 📅 2025-12-05 | 本地开发非常实用的测试 SMTP 服务器。 |
| [gizak/termui](https://github.com/gizak/termui) ⭐ 13,582 \| 🐛 106 \| 🌐 Go \| 📅 2025-07-10                             | 在终端里构建可视化面板的 Go UI 库。 |
| [golang/mobile](https://github.com/golang/mobile) ⭐ 6,211 \| 🐛 37 \| 🌐 Go \| 📅 2026-08-21                             | Go 官方维护的移动端开发工具链。     |
| [hound-search/hound](https://github.com/hound-search/hound) ⭐ 5,875 \| 🐛 118 \| 🌐 JavaScript \| 📅 2026-08-13          | 适合自建的代码搜索工具。          |

## 区块链

仍在维护、影响力最大的 Go 区块链项目

| 项目                                                                                                           | 简介                 |
| ------------------------------------------------------------------------------------------------------------ | ------------------ |
| [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) ⭐ 51,314 \| 🐛 423 \| 🌐 Go \| 📅 2026-08-28 | 以太坊客户端 geth 的官方实现。 |
| [hyperledger/fabric](https://github.com/hyperledger/fabric) ⭐ 16,706 \| 🐛 205 \| 🌐 Go \| 📅 2026-08-28     | 企业级联盟链平台的代表项目。     |

## 维护说明

目录已经去掉旧版 README 中的重复收录、过时仓库和“其它”大杂烩分类。后续如果继续扩展，建议优先更新 [projects.json](projects.json)，再运行 `go run ./tools/generate_readme.go` 同步生成 README。

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._
