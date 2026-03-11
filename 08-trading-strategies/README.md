**English** | [中文](./README.zh-CN.md)

# 08 | Trading Strategies

> Quality over quantity. Mastering one or two strategies beats knowing ten mediocre ones.

---

## 8.1 Strategy Selection Matrix

```
By capital:
  $1,000–$10,000  → Index DCA + small individual positions
  $10,000+        → Individual stocks + simple options strategies
  $50,000+        → Full options strategy portfolio

By time available:
  <1 hr/week      → Index ETF dollar-cost averaging
  1–5 hrs/week    → Trend investing + Covered Call
  1–2 hrs/day     → Active stock picking + options strategies
  Full-time       → Swing trading + complex options
```

---

## Strategy 1: Index Dollar-Cost Averaging (Best for Beginners)

**Core Logic:** Don't try to beat the market — grow with it

```
How it works:
  On a fixed date each month, invest a fixed amount in VOO or SPY
  Stay disciplined regardless of market direction (DCA strategy)

Historical validation:
  S&P 500 annualized return since 1950: ~10.7%
  $10,000/year for 30 years → approximately $1,800,000
```

**Best For:** Passive investors, long-term investors, complete beginners

**Learning Resources:**
- [Vanguard DCA Calculator](https://investor.vanguard.com/tools-and-calculators/dollar-cost-averaging)
- [JL Collins - Simple Path to Wealth](https://jlcollinsnh.com/stock-series/)

---

## Strategy 2: Trend Following (Intermediate)

**Core Logic:** Go with the trend — don't try to predict turning points

```
Entry Conditions (ALL must be met):
  ✓ Price is above both MA50 and MA200
  ✓ MA50 > MA200 (golden cross or already above)
  ✓ Volume expands on breakout above resistance
  ✓ RSI between 40–70 (not overbought)

Exit Conditions (ANY one triggers):
  ✗ Stop loss is hit
  ✗ Price breaks below MA50 (optional, looser version)
  ✗ Target price reached (2R or more)
```

**Recommended Learning:**
- [Minervini Trend Template](https://www.markminervini.com)
- [William O'Neil CANSLIM Method](https://www.investors.com/ibd-university/)

---

## Strategy 3: Covered Call (Generating Income from Holdings)

**Core Logic:** Already holding stock; sell OTM Calls each month to collect premium

```
Scenario: Hold 100 shares AAPL @ $185
Action: Sell 1 AAPL Call expiring in 30 days at $195 strike, collect $2.50 premium ($250)
Outcome:
  Price stays below $195 → Keep $250 premium (1.35% monthly)
  Price exceeds $195     → Shares called away at $195 (effectively sold at a premium)

Annualized premium yield: ~12–18%
```

**Risk:** Missing out on a large rally; still holding shares if price drops sharply

**Best Market Environment:** Sideways / choppy market, large-cap holdings

---

## Strategy 4: Cash Secured Put (Buying Stock at a Discount)

**Core Logic:** Want to buy a stock but think it's slightly overpriced — sell a Put to wait

```
Scenario: Want to buy AAPL at $180 (current price $185)
Action: Sell 1 AAPL $180 Put expiring in 30 days, collect $3.00 premium ($300)
        Keep $18,000 cash in account as collateral
Outcome:
  AAPL > $180 at expiration → Keep $300 premium, continue waiting
  AAPL < $180 at expiration → Buy 100 shares at $180 (effective cost $177)

Annualized premium yield: ~10–15%
```

**Best Use Case:** When you genuinely want to own the stock at that price

---

## Strategy 5: Bull Call Spread (Bullish Debit Spread)

**Core Logic:** Buy a low-strike Call, sell a high-strike Call to reduce premium cost

```
Scenario: Bullish on AAPL but don't want to pay full premium
Action:
  Buy  AAPL $185 Call @ $6.00
  Sell AAPL $195 Call @ $2.50
  Net cost = $3.50 ($350/contract)

Max profit: ($195 − $185) − $3.50 = $6.50 ($650/contract)
Max loss:   $3.50 ($350/contract)
Risk/Reward ratio: 1:1.86

Trigger: AAPL > $195 at expiration
```

**P&L Visualizer:** [Options Profit Calculator](https://www.optionsprofitcalculator.com/calculator/bull-call-spread.html)

---

## Strategy 6: Protective Put (Portfolio Insurance)

**Core Logic:** Hold stock + buy Put to limit downside risk

```
Scenario: Hold 100 shares SPY, concerned about a market drop
Action: Buy SPY Put with strike 5%–10% below current price
Cost: ~1–3% of portfolio value per year (insurance premium)
Effect: If market drops >10%, Put gains offset losses
```

---

## Strategy 7: Earnings Trading (High Risk — For Reference Only)

**Principle:** Options IV spikes before earnings, then collapses after (IV Crush)

```
Aggressive approach (buying options):
  Bet on direction before earnings — but IV crush can cause losses
  Even if your direction is right, you can still lose money!

Conservative approach (selling options):
  Sell a Short Straddle — bet that post-earnings move is small
  Only suitable for traders familiar with options Greeks
```

**Tool:** [Market Chameleon Earnings Stats](https://marketchameleon.com/Reports/Earnings)

---

## 8.2 Strategy by Market Environment

| Market Condition | Characteristics | Recommended Strategy |
|-----------------|-----------------|---------------------|
| Strong Bull | VIX < 15, uptrend | Trend following, buy Calls |
| Sideways | VIX 15–25 | Covered Call, Cash Secured Put |
| High Volatility | VIX > 25 | Reduce exposure, buy Protective Puts |
| Bear Market | Sustained decline | Cash is king, buy Puts for hedge |

**VIX:** [CBOE VIX](https://www.cboe.com/tradable_products/vix/)

---

## 8.3 Building a Complete Trading System

A complete trading system includes:

```
1. Stock Selection Criteria (What to trade)
   └── Fundamental filter + technical confirmation

2. Entry Conditions (When to enter)
   └── Specific technical signal

3. Position Size (How much)
   └── 1–2% risk rule

4. Stop Loss (Where to exit if wrong)
   └── Technical support level or fixed %

5. Target Price (Where to exit if right)
   └── 2R–3R target

6. Management Rules (How to manage)
   └── When to add? When to move stop?

7. Review Process (How to improve)
   └── Weekly review of trading journal
```

---

## ✅ Chapter Checklist

- [ ] Have chosen 1–2 strategies that fit your profile
- [ ] Executed a complete trade in a paper account (entry to exit)
- [ ] Recorded a complete trading journal entry

**Last Chapter:** [09 - Learning Resources →](../09-learning-resources/README.md)
