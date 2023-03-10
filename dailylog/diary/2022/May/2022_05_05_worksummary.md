
# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态   | 投入时间 |
| -- | -- | ---- | -----| ------ | -------- |
| E34R静电检测 | 中| ７０%  |验证后输出测试固件| 解决中 |２D|
| 大鹏：ESD验证| 中 | ６０%  |配合龙迅验证固件修改| 解决中| １.５Ｄ|
|DPVR_CAM功耗优化需求评估| 中 | ６０%  |低功耗流程梳理优化测试| 验证完成| 4Ｄ|
| junkeV2：时间戳问题修改| 中 | ６０%  |修改内核获取基准时间| 解决中| 3H|
| E34R：亮度调节功能修改| 中 | ６０%  |检查环境光改变后３ｓ才改变亮度| 解决中| 3H|


# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
| 大鹏：DPVR_CAM功耗 | 中| ７０%  |测试，代码合并| 解决中 |１D|
|  E34R ：亮度调节，ＥＳＤ| 中| ７０%  |代码合并| 解决中 |１D|
| ＥＳＰ光机 | 低 | ５%  | 等待硬件| 待解决| ５Ｄ  |
| usb 2.0 3.0  判断问题| 低 | ５%  | type-C&A识别优化和接845box热插拔出现异常| 待解决| ５Ｄ  |

# 挂起任务
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
| ＥＳＰ光机 | 低 | ５%  | 使用新的光机，验证眼镜功能．| 待解决| ５Ｄ  |
| ＯＳＡＫ０９９１８摄像头调试 | 低 | ５%  |  解决无法读取数据问题，剩余业务代码| 待解决| ５Ｄ  |
| oppo项目 | 低 | ５%  | 7911uxc代码合入ｂｒａｎｃｈ分支| 待解决| ５Ｄ  |
| 框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | １０D|
| RK平台开发| 中 | ６%  |内核裁剪与裁剪| 解决中| ２Ｄ|
| BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 |２D|

# 任务说明：
## 【缺陷】
【缺陷】<font color='red'> 【中优先级】  </font>E34R静电检测
- 进展：重新优化逻辑
    -　静电复位，亮度不需要缓慢调节．
    -　按照ＥＰＳＯＮ　答复，去掉了复位中的ｓｌｅｅｐ过程．输出固件．
    - 上次周报答复的２～３Ｓ是因为，复位的亮度调节是缓慢调节．现在改为直接是上次的值．　  
- 计划：
　　　- 当前输出两个版本，一个是之前正常的版本，一个后面ＳＰＳＯＮ答复去掉两个版本．
　　　- 目前复位时间最短１～２Ｓ．
　　　- 等待硬件测试报告．

【缺陷】<font color='red'> 【中优先级】  </font>type-C&A识别优化和接845box热插拔出现异常
- 进展：当前在epson 平台，２.0 和　３.0 标志存在有误，导致逻辑结果存在误判，需要定位。
- 计划：
　　　- 在ｄｅｍｏｋｉｔ版本上，原来的逻辑正常，有概率会失败．
　　　- 还有继续跟踪ｕｓｂ驱动。
  
【缺陷】<font color='red'> 【中优先级】  </font>junkeV2：时间戳问题修改
- 问题：ｂｏｘ驱动，同步的时间使用的ＣＬＯＣＫ＿ＭＯＮ０ＴＩＣ时间，这个时间不会计算休眠时间．
- 进展
　　　- 在ｄｅｍｏｋｉｔ版本上，原来的逻辑正常，有概率会失败．
　　　- 还有继续跟踪ＵＳＢ驱动。
　　　- 
【缺陷】<font color='red'> 【中优先级】  </font>DPVR_CAM功耗优化需求评估
- 问题：梳理了原来的ＬＰ逻辑，当前在大鹏项目，增加浅睡和深睡．屏幕和ａｕｄｉｏ深睡时，不涉及ｃｐｕ和ｕｓｂ睡眠，不需要做ＡＰＰ＿ＰＭ睡眠．
- 计划
    - 摘下头套后，５ｓ后进入浅睡，３０ｓ后进入深睡．（实际测试中３０ｓ有点短）
　　　- 不放开ＣＰＵ和ＵＳＢ休眠逻辑，合入大鹏项目．
　　　- 测试ｃｐｕ和ｕｓｂ睡眠逻辑。
