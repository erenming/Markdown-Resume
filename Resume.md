 <center>
     <h1>姜闻名</h1>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="18px">
             xxx
         </span>
         ·
         <span>
             <img src="assets/envelope-solid.svg" width="18px">
             xxx@gmail.com
         </span>
         ·
         <span>
             <img src="assets/github-brands.svg" width="18px">
             <a href="https://github.com/erenming">erenming</a>
         </span>
     </div>
 </center>

 ## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息 

 - 求职意向：可观测性研发工程师
 - 教育经历：华侨大学，土木工程，2013.6-2017.9
 ## <img src="assets/info-circle-solid.svg" width="30px"> 摘要

熟练掌握可观测相关技能和方法。拥有7年开发经验，且一直从事于监控可观测领域。热衷并善于解决各种疑难杂症，追求代码简洁严谨。拥有良好的沟通能力，能与其他团队高效合作。

## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

**溪数科技，采集组，研发工程师，2023.6~至今**

负责KetaOps平台采集侧的开发维护

- 主导APM采集侧的设计研发，包括引入并扩展OTEL探针、探针自动注入等。
- 开发维护KetaAgent，包括插件开发、Agent配置管理优化等各项功能开发。

**端点科技，监控组，研发工程师， 2020年3月-2023年12月**

负责Erda平台可观测性（监控）部分的开发维护

- 主导时序数据库的迁移工作，将可观测性数据统一迁移到ClickHouse，极大地降低了存储和写入成本。
- 重构Collector组件，将其解耦并模块化，实现代码复用及数据处理可配置化。
- 持续优化可观测性数据传输链路，包括稳定性、安全性以及性能等方面。
- 切换日志和指标采集Agent，促进了平台的云原生化。

**浙江胄天科技，后端开发工程， 2018年3月-2020年3月**

负责测风设备平台的开发维护

- 基于北斗传输协议自研传输协议开发了测风数据上报功能，实现了测风每日上报。

**北京金道天成信息技术，运维开发工程师， 2017年6月-2018年3月**

担任运维开发工程师，负责运维巡检平台（铜雀）的开发维护

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历

**APM探针自动注入 2023年08月-2023年12月**

*在用户无感知的情况下，将APM探针自动注入到用户进程中*

- 基于LD_PRELOAD技术并使用C编写动态库，支持包括服务名自动探测、进程白名单、自定义服务名等功能，实现了在Linux下的自动注入。
- 引入并修改官方Opentelemetry Operator，主要包括持兼容低版本k8s，权限依赖最小化改造，实现了k8s环境下的自动注入

**APM探针二次开发 2023年10-2024年04月**

*对OTEL探针进行扩展及二开，以解决并满足了客户的个性化问题及需求*

- 通过开发增强包扩展了OTEL的Java探针，支持了原生日志关联、探针日志重定向等功能。同时协助客户统一日志格式，实现了trace和日志关联查询。
- 二次开发Nginx探针，包括支持采样率、解决探针Bug等，成功帮助客户将Kong和Openresty接入APM，得到了客户肯定。

**可观测性数据迁移 2022年05月-2022年08月**

*迁移可观测性数据存储至ClickHouse，实现了降本增效的目标*

- 设计Metrics, Logs和Traces三种数据的ClickHouse表结构：经反复调研、测试及权衡后，最终通过牺牲部分存储成本（约30%），设计出了结构简单且查询性能良好的表结构。
- 开发ClickHouse写入模块，抽象通用写入逻辑，包括模板化DDL、写入流控、动态攒批等。
- 优化实际上线后的性能问题：通过优化慢SQL，使页面整体响应由30s+降低到5s以内。通过动态攒批，消除小批次数据写入请求。

**Collector组件重构 2021年03月-2021年06月**

*重构数据处理组件Collector，降低了维护成本，提升了代码复用性*

- 解耦数据接收、处理和导出逻辑，抽象成Receiver、Processor和Exporter并插件化。并支持以Pipeline的方式将其链接，从而实现了通过配置文件即可处理数据，而无需重复编码。

**采集组件云原生化 2020年06月-2020年08月**

*对指标和日志采器端进行迁移，并促进了平台的云原生化*

- 日志和指标采集器由二开版本的Telegraf和Filebeat切换为Prometheus和FluentBit，并使用Operator进行管理；同时推动sre团队将平台tag注入到注解中。

## <img src="assets/tools-solid.svg" width="30px"> 技术栈

- 编程语言：工作不受语言限定，尤为熟悉Go，较为熟悉Java，C/C++，Python，Shell
- 可观测性：熟悉OTEL，Prometheus，Telegraf，Beats，FluentBit，eBPF；Kafka，ClickHouse，MySQL；了解ES，Flink，Cassandra
- 运维&系统：熟悉Linux，Docker，Kubernetes及Helm、Operator等云原生技术栈