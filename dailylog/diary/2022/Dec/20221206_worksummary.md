# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态|投入时间 |
|-----|-------| ---- | ---|----|--------|
|E34RE 低功耗| 中 |50%|测试逻辑|输出集成包|1.5Ｄ|
|jenkins| 中 |30%|部署Jenkins，完成在本地测试，下一步在编译服务测试|在本地部署|2Ｄ|
|Junkev2| 中 |10%|禁止掉SPK驱动注册，非标UAC和movidius的UAC都测试过，未解决|未解决|1.5Ｄ|
|大鹏| 中 |100%|配合SDK搭建调试环境，输出固件|解决|0.5Ｄ|


# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|E34RE 低功耗| 中 |80%|psensor触发，会引起手机重新弹框APK选择|解决中|1Ｄ| 完成。

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
- 浅睡，重新佩戴，手机会弹框。独立audio引起的。

1. <font color='red'> 【高优先级】  </font>gerrit+Jenkins
- bylibre 的源码，repo管理问题，投入了点时间，解决漏上传问题。
- Jenkins 先在本地安装测试，下一步部署在编译服务器，新起一个docker单独编译。
- 由于安装新的配置，导致本地wiki无法使用，投入了0.8D时间

2. audio是否引起该问题。
3. 音频和视频。有深睡。其他没有深睡，关掉。这个一定
4. E34R 设备

|Junkev2| 中 |10%|禁止掉SPK驱动注册，非标UAC和movidius的UAC都测试过，未解决|解决中|1.5Ｄ| x
|大鹏| 中 |10%|修睡眠逻辑，睡眠受不关闭fisheye|待解决|1.5Ｄ| 验证，休眠唤醒不会影响fisheye测试
|jenkins| 中 |30%|部署Jenkins，完成在本地测试，下一步在编译服务测试|解决中|2Ｄ| x


直接虚拟机上拉代码编译。

