# SLA


**1.服务范围**

京东云DevOps服务，是京东云结合自身自动化运维技术与能力的基础上，针对公有云的场景和特性，构建的一套DevOps服务。简化部署、监控、运维等应用的生命周期管理环节，从而大大提升运维效率和稳定性，助力企业快速实现服务搭建及高效稳定运维。


**2.服务等级指标**

**2.1数据持久性**

数据持久性：不低于99.999%

数据持久性按服务周期统计，一个服务周期为一个自然月，如不满一个月不计算为一个服务周期。

**2.2数据可销毁性**

2.2.1在用户主动删除数据或用户服务期满后需要销毁数据的，京东云将自动清除对应物理服务器上磁盘和内存数据，使得数据无法恢复。

2.2.2云服务所用的设备在报废弃置、委外维修或转售前，京东云将对其物理磁盘采用消磁操作。

**2.3数据可迁移性**

用户使用DevOps服务时，京东云提供程序包版本管理功能，包括上传与下载，以便于用户快速部署。

**2.4数据私密性**

京东云使用加密和安全组隔离等手段保证不同资源池用户数据互不可见。

**2.5数据知情权**

2.5.1用户对于数据、备份数据所在数据中心地理位置、数据备份数量具有知情权，其中：

2.5.1.1目前京东云数据中心分别位于华北（北京）、华东（宿迁）、华东（上海）、华南（广州），用户在开通云服务时必须根据地理位置选择相应的数据中心，用户数据将存储在其指定的数据中心；

2.5.1.2京东云服务具备自动数据备份功能，备份数据默认与源数据存储在同一个数据中心。用户无需指定数据自动备份数量及自动备份数据所存储的位置。

2.5.2京东云的数据中心将遵守当地的相关法律法规，用户对此具有知情权，并可联系京东云的客户服务人员获得详尽信息。

2.5.3 除应当地法律法规、或政府监管部门的监管、审计要求，用户的所有数据、应用及行为日志不会提供给第三方。除用于京东云的产品运行状态的统计分析，用户的行为日志不会对外呈现用户个人信息数据。

**2.6数据可审查性**

依据现行法律法规或根据政府监管部门监管、安全合规、审计或取证调查等原因的需要，在符合流程和手续完备的情况下，京东云可以提供用户所使用的服务的相关信息，包括关键组件的运行日志、运维人员的操作记录、用户操作记录等信息。

**2.7服务功能**

DevOps服务具有CMDB、CICD、智能监控、运维工具等功能，DevOps服务的所有具体功能详见京东云在官网上提供的详细说明文档、技术文档及帮助文档。DevOps服务所有可能影响用户的功能性变更都将向用户公告。

**2.8 服务可用性**

服务可用性：不低于99.99%。

DevOps服务可用性按服务周期统计，一个服务周期为一个自然月，如不满一个月不计算为一个服务周期，统计的业务单元为单个功能模块，时间单位为分钟。

不可用时间：DevOps服务所提供的服务在连续的5分钟或更长时间不可使用方计为不可用时间，不可使用的服务时间低于5分钟的，不计入不可用时间，DevOps服务不可用时间不包括日常系统维护时间、由用户原因、第三方原因或不可抗力导致的不可用时间（具体见2.12.1条）。

**2.9 服务资源调配能力**

DevOps服务提供多种配置并具备弹性扩缩容能力，用户可根据需要按照京配置方案自行在线扩展或缩减所使用的资源。

**2.10 故障恢复能力**

京东云为付费用户的云服务提供7×24小时的运行维护，并以电话报障等方式提供技术支持，具备完善的故障监控、自动告警、快速定位、快速恢复等一系列故障应急响应机制。

**2.11 服务计量准确性**

DevOps服务具备准确、透明的计量计费系统，京东云根据用户的实际使用量据实结算，实时扣费，具体计费标准以京东云官网公布的有效的计费模式与价格为准。用户的原始计费日志默认最少保留1年备查。

**2.12 服务赔偿条款**

2.12.1 赔偿范围：

因京东云故障导致DevOps服务无法正常使用，以及京东云故障引起的网站无法正常访问，京东云将对不可用时间进行赔偿，但不包括以下原因所导致的服务不可用时间：

（1）京东云预先通知用户后进行系统维护所引起的，包括割接、维修、升级和模拟故障演练；
（2）由于运营商故障导致的丢包和延时等不可用情况；
（3）用户的应用程序或数据信息受到黑客攻击而引起的；
（4）用户维护不当或保密不当致使数据、口令、密码等丢失或泄漏所引起的；
（5）用户自行升级操作系统所引起的；
（6）用户的应用程序或安装活动所引起的；
（7）用户的疏忽或由用户授权的操作所引起的；
（8）不可抗力以及意外事件引起的；
（9）其他非京东云原因所造成的不可用。

2.12.2 赔偿方案

故障时间=不可用时间。

对于免费使用DevOps服务，不予赔偿。
对于付费使用DevOps服务，以补充服务时长的方式，按照故障时间100倍赔偿
赔偿总时长不超过已支付的服务总时长。



**3.其他**

京东云有权根据变化适时对本服务等级协议部分服务指标作出调整，并及时在京东云官网 www.jdcloud.com 发布公告或发送邮件或书面通知向用户提示修改内容。



