# derrrrrrrq 数据源

> 时间跨度: 2024.04 – 2026.05 | 来源: 507 篇 X 帖子

---

## 一级数据源：自建平台
derrrrrrrq 自己搭建了底层数据平台，接入 8 个 AI 服务，日均百万级数据流入流出。以下是可推断使用的数据维度：

| 维度 | 来源/工具 | 用途 |
|------|----------|------|
| 合约 OI + 多空比 | 交易所 API（Binance/OKX/Bybit） | 主力 OI vs 散户 OI 区分 |
| 合约清算数据 | 交易所 API + Coinglass | 挤压时机判断 |
| 链上持仓变化 | 链上浏览器 + Alchemy API | 筹码健康度 |
| 交易所地址追踪 | 链上浏览器 | 充值/提现/出货检测 |
| 订单簿深度 | 交易所 WebSocket | 真实供需方向 |
| Smart Money 盈亏 | OKX/Dune 链上数据 | 聪明钱行为验证 |
| 合约盘口流动性 | 交易所 WebSocket | 杀猪盘识别 |
| 历史 K 线 | 交易所 API | Wyckoff 形态识别 |
| DEX 流动性池 | 链上数据 | 链上筹码分布 |

## 二级数据源：公开工具

| 工具 | 用途 |
|------|------|
| **TradingView** | K 线图表、Wyckoff 形态标注 |
| **Coinglass** | 合约清算数据、OI 变化 |
| **DefiLlama** | TVL、DEX 流动性 |
| **Dune Analytics** | 自定义链上查询 |
| **Alchemy** | 链上数据 API |
| **Allium** | 链上数据聚合 |
| **DEX Screener** | DEX 实时价格和交易量 |
| **Etherscan/Solscan** | 地址追踪、持仓变化 |

## 三级数据源：信息与社区

| 来源 | 用途 |
|------|------|
| **X/Twitter** | 市场情绪、KOL 观点交叉验证 |
| **Discord 社区** | 项目一手信息 |
| **GitHub** | 项目代码活跃度（QUIL 等） |

## 关键数据监控指标
1. **主力 OI 均价** vs 当前价格 → 主力盈亏状态
2. **多头 follow OI 累积量** → 洗盘概率
3. **交易所冷钱包充值量** → 主力出货信号
4. **SC 处的量价关系** → 吸筹确认
5. **Order book imbalance** → 短期方向
6. **合约盘口滑点** → 流动性健康度
