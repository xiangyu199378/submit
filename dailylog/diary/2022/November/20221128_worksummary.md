# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|放开设备状态验证| 中 |100%|增加HID使能接口|完成|0.5Ｄ|
|K40RE：客户反馈无法正常显示| 中 |100%|配合SDK抓日志|提供日志|0.5Ｄ|
|大棚：休眠事件修改| 中 |100%|事件上报改为状态上报|完成|1Ｄ|
|E34RE 低功耗| 中 |50%|完成逻辑修改，RGB和fisheye休眠唤醒后是否正常，待验证|提供日志|3Ｄ|

# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|E34RE 低功耗| 中 |50%|完成逻辑修改，RGB和fisheye休眠唤醒后是否正常，待验证|提供日志|3Ｄ|
|gerrit| 中 |10%|部署gerrit+Jenkins，实现自动编译|完成手册编写|2Ｄ|


# 挂起任务
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | １０D|
|BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 |２D|
|JunkeV2| 中 | 10%  |fisheye帧间隔问题imu上报数据问题| 提交代码|2D|
|E34R静电检测| 中 | 10%  |HID单步调试，解决| 提交代码|2D|
|固件组:资料整理| 中 |10%|打包，升级，flash存储，CPU运行框架|ppt|2D|

## 【缺陷解决】

1. <font color='red'> 【高优先级】  </font> E34RE 低功耗
- 修改demo-api能够记录重启事件。
- 目前在手机测试USB挂起，cpu低功耗模式下，最新电流26MA，是否会有其他问题在确认中。
- 系统休眠唤醒后，RGB数据丢失待定位，fisheye数据待检测，
- slam在测试中偶有数据停止，目前不能确认跟休眠相关，因为设备正常起来也会有数据不上报的问题，


2. <font color='red'> 【高优先级】  </font>gerrit
- 出一个开发人员，单独新增一个库的方法。
- 鹏哥已经自己完成。
- 自己后续补上。
- 之前开发板使用的aosp源码问题，有时间看下。
