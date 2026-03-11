[English](./README.md) | **中文**

# 04 | 技术分析

> 技术分析研究"价格行为"——市场已知的一切都反映在价格上

---

## 4.1 K线图（蜡烛图）基础

K线是技术分析的语言，必须掌握。

```
          │  ← 上影线（最高价）
        ┌─┴─┐
        │   │  ← 实体（开盘-收盘）
        │   │     绿/白 = 收盘>开盘（上涨）
        └─┬─┘     红/黑 = 收盘<开盘（下跌）
          │  ← 下影线（最低价）
```

### 重要K线形态

| 形态 | 含义 | 信号 |
|------|------|------|
| 锤子线 | 下影线很长，实体小 | 底部反转信号 |
| 射击之星 | 上影线很长，实体小 | 顶部反转信号 |
| 十字星 | 开收盘接近，上下影线 | 犹豫，趋势可能转变 |
| 吞没形态 | 大实体包住小实体 | 强烈反转信号 |
| 三白兵/三黑鸦 | 连续三根同色K线 | 强趋势延续 |

**K线学习：**
- [Investopedia蜡烛图图解](https://www.investopedia.com/trading/candlestick-charting-what-is-it/)
- [TradingView图表（免费）](https://www.tradingview.com/chart/)
- [StockCharts图表教育](https://school.stockcharts.com)

---

## 4.2 移动平均线（MA）

移动平均线平滑价格波动，显示趋势方向。

| 均线 | 周期 | 用途 |
|------|------|------|
| MA20 | 20日 | 短期趋势，日内支撑 |
| MA50 | 50日 | 中期趋势，机构关注 |
| MA200 | 200日 | 长期趋势，牛熊分界线 |

### 黄金交叉 vs 死亡交叉
```
黄金交叉（Golden Cross）：MA50 上穿 MA200 → 看涨信号 📈
死亡交叉（Death Cross）：MA50 下穿 MA200 → 看跌信号 📉
```

### EMA vs SMA
- **SMA（简单移动平均）**：权重相同
- **EMA（指数移动平均）**：近期价格权重更高，反应更快

---

## 4.3 RSI（相对强弱指数）

RSI衡量价格变动的速度和幅度，范围0-100。

```
RSI > 70 → 超买区域（可能回调）
RSI = 50 → 中性
RSI < 30 → 超卖区域（可能反弹）
```

**使用技巧：**
- 不要单独使用RSI，结合价格行为
- 强趋势中RSI可以长时间维持在70以上
- 寻找**背离（Divergence）**：价格新高但RSI不创新高 = 警告信号

---

## 4.4 MACD（移动平均收敛散度）

MACD = EMA12 - EMA26，反映趋势动量。

```
MACD线 穿越 信号线（向上）→ 买入信号
MACD线 穿越 信号线（向下）→ 卖出信号
柱状图（Histogram）变大 → 趋势增强
柱状图（Histogram）缩小 → 趋势减弱
```

**深度学习：**
- [Investopedia MACD](https://www.investopedia.com/terms/m/macd.asp)

---

## 4.5 布林带（Bollinger Bands）

布林带 = MA20 ± 2倍标准差

```
价格触碰上轨 → 可能超买，考虑卖出
价格触碰下轨 → 可能超卖，考虑买入
布林带收窄   → 波动率降低，大行情将至
布林带扩张   → 波动率增加，趋势确认
```

---

## 4.6 支撑与阻力

这是技术分析最核心的概念：

```
阻力位（Resistance）：价格难以突破的上方区域
支撑位（Support）：价格难以跌破的下方区域

规律：突破阻力位后，阻力位变支撑位
      跌破支撑位后，支撑位变阻力位
```

**找支撑阻力的方法：**
- 历史价格的多次触碰点
- 整数关口（$100, $150, $200）
- 均线（MA50, MA200）
- 前期高点/低点

---

## 4.7 成交量分析

**黄金法则：**
```
价涨量增 → 趋势健康，可信度高 ✅
价涨量缩 → 上涨乏力，注意反转 ⚠️
价跌量增 → 抛压大，趋势可能持续 ⚠️
价跌量缩 → 跌势减弱，可能企稳 ✅
```

---

## 4.8 图表形态

### 反转形态
| 形态 | 信号 | 学习链接 |
|------|------|---------|
| 头肩顶/底 | 最可靠的反转形态 | [Investopedia](https://www.investopedia.com/terms/h/head-shoulders.asp) |
| 双顶/双底（M/W顶底） | 常见反转 | [StockCharts](https://school.stockcharts.com/doku.php?id=chart_analysis:chart_patterns:double_top_reversal) |

### 持续形态
| 形态 | 信号 | 学习链接 |
|------|------|---------|
| 旗形/楔形 | 趋势中的整理 | [Investopedia](https://www.investopedia.com/terms/f/flag.asp) |
| 三角形（上升/下降/对称） | 蓄势待发 | [StockCharts](https://school.stockcharts.com/doku.php?id=chart_analysis:chart_patterns:symmetrical_triangle) |
| 杯柄形态 | 中长线强势形态 | [Investors.com](https://www.investors.com/ibd-university/how-to-buy/bases-overview-1/) |

---

## 4.9 技术分析工具推荐

| 工具 | 链接 | 费用 | 特点 |
|------|------|------|------|
| TradingView | [tradingview.com](https://www.tradingview.com) | 免费/付费 | 最好用的图表工具 |
| StockCharts | [stockcharts.com](https://stockcharts.com) | 付费 | 教育资源丰富 |
| Finviz | [finviz.com](https://finviz.com) | 免费/付费 | 热力图和筛选器 |
| 同花顺 | [10jqka.com.cn](http://www.10jqka.com.cn) | 免费 | A股最好用 |

---

## ✅ 本章检验

- [ ] 能识别锤子线和射击之星
- [ ] 知道RSI>70意味着什么
- [ ] 在TradingView上添加了MA50和MACD指标
- [ ] 找到一支股票的支撑和阻力位

**下一章：** [05-fundamental-analysis →](../05-fundamental-analysis/README.zh-CN.md)
