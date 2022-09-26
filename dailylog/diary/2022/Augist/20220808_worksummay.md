

# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|大棚:USB没有端口,cd-room后无法点亮| 中 |50%  |USB异常，导致UAC协议阻塞|解决中|2.5Ｄ|
|大棚:偶现闪屏问题| 中 |50%|增加背光芯片寄存器获取接口|输出测试包|0.5Ｄ|
|大棚:屏幕错位问题| 中 |50%|原厂沟通，更换龙讯hex|输出测试包|0.5Ｄ|
|大棚:会议处理缺陷流程| 中 |50%|缺陷流程处理|会议记录|0.5Ｄ|
|E34R ESD| 中 |80% |E34Rdvt ESD宏的问题，没有放开，使能后合到dailybuild分支后，通知测试验证。| 解决中|0.5D|
|JunkeV2| 中 |80% |junkeveUSB，待合入主分支，目前代码还需要修改，存入flash失败| 解决中|0.5D|
|RH：display| 中 | 5% |协助解决调试点不亮的问题| 解决中|3H|
|RH：地磁模块| 中 | 5% |建立源码文件修改| 解决中|2H|
|E34设置redriver| 中 | 5% |003模式，redriver做了那些配置| 解决中|0.5D|

# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|E34设置redriver| 中 | 5% |003模式，redriver做了那些配置| 解决中|2H|
|E34R ESD| 中 |80% |E34Rdvt合入后，时间效果没有之前好，需要确认小效果。| 解决中|0.5D|
|JunkeV2| 中 |80% |junkeveUSB，需要修改存入flash区域，存入flash失败| 解决中|0.5D|
|大棚:USB没有端口,cd-room后无法点亮| 中 |50%  |USB异常，导致UAC协议阻塞|解决中|2.5Ｄ|
|RH：display| 中 | 5% |协助解决调试点不亮的问题| 解决中|3H|
|RH：地磁模块| 中 | 5% |建立源码文件修改| 解决中|2H|




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
   - USB挂载上，但是处于异常状态，导致UAC协议阻塞，引起一系列异常，
- [解决方法]找到失败方法，更新固件
  

1. <font color='red'> 【中优先级】  </font>RH:地磁的问题，
- 进展：
- 编码中
- 
1. <font color='red'> 【中优先级】  </font>RH:显示模块
- 进展：
-调试中


1. <font color='red'> 【中优先级】  </font>fisheye 间隔问题，imu
- 进展：裸板无法写入校验参数，无法调试，还需投入。

5. <font color='red'> 【中优先级】  </font> junke no imu 版本，SDK发现错误的HID命令，导致imu会一直上报数据，
- 进展：待验证

 <font color='red'> 【中优先级】  </font>other
1. 设置0增益测试，redriver
2. E34Rdvt合入后，查看效果是否可优化
3.junkeveUSB，需要修改存入flash区域，存入flash失败
4.USB异常，导致UAC协议阻塞


升级过后，DP是否开启，当前7911是否开启。framework和usbloader redriver是否有差异。
ak9188的设备问题。
usb loader 没有设置DP。7911上电也。