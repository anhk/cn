# 产品功能


## 设备通信

- 提供设备与云端的双向通信，设备上报与指令下发设备稳定可靠。

## 设备管理

- 设备注册：通过预置物类型注册设备。
- 设备状态：可以实时获取设备状态信息。
- 设备数据采集： 通过物模型上报设备数据到云端，随时查询设备数据。
- 设备删除：通过云端控制台禁用或删除可疑设备，调配设备，进行便捷设备管理。
- 设备分组：可根据需要创建设备分组、支持父级下选择相应的设备。

## 物模型

- 物模型：设备在云端的功能描述，通过统一的物模型定义，标准化数据，包括设备的设备遥测数据属性、设备状态属性、设备控制指令。物模型采用JSON格式描述。
- 创建物类型：可创建直连设备、连接代理设备及非直连设备三种物类型。
- 物类型删除：通过云端控制台删除已创建物类型。注意：如物类型下已经注册设备，则该物类型不可删除！
- 物模型：设备在云端的功能描述，通过统一的物模型定义，标准化数据，包括设备的设备遥测数据属性、设备状态属性、设备控制指令。物模型采用JSON格式描述。
  - 物模型 – 设备遥测数据：设备上行的报文流式数据，是一个描述客观事实的观测值，不可被云端服务或者其他应用修改。
  - 物模型 – 设备状态属性：设备状态数据，例如设备的运行状态等，相对于报文数据，更新频率较低。状态属性可以被云端服务或者其他应用修改。
  - 物模型 – 设备控制指令：云端服务或其他应用主动调起或者规则引擎中某条规则触发的对设备的控制指令，此类指令不修改设备状态属性。例如对于所有的设备的消息广播指令。
- 提供设备影子的缓存机制，保证设备在网络不稳定的情况下通信可靠正常。

## 规则引擎

- 数据处理：对物联网引擎接收的设备数据进行预处理，支持条件筛选，过滤。
- 数据转储：将处理后的数据转发转储到京东云其他服务，例如RDS，JCQ，ES等。
- M2M场景：基于规则引擎可以配置规则事项设备与设备之间的通信，快速实现M2M场景。

## 档案管理
- 新增档案：可基于全局设备、全局物类型、物类型设备创建相应的档案
- 查询档案：全局及分类型查询相应的档案
- 编辑档案：可修改档案的类型、物类型、档案名称、档案编码及其它属性及说明。
- 删除档案：可删除选定的档案。

## 相关参考

- [产品概述](../Introduction/Product-Overview.md)
- [价格总览](../Pricing/Price-Overview.md)



