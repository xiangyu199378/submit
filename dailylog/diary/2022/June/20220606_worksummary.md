
# 上周投入
| 任务| 优先级 | 进度 | 问题| 状态   | 投入时间 |
| -- | -- | ---- | -----| ------ | -------- |
|大棚背光灯| 中 |１０%  |协助解决产线问题| 解决中|２Ｄ|
|E34R| 中 | ７０%  |修复光机点亮问题和新ＨＩＤ命令| 待合并代码|１Ｄ|
|大棚ＫＥＹ| 中 |１００%  |协助解决问题| 完成|2H|
|大鹏ＥＱ|低| ６０%  |完成固件输出| 等待第三方反馈|0.5Ｄ|

# 本周计划
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
|大棚| 中 | ７０%  |新增亮度，呼吸灯模式，频率设置| 解决中| １.5Ｄ|
|E34R| 中 | ７０%  |提交问题修改代码| 解决中| １.5Ｄ|
|大棚| 中 | ７０%  |产线偶现无法识别点亮问题| 解决中| １.5Ｄ|


# 挂起任务
| 任务| 优先级 | 进度 | 问题| 状态|计划时间 |
|-----|-------| ---- | ---|----|--------|
| ＯＳＡＫ０９９１８摄像头调试 | 低 | ５%  |  解决无法读取数据问题，剩余业务代码| 待解决| ２Ｄ  |
| oppo项目 | 低 | ５%  | 7911uxc代码合入ｂｒａｎｃｈ分支| 待解决| ２Ｄ  |
| 框架优化 | 低 | 15%  | 输出一版细化，再次会议讨论结构体设计 | 待解决 | １０D|
| RK平台开发| 中 | ６%  |内核裁剪与裁剪| 解决中| ２Ｄ|
| BUG：DP信号问题 | 中| ７０%  | EPSON２.0,3.0判断条件判断条件存在问题，导致逻辑结果存在误判,后续需要需要验证下对版本号是否对ＤＰ是否有影响|解决中 |２D|
|ＥＰＳＯＮＢＢ| 中 | ７０%  |后续需要合入主分支，考虑兼容性| 解决中| １Ｄ|



# 任务说明：
## 【缺陷】
【缺陷】<font color='red'> 【中优先级】  </font>E34R静电检测
- 结论：
    -　优化后最短时间１最后有３％的概率 无法点亮为ＥＰＳＯＮ光机无法点亮．
- 计划：    
　　　- 单步ＨＩＤ命令，当出现问题后，单步查看每个步骤．

【缺陷】<font color='red'> 【中优先级】  </font>大鹏ＥＳＤ
- 结论：
    -　当前无法复现花屏问题．
- 计划：   
    - 增加状态点检测打印，合入分支．
    - 对于ＥＳＤ出现休眠无法唤醒，ＡＵＤＩＯ起不来问题，在测试问题性安排投入．
 

## 【开发任务】
  1.<font color='red'> 【高优先级】  </font>大棚产线
 - 进展：
    - 产线跟换背光灯，本地花费１天时间．
    - 其中出现ｕｓｂ模式切换重启，偶现屏幕无法正常点亮，端口无法通讯问题，
    - 增加debug flash 存储ｌｏｇ日志，获取到的日志，暂未分析到原因．
    - 产线问题反馈偶像无法点亮问题．
- 计划：
  - 同步产线和研发这边的环境．目前是徐兄和我这边都在提供固件，可能会存在ｂｏｏｌａｄｅｒ不一致的问题．
  - 分析概率性无法点亮问题．当前跟直显模式有关，因为通过在电脑里检测就可以正常识别．
  

２.<font color='red'> 【高优先级】  </font>ＥＳＰ光机显示开发
 - 进展：
    - 完成临时分支代码合入
- 计划：
  　- 后续等待合入主分支

３.<font color='red'> 【高优先级】  </font>新增亮度，呼吸灯模式，频率设置
 - 进展：
    - 未开始
- 计划：
  　- 梳理需求和设计
  　- 设置参数的同时需要生效．
