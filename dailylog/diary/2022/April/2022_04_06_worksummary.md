<font color='red'> #include "Monday , March 21 ,2022 yingguang work summary "  </font>

# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态   | 投入时间 |
| -- | -- | ---- | -----| ------ | -------- |
| BUG：DP信号问题 | 中| ７０%  |修改提交专项测试后合入| 解决中 | 1D|
| docker搭建８４５安卓环境 | 中 | ５%  |docker 手册整理中| 解决中| １Ｄ|
| RK平台开发| 中 | ５%  |源码编译，烧写完成，剩余调试和裁剪| 解决中| ４Ｄ|

# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
| docker环境| 中 | ５%  |docker 手册整理中，在ＩＴ服务器上推送ｄｏｃｋｅｒ和源码管理| 解决中| １Ｄ|
| BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 | １D|
| RK平台开发| 中 | ６%  |剩余调试和内核裁剪| 解决中| １Ｄ|
| ＯＳＡＫ０９９１８摄像头调试 | 低 | ５%  |  解决无法读取数据问题，剩余业务代码| 待解决| 0Ｄ  |
| 框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | 0D|

# 任务说明：
## 【缺陷】
  
【缺陷】<font color='red'> 【中优先级】  </font>type-C&A识别优化和接845box热插拔出现异常
- 进展：当前在epson 平台，２.0 和　３.0 标志存在有误，导致逻辑结果存在误判，需要定位。
- 计划：
　　　- 在原有代码，原有平台验证逻辑为什么正常
　　　- 验证版本号对dp读取是否有影响。


 ## 【开发任务】 
１.<font color='red'> 【中优先级】  </font>ｄｏｃｋｅｒ搭建８４５安卓环境
 - 进展：完成本地ｄｏｃｋｅｒ搭建
 - 计划：
    - 推送代码ｄｏｃｋｅｒ镜像到ＩＴ服务器。
    - 运行ｄｏｃｋｅｒ，拉取ｓｄｋ源码，编译。

１.<font color='red'> 【中优先级】  </font>ＲＫ平台开发
- 进展：
    - 内核单独编译，ｕｂｏｏｔ单独编译。
- 计划
    - BSP裁剪 
    - 流程文档整理