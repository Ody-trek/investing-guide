# 05 | 基本面分析

> 技术分析告诉你"何时买"，基本面分析告诉你"买什么"

---

## 5.1 三张核心财务报表

每家上市公司每季度必须公布：

### 损益表（Income Statement）
> 公司赚了多少钱？

```
营业收入（Revenue）
  - 营业成本（Cost of Revenue）
= 毛利润（Gross Profit）
  - 运营费用（Operating Expenses）
= 运营利润（Operating Income / EBIT）
  - 利息/税费
= 净利润（Net Income）
```

### 资产负债表（Balance Sheet）
> 公司有什么？欠什么？

```
资产（Assets）= 负债（Liabilities）+ 股东权益（Equity）

流动资产：现金、应收账款、库存
固定资产：厂房、设备、专利
流动负债：应付账款、短期债务
长期负债：长期贷款、债券
```

### 现金流量表（Cash Flow Statement）
> 公司真实的现金进出

```
经营活动现金流（Operating CF）← 最重要
投资活动现金流（Investing CF）
融资活动现金流（Financing CF）
```

**⚠️ 关键原则：** 净利润可以作假，但现金流更难造假

**财报查询：**
- [SEC EDGAR（美股官方财报）](https://www.sec.gov/cgi-bin/browse-edgar)
- [Macrotrends财报历史](https://www.macrotrends.net)
- [巨潮资讯（A股官方）](http://www.cninfo.com.cn)

---

## 5.2 估值方法

### 方法一：PE估值法（市盈率法）

```
合理股价 = 预期EPS × 合理P/E

例：苹果2025年预期EPS = $7.00
    行业平均P/E = 28x
    合理股价 = $7.00 × 28 = $196
```

**P/E参考（美股历史平均）：**
- 市场整体：15-20x
- 科技股：25-35x
- 高成长股：40x+
- 价值股：10-15x

### 方法二：DCF估值法（折现现金流）

> 公司的价值 = 未来所有现金流的现值之和

```
公司价值 = Σ [未来现金流 / (1+折现率)^年数]
```

这是最严谨但最复杂的方法。

**DCF计算器：**
- [Gurufocus DCF Calculator](https://www.gurufocus.com/term/dcf/AAPL/DCF-Calculator/Apple)
- [Simply Wall St（可视化）](https://simplywall.st)

### 方法三：PEG估值法

```
PEG = P/E ÷ 盈利增长率

PEG < 1 → 被低估
PEG = 1 → 合理
PEG > 1 → 可能被高估
```

---

## 5.3 关键财务健康指标

### 盈利能力
| 指标 | 公式 | 好的标准 |
|------|------|---------|
| 毛利率 | 毛利/收入 | 科技公司>50% |
| 净利率 | 净利润/收入 | >10%为佳 |
| ROE | 净利润/股东权益 | >15% |
| ROA | 净利润/总资产 | >5% |
| ROIC | NOPAT/投入资本 | >10% |

### 偿债能力
| 指标 | 公式 | 参考 |
|------|------|------|
| 流动比率 | 流动资产/流动负债 | >1.5为安全 |
| 速动比率 | (流动资产-库存)/流动负债 | >1为安全 |
| 负债权益比 | 总负债/股东权益 | 越低越好 |
| 利息覆盖率 | EBIT/利息费用 | >3倍为安全 |

### 成长性
| 指标 | 说明 |
|------|------|
| 收入增长率 YoY | 同比收入增长 |
| EPS增长率 | 每股收益增长 |
| 用户/订阅增长 | 科技公司的核心指标 |

---

## 5.4 行业分析框架

### 波特五力模型
```
          新进入者威胁
               ↕
供应商议价力 ←→ 行业竞争 ←→ 买家议价力
               ↕
          替代品威胁
```

### 护城河（Economic Moat）
巴菲特最看重的概念——公司的竞争壁垒：

| 护城河类型 | 例子 |
|-----------|------|
| 品牌价值 | 苹果、可口可乐 |
| 网络效应 | 微信、Facebook |
| 成本优势 | 亚马逊、沃尔玛 |
| 转换成本 | Salesforce、Adobe |
| 专利/许可 | 制药公司 |
| 规模经济 | 谷歌、微软 |

---

## 5.5 财报季日历

美股财报季（Earnings Season）：
- **Q1财报**：4月-5月
- **Q2财报**：7月-8月
- **Q3财报**：10月-11月
- **Q4/全年财报**：1月-2月

**财报日历工具：**
- [Earnings Whispers](https://www.earningswhispers.com)
- [Yahoo Finance Earnings Calendar](https://finance.yahoo.com/calendar/earnings)

---

## 5.6 分析师报告和评级

| 评级 | 含义 |
|------|------|
| Strong Buy / Overweight | 强烈看涨 |
| Buy | 看涨 |
| Hold / Neutral | 持有观望 |
| Sell / Underweight | 看跌 |
| Strong Sell | 强烈看跌 |

**免费分析师评级：**
- [TipRanks](https://www.tipranks.com)
- [Seeking Alpha](https://seekingalpha.com)
- [Benzinga](https://www.benzinga.com)

---

## 5.7 巴菲特的选股标准

> "用合理价格买入优秀公司，比用低廉价格买入普通公司要好得多"

1. 业务简单，能理解 (Business I Understand)
2. 持续的竞争优势 (Durable Competitive Advantage)
3. 能干诚实的管理层 (Capable and Honest Management)
4. 合理的估值 (Fair Price)

**学习巴菲特：**
- [Berkshire Hathaway股东信（免费）](https://www.berkshirehathaway.com/letters/letters.html)
- [《穷查理宝典》（芒格思维）](https://www.amazon.cn)

---

## ✅ 本章检验

- [ ] 能读懂一份损益表的基本结构
- [ ] 知道如何计算P/E
- [ ] 查看了AAPL最新一季财报
- [ ] 能解释什么是护城河

**下一章：** [06-风险管理 →](../06-风险管理/README.md)
