
# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态|投入时间 |
|-----|-------| ---- | ---|----|--------|
|HID DP 寄存器透传| 中 |100%|完成HID程序包，接口文档输出|输出测试包|1.5Ｄ|
|cougerv5：HID接口切换imu频率| 中 |50%|手动切换1kz频率失败|解决中|1.5Ｄ|
|DP:pesenor低概率失败| 中 |10%|未发现问题，增加打印给测试复现|解决中|0.5Ｄ|
|MTK：gerrit代码| 中 |10%|gerrit无法正常启动|解决中|0.5Ｄ|

# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|cougerv5：HID接口切换imu频率| 中 |100%|手动切换1kz频率失败|解决中|0.5Ｄ|
|DP:120hz频率选项切换缺失| 中 |10%|代码走读|解决中|1Ｄ|
|MTK：gerrit代码| 中 |10%|gerrit无法正常启动，解决完成后重新推代码|解决中|2.5Ｄ|
|junkeV2：偶现时间戳glass值是一个异常的值| 中 |10%|需要增加日志打印|解决中|2.5Ｄ|

# 挂起任务
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | １０D|
|BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 |２D|
|JunkeV2| 中 | 10%  |fisheye帧间隔问题imu上报数据问题| 提交代码|2D|
|E34R静电检测| 中 | 10%  |HID单步调试，解决| 提交代码|2D|
|固件组:资料整理| 中 |10%|打包，升级，flash存储，CPU运行框架|ppt|2D|


## 【缺陷解决】


1. <font color='red'> 【高优先级】  </font>gerrit+Jenkins
- bylibre 的源码，repo管理问题，投入了点时间，解决漏上传问题。
- Jenkins 先在本地安装测试，下一步部署在编译服务器，新起一个docker单独编译。
- 考虑FTP问题。

- 重启Nginx，gerrit登录不了，就解决了。

- 复制一台win虚拟机

