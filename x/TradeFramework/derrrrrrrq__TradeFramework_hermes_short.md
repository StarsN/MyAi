# derrrrrrrq · Wyckoff结构+多空挤压 [Hermes蒸馏版]

> 定位: 区分主力OI vs 散户OI,识别多空挤压(爆仓)机会
> 源: 2,437字 → 蒸馏: ~480字 | 压缩率 80%

## 主力vs散户分歧
L1  主力建仓: 大户多+散户空 | top_lsr>1.5 & lsr<0.7
S1  主力派发: 大户空+散户多 | top_lsr<0.7 & lsr>1.5

## 挤压信号(高赔率)
L2  多头挤压→反转做多: 散户极度看空→爆空后跟多 | lsr<0.3 & funding<-0.03%
S2  空头挤压→反转做空: 散户极度看多→爆多后跟空 | lsr>3 & funding>0.06%

## 杀猪盘检测(核心否决)
X1  盘口极浅+OI双向都大 → 多空双杀,远离 | (depth_bid+depth_ask<200K) & oi_usd>5M
X2  价差异常宽 → MM不在 | spread>0.5%
X3  刷量假币: vol/OI极高+盘口浅 | vol_oi>15 & depth_bid<100K
X4  Wyckoff派发确认: OI+价格同时见顶后回落 → 主力已走 | oi_1h<-5% & ch_1h<-3%

## 核心原则
- 过滤90%的机会;确定性高才上仓位;止损基于主力OI均价
- 判断Wyckoff阶段: 吸筹(SC→AR→ST→SOS)做多,派发(PSY→BC→SOW→LPSY)做空
- 区分"主力构建的OI"vs"散户follow的OI": 大户多+散户空=健康;反之警惕

## ⚠️ KOL间冲突
- vs Arya: lsr<0.4做多→一致;但derrrrrrrq额外要求确认不是杀猪盘(深度+价差过滤)
- Wyckoff阶段判断无法从38维数据直接读取,需要K线形态辅助(本数据不提供)
