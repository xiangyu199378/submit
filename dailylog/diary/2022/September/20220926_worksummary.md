# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|大棚：FLASH参数异常问题| 中 |50%|Flash参数异常，导致读取参数时指针越界，解决越界问题，未找到异常原因|解决中|3Ｄ|
|大棚：升级失败| 中 |50%|没有端口framework没有启动，升级超时没有接受的NDF数据包|解决中|0.5Ｄ|
|K40RE：音频出现中断的问题| 中 | 20% |UAC播放过程中会收到停止消息| 解决中|3D|


# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|大棚：FLASH参数异常问题| 中 |50%|走查FLASH存储代码|解决中|3Ｄ|
|K40RE：音频出现中断的问题| 中 | 20% |UAC驱动兼容问题，需要梳理UAC代码结构和协议内容，需要排查loading是否有影响| 解决中|3D|


# 挂起任务
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | １０D|
|BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 |２D|
|JunkeV2| 中 | 10%  |fisheye帧间隔问题imu上报数据问题| 提交代码|2D|
|E34R静电检测| 中 | 10%  |HID单步调试，解决| 提交代码|2D|
|固件组:资料整理| 中 |10%|打包，升级，flash存储，CPU运行框架|ppt|2D|

## 【缺陷解决】
1. <font color='red'> 【高优先级】  </font>大棚产线
- [问题1]有概率升级失败问题。
   - 升级会超时。设备未收到NDU升级包。
   - 升级会偶现固件启动失败，表现就是设备没有端口，重新插拔后解决。

- [问题2]仿真过程中，遇到FLASH读取指针崩溃的问题，仿真过程中出现，数据类型长度会出现异常长度值。
   - 目前方向，不同branch版本切换会导致该问题，flash异常。
   - 需要走查逻辑。

2 . 所有的设备，BACKUP，
- 所有的设备都downup出来。
- crash的问题，写工具。
- 换一个工程，也会出现FLASH崩溃问题。
- 测试帮忙复现。
3 K40RE过程。
- 使用原生的845BOX，音频不会断。QQ音乐。
- 使用VR投屏查看。
- 



 guest
	
 P@ssXvisio
 mount -t cifs //192.168.20.206/testfile /home/mnt -o user=guest,password=P@ssXvisio