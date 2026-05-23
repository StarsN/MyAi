---
kol: "@CryptoRounder"
type: DataSource
updated: 2026-05-23
---

# CryptoRounder 数据源

## 一、交易所与交易平台

### OKX（主力平台）
- **图表分析工具**：免费，布林带 + ATR 一键添加
- **期权交易**：支持 RFQ 询价、多腿策略、API 自动执行
- **金融日历**：宏观事件驱动交易（FOMC、CPI、NFP 等）
- **OKX 账户**：ETH 为主要持仓资产，用作期权保证金

### GreeksLive
- **OKX 期权 RFQ**：最小询价门槛 $50,000
- **T 型报价表**：期权价格（币本位+美元）、权利金年化 APR
- **多腿策略**：Iron Condor、Bull-Bear Spread 一键构建

## 二、技术分析工具

### 核心指标
| 工具 | 用途 | 来源 |
|------|------|------|
| 布林带 (Bollinger Bands) | 震荡区间 + 超买超卖 | OKX / TradingView |
| ATR | 波动率，插针范围 | OKX / TradingView |
| MACD 周线 | 大趋势方向 | TradingView |
| VPVR POC | 密集成交区 | TradingView |
| ASR-VC 4h | 震荡支撑/阻力 | @cryptopainter 付费指标 |
| 200 日 SMA | 长期趋势线 | TradingView |

### TradingView
- 社区脚本（全球 M2 指标）
- 自定义图表
- 多时间框架分析

## 三、宏观数据

### 流动性数据
- **全球 M2 货币供应**：TradingView 社区脚本，前移 90 天对比 BTC
- **央行政策**：美联储利率决议、欧洲央行、日本央行

### 估值指标
- **巴菲特指标**（美股总市值/GDP）：> 200% = 高估警告
- **伯克希尔现金储备**：作为市场恐慌/贪婪的代理指标

### 经济日历
- **OKX 金融日历**：事件驱动期权策略（利率决议、CPI 等）
- 双买期权策略（重大事件前同时买 Call + Put）

## 四、预测市场

### Polymarket
- 实时概率定价
- 事件驱动交易信号
- 选举、政策、体育、流行文化

## 五、信息来源

### KOL 与社区
- @cryptopainter（画师）：ASR-VC 指标
- @CryptoRounder（自身）：每日 BTC 分析
- TradingView 社区：M2 指标开发者

### 自有框架
- 宏观 → 技术 → 期权的三层过滤体系
- OKX 金融日历 + Polymarket 双事件源
