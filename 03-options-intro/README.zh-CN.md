[English](./README.md) | **中文**

# 03 | 期权入门

> 期权是杠杆工具，可以用小钱控制大仓位——但双刃剑会切到自己

---

## ⚠️ 重要警告

**期权交易复杂，新手务必：**
1. 先在模拟账户练习至少1个月
2. 只用你能接受损失100%的资金
3. 从最简单的策略（买Call/Put）开始

---

## 3.1 期权是什么？

期权是一种**合约**，给你**权利（不是义务）**在特定时间以特定价格买卖股票。

**类比：**
你交了1万元定金，锁定3个月后以100万购买某套房。
- 如果3个月后房价涨到150万 → 你执行权利，赚50万
- 如果3个月后房价跌到80万 → 你放弃权利，只损失1万定金

**官方教育资源：**
- [OCC Options Education（期权结算公司，最权威）](https://www.optionseducation.org)
- [CBOE Options Institute](https://www.cboe.com/education/)
- [Investopedia: Options Basics](https://www.investopedia.com/options-basics-tutorial-4583012)

---

## 3.2 两种基本期权

### Call Option（看涨期权）
- **买Call** = 花小钱赌股价上涨，最多亏权利金
- **卖Call** = 收权利金，但涨太多会亏损

### Put Option（看跌期权）
- **买Put** = 花小钱赌股价下跌，最多亏权利金
- **卖Put** = 收权利金，但跌太多会亏损

```
方向预测 → 涨 → 买 Call
          → 跌 → 买 Put

收入策略 → 股价不动或小涨 → 卖 Call（Covered Call）
          → 股价不动或小跌 → 卖 Put（Cash Secured Put）
```

---

## 3.3 期权合约要素

以 `AAPL 250117C00190000` 为例解读：

| 要素 | 值 | 说明 |
|------|-----|------|
| 标的 | AAPL | 苹果股票 |
| 到期日 | 250117 | 2025年1月17日 |
| 类型 | C | Call（看涨） |
| 行权价 | 190 | Strike Price |
| 权利金 | ~$5.20 | 你付的"保险费"（×100） |

**关键点：** 1份合约 = 100股，所以付$5.20实际花 **$520**

---

## 3.4 价值内外分析（Moneyness）

| 状态 | 英文 | Call情况 | Put情况 |
|------|------|----------|---------|
| 实值 | In-the-Money (ITM) | 股价>行权价 | 股价<行权价 |
| 平值 | At-the-Money (ATM) | 股价≈行权价 | 股价≈行权价 |
| 虚值 | Out-of-the-Money (OTM) | 股价<行权价 | 股价>行权价 |

**新手建议：** 买ITM或ATM的期权，成功概率更高

---

## 3.5 希腊字母（Greeks）——期权定价的核心

| 希腊字母 | 含义 | 一句话解释 |
|----------|------|-----------|
| **Delta (Δ)** | 股价变动1元，期权价格变动多少 | 最重要！ITM call约0.5-0.9 |
| **Theta (Θ)** | 每天时间损耗 | 对买方不利，期权每天贬值 |
| **Vega (V)** | 波动率变化1%的影响 | 不确定性越大期权越贵 |
| **Gamma (Γ)** | Delta的变化率 | 到期前加速变化 |
| **Rho (ρ)** | 利率变化的影响 | 通常影响较小 |

**深度学习：**
- [Options Greeks Explained（英文视频）](https://www.youtube.com/watch?v=kCJcEOFuuZk)
- [Tastytrade Greeks教程](https://tastytrade.com/learn/options-greeks/)

---

## 3.6 期权定价——Black-Scholes模型

影响期权价格的6个因素：

```
期权价格 ↑ 当：
  ✓ 标的价格↑（Call）/ 标的价格↓（Put）
  ✓ 距到期日更远（时间价值↑）
  ✓ 隐含波动率（IV）↑
  ✓ 无风险利率↑（Call受益）
```

**IV（隐含波动率）是关键：**
- IV高 = 期权贵，市场预期大幅波动（财报前）
- IV低 = 期权便宜，市场平静

查看IV工具：[Market Chameleon](https://marketchameleon.com) | [Barchart Options](https://www.barchart.com/options)

---

## 3.7 新手友好策略

### 策略一：买Call（方向性押注）
```
场景：你认为AAPL会在1个月内上涨
操作：买1份 AAPL ATM Call，到期1个月
风险：最多亏权利金（例如$500）
回报：不设上限
```

### 策略二：买Put（看跌或对冲）
```
场景：你认为市场会下跌，或你已持有股票想对冲
操作：买SPY Put
风险：最多亏权利金
回报：股价越跌赚越多
```

### 策略三：Covered Call（持股增收）
```
场景：你已持有100股AAPL，不准备近期卖出
操作：卖出1份OTM Call，收取权利金
风险：股票被以行权价强制卖出
回报：每月稳定收权利金（月化1-3%）
```

### 策略四：Cash Secured Put（低买股票）
```
场景：你想以更低价格买入AAPL
操作：卖出1份OTM Put，账户备足资金
风险：股价暴跌超出预期
回报：收权利金；若跌破行权价则以理想价买入股票
```

**策略学习平台：**
- [Tastytrade（最好的期权教育平台）](https://tastytrade.com/learn/)
- [Options Playbook](https://www.optionsplaybook.com)
- [Investopedia期权策略](https://www.investopedia.com/trading/options-strategies/)

---

## 3.8 期权交易平台

| 平台 | 特点 | 适合 |
|------|------|------|
| [Thinkorswim (TD/Schwab)](https://www.tdameritrade.com/tools-and-platforms/thinkorswim.html) | 最专业，有纸盘 | 认真学习者 |
| [Tastytrade](https://tastytrade.com) | 专为期权设计，界面简洁 | 期权专用 |
| [IBKR](https://www.interactivebrokers.com) | 专业级，费用低 | 进阶用户 |
| [Robinhood](https://robinhood.com) | 简单，免佣金 | 入门 |

---

## 3.9 期权风险矩阵

| 操作 | 最大亏损 | 最大盈利 | 新手适合？ |
|------|----------|----------|-----------|
| 买Call | 权利金 | 无限 | ✅ 适合 |
| 买Put | 权利金 | 股价-0 | ✅ 适合 |
| 卖Covered Call | 股票被卖出 | 权利金 | ✅ 适合 |
| 卖Cash Secured Put | 行权价-0 | 权利金 | ✅ 适合 |
| 卖Naked Call | **无限！** | 权利金 | ❌ 危险！ |
| 卖Naked Put | 行权价 | 权利金 | ⚠️ 谨慎 |

---

## ✅ 本章检验

- [ ] 能解释Call和Put的区别
- [ ] 知道Delta代表什么
- [ ] 在模拟账户买过一次Call期权
- [ ] 能计算一个期权合约的最大亏损

**下一章：** [08-trading-strategies →](../08-trading-strategies/README.zh-CN.md)
