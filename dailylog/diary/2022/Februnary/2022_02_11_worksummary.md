# 上周投入
| 任务| 优先级 | 进度 | 问题 | 状态| 投入时间| 
| ------ | ------ | ------ |------ |------ |------ |
| BUG |中 |  90%|type-C&A识别优化和接845box热插拔出现异常|解决中|2H
| BUG |中 |  100%|E34R 连接三星S21 手机即使有外部供电也无法打开viewer|完成|1.5D
| BUG | 中 | 90%|junke连接亿镜板子，USB异常掉端口问题|完成|0.5D
| 临时任务 | 高 | 100%|配合Daniel，修改代码测试|完成|0.5D
| 开发任务 | 高 | 30%|linux-kernel时间同步驱动|解决中|2.5D
| Bringup显示 |低 | 0%|代码合并|待机解决|0D
| 框架优化 |低 | 10%|输出一版细化，再次会议讨论结构体设计|解决中|0D

# 本周计划
| 任务| 优先级 | 进度 | 问题 | 状态| 计划时间| 
| ------ | ------ | ------ |------ |------ |------ |
| BUG |中 |  90%|type-C&A识别优化和接845box热插拔出现异常|解决中|0.5D
| BUG | 中 | 90%|junke连接亿镜板子，USB异常掉端口问题|完成|0.5D
| 开发任务 | 高 | 30%|linux-kernel时间同步驱动|解决中|3D

# 任务说明：
## 【缺陷】
【缺陷】<font color='red'> 【中优先级】  </font>type-C&A识别优化和接845box热插拔出现异常
- 进展：龙迅需要抓AUX波形。
- 结论：搭建环境和matt一起抓失败下的波形。

  
【缺陷】<font color='red'> 【中优先级】  </font>junke连接亿镜板子，USB异常掉端口问题
- 进展：完成固件和测试文档输出。暂时不需要投入。
- 存在问题：usb初始化在flash获取USB witch之前，所以USB会先默认设置为0.再根据Flash保存的参数获取USB witch状态。
- 影响：暂时未发现问题。

  
【缺陷】<font color='red'> 【中优先级】  </font>E34R 连接三星S21 手机即使有外部供电也无法打开viewer  
- 进展：定位到是由于RGB camera打开导致的。已经转给安卓端。暂时不需要投入


 ## 【开发任务】 
 1.<font color='red'> 【高优先级】  </font>linux-kernel时间同步驱动
 - 进展：
   - 完成驱动梳理，驱动示例提供。
   - 完成时间同步功能梳理。
- 问题
   - glass端，存在编译报错问题，需要解决。
   - Android端，脉冲信号没有输出，
- 计划：
   - 本周内编译驱动在开发板中跑通流程。 


 2.<font color='red'> 【低优先级】  </font> 输出一版细化，再次会议讨论结构体设计。
 - 进展：
   - 完成分层框架设计。
   - 完成框架方向设计。
- 计划：
  - 对象编程和流式API编程伪代码梳理。
  - 输出详细设计稿，开会讨论。
  - make编译流程梳理。

