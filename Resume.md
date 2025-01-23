 <center>
     <h1>姜闻名</h1>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="18px">
             13296715293
         </span>
         ·
         <span>
             <img src="assets/envelope-solid.svg" width="18px">
             erenming233@gmail.com
         </span>
         ·
         <span>
             <img src="assets/github-brands.svg" width="18px">
             <a href="https://github.com/erenming">erenming</a>
         </span>
         ·
         <span>
             <img src="assets/rss-solid.svg" width="18px">
             <a href="https://erenming.github.io/">My Blog</a>
         </span>
     </div>
 </center>



 ## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息 

 - 求职意向：Golang开发 -- 可观测性方向
 - 教育经历：华侨大学 -- 2013.6-2017.9
 ## <img src="assets/tools-solid.svg" width="30px"> 技术栈

- 编程语言：精通Golang，熟悉Python，Java，C/C++
- 可观测性：掌握OTEL，Telegraf，Beats，FluentBit，eBPF，Prometheus
- 中间件：掌握Kafka，ClickHouse，熟悉MySQL，Redis，ES，Flink，Cassandra
- 系统和运维：熟悉Linux，Kubernetes，容器以及Windows


## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

**溪数科技 -- 采集组 -- 研发工程师 -- 2023.6-至今**

负责KetaOps产品中，采集侧的开发与维护

- 通过引入并扩展OTEL探针以及实现探针自动注入，完成APM产品中采集侧的开发
- 通过引入eBPF技术并开发ebpf-agent，完成NPM产品中采集侧的开发
- 优化重构KetaAgent，包括代码结构优化，进程管理优化，数据处理支持并行等

**端点科技 -- 监控组 -- 研发工程师 -- 2020年3月-2023年12月**

负责Erda平台可观测性（监控）部分的开发维护

- 通过将时许存储层改为ClickHouse，降低了10倍的存储，及4倍的写入成本
- 通过采用Pipeline架构重构了Collector组件，提升了该核心组件的扩展性和稳定性。
- 持续优化可观测性数据传输链路，包括稳定性、安全性及性能等方面。

**浙江胄天科技 -- 研发部 -- 后端开发 -- 2018年3月-2020年3月**

担任后端开发工程师，负责雷达测风设备平台的开发维护

**北京金道天成 -- 研发部 -- 运维开发 -- 2017年6月-2018年3月**

担任运维开发工程师，负责运维巡检平台（铜雀）的开发维护

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历

**KetaAgent优化重构 2024年04月-至今**

*负责KetaAgent的日志维护开发，并递进式地完善和重构*

- 代码结构优化：按功能分拆go.mod并调整编译打包，删除冗余代码，调整包名等，有效提升了项目的可维护性

- 代码优化重构：进程管理模块重构，支持通过gRPC与子进程通信，实现notify机制；数据处理支持并行处理；心跳逻辑优化；数据结构模型优化；

**eBPF探针开发 2023年10月-2023年12月**

*为实现NPM产品功能，引入了eBPF技术并完成采集侧的研发*

- 引入并二开DataDog的ebpf模块作为KetaAgent项目一部分，实现了编译打包，支持了主机和K8S环境下的正常部署和运行

**APM探针开发 2023年08月-2023年12月**

*负责APM产品，探针侧从0到1的研发工作*

- 调研引入并二开OTEL探针：二次开发扩展Java探针，支持原生日志关联、探针日志重定向等功能。同时协助客户统一日志格式，实现Trace和日志关联查询；二次开发Nginx探针，包括支持采样率、解决探针Bug等，成功帮助用户将Kong和Openresty接入APM
- 实现探针自动注入：基于LD_PRELOAD技术并使用C编写动态库，支持包括服务名自动探测、进程白名单、自定义服务名等功能，实现了在物理机环境下的自动注入；修改官方Operator，包括支持兼容低版本k8s、权限依赖最小化，实现了k8s环境下的自动注入

**可观测性数据迁移 2022年05月-2022年10月**

*迁移可观测性数据存储至ClickHouse，实现了存储侧降本10倍以上*

- 设计Metrics, Logs和Traces数据的ClickHouse表结构：经反复调研、测试及权衡后，最终以通过牺牲部分存储成本（约30%）的代价，设计了结构简单且查询性能良好的表结构。
- 开发ClickHouse写入模块，抽象通用写入逻辑，实现了模板化DDL、写入流控、动态攒批、数据过期管理等功能。
- 优化性能：实际上线后出现了一些性能问题，通过优化慢SQL，使页面整体响应由30s+降低到5s以内。通过动态攒批消除小批次数据写入请求，提升整体写入性能。

**Collector组件重构 2021年03月-2021年06月**

*重构数据处理组件Collector，解耦数据接收、处理和导出逻辑并抽象化、插件化，并以Pipeline的模式链接*

**测风雷达设备平台开发 2018年03月-2020年06月**

负责海上测风雷达设备的数据收集、传输、存储及控制功能的研发

**测风雷达设备平台开发 2017年06月-2018年03月**

负责“铜雀”私有云健康巡检平台的研发

 ## <img src="assets/info-circle-solid.svg" width="30px"> 摘要

熟练掌握可观测相关技能和方法。拥有8年工作经验，一直从事于监控可观测领域。喜欢挑战自我，追求代码简洁。拥有良好的沟通能力，能与其他团队进行高效合作。