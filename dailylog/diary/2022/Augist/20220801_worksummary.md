

# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|大棚:USB没有端口| 中 |50%  |USB数据包异常| 解决中|1Ｄ|
|大棚:USB枚举成U2| 中 |50%  |增加软件复位逻辑|输出测试包|1Ｄ|
|大棚:其他缺陷处理| 中 |50%  |休眠事件上报，psensor唤醒，缺陷流程处理，配合龙讯更新|输出测试包|0.5Ｄ|
|固件组手册项目| 中 | 80%  |完成wiki搭建| 完成|1.5D|
|RH：display| 中 | 5%  |任务梳理| 完成|0.5D|
|RH：地磁模块| 中 | 5%  |任务梳理| 解决中|2H|
|E34R ESD| 中 |80%  |E34Rdvt ESD宏的问题，没有放开，使能后合到dailybuild分支后，通知测试验证。| 解决中|0.5D|


# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|大棚:问题解决| 中 |50%  |USB没有端口| 解决中|1Ｄ|
|RH：地磁| 中 | 10%  |业务和模块梳理| 投入|3D|
|RH：display| 中 | 5%  |任务分解| 投入|1D|

2805V5换成 AK099 

# 挂起任务
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
| oppo项目 | 低 | ５%  | 7911uxc代码合入ｂｒａｎｃｈ分支| 待解决| ２Ｄ  |
| 框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | １０D|
| RK平台开发| 中 | ６%  |内核裁剪与裁剪| 解决中| ２Ｄ|
| BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 |２D|
|JunkeV2| 中 | 10%  |E34R静电检测,HID单步测试，每个状态的复位问题| 提交代码|1D|
|JunkeV2| 中 | 10%  |fisheye帧间隔问题imu上报数据问题| 提交代码|2D|

# 任务说明：
## 【缺陷】
【缺陷】<font color='red'> 【中优先级】  </font>E34R静电检测
- 结论：
    -　优化后最短时间１最后有３％的概率 无法点亮为ＥＰＳＯＮ光机无法点亮．
    -  新的机器DVT2设备，ESD功能失效，
- 计划：    
    - 单步ＨＩＤ命令，当出现问题后，单步查看每个步骤．
    - 目前让测试人员收集日志。



## 【缺陷解决】
1. <font color='red'> 【高优先级】  </font>大棚产线
- [问题2]USB识别不出端口问题
   - 当前通过USB分析仪器，显示数据包全是未知的数据包。
   - 未定位到具体原因 
   - main函数，判断USB枚举成功与否，1.5s.超时等待
   - JTAG 看下能否他出现。在Jtag仿真运行的情况下，始终是U3并且能稳定识别出来。
   - 就需要看一下，仿真运行下和插拔运行下，有什么不一样。
   - 仿真运行下，USB没有断过电源，是不是插拔的过程会导致USB信号不稳定。
   - 目前这个问题，在HUB的情况下可以复现，USB线材那边反应，可以先不看hub
   - 如果只升级USBloader，能识别出来端口，但是升级。
   - 这个问题，只是在HUB情况下，可以出现。目前待验证。
   - 仿真情况，不断插拔，没有出现无端口的问题，让测试帮忙测试下。提供环境，
- 提一个测试说明。 
- 试下，log_printf uart 串口，
  

1. <font color='red'> 【中优先级】  </font>RH:地磁的问题，
- 进展：
- imu业务。了接项目的背景。
- 
3. <font color='red'> 【中优先级】  </font>RH:显示模块
- 进展：
- 分解和设计模块。


4. <font color='red'> 【中优先级】  </font>fisheye 间隔问题，imu
- 进展：裸板无法写入校验参数，无法调试，还需投入。

5. <font color='red'> 【中优先级】  </font> junke no imu 版本，SDK发现错误的HID命令，导致imu会一直上报数据，
- 进展：待验证


## 【组织建设】
建立内部wiki： http://192.168.20.22/mediawiki/index.php/%E9%A6%96%E9%A1%B5



