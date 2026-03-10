**English** | [中文](./README.zh-CN.md)

# 03 | Options Fundamentals

> Options are leveraged instruments — they let you control large positions with small capital. But the double-edged sword cuts both ways.

---

## ⚠️ Important Warning

**Options trading is complex. Beginners must:**
1. Practice in a paper trading account for at least 1 month
2. Only use capital you can afford to lose 100%
3. Start with the simplest strategies (buying Calls/Puts)

---

## 3.1 What Is an Option?

An option is a **contract** that gives you the **right (not obligation)** to buy or sell a stock at a specific price by a specific date.

**Analogy:**
You pay a $10,000 deposit to lock in the right to buy a house for $1,000,000 within 3 months.
- If the house is worth $1,500,000 in 3 months → you exercise your right and profit $500,000
- If the house drops to $800,000 → you walk away, losing only your $10,000 deposit

**Official Educational Resources:**
- [OCC Options Education (most authoritative)](https://www.optionseducation.org)
- [CBOE Options Institute](https://www.cboe.com/education/)
- [Investopedia: Options Basics](https://www.investopedia.com/options-basics-tutorial-4583012)

---

## 3.2 Two Basic Option Types

### Call Option
- **Buying a Call** = Pay a small premium to bet on a rising stock price; max loss = premium paid
- **Selling a Call** = Collect premium, but risk losses if the stock rises sharply

### Put Option
- **Buying a Put** = Pay a small premium to bet on a falling stock price; max loss = premium paid
- **Selling a Put** = Collect premium, but risk losses if the stock falls sharply

```
Directional bets:
  Bullish → Buy Call
  Bearish → Buy Put

Income strategies:
  Stock stays flat or rises modestly → Sell Call (Covered Call)
  Stock stays flat or falls modestly → Sell Put (Cash Secured Put)
```

---

## 3.3 Option Contract Components

Reading `AAPL 250117C00190000`:

| Component | Value | Description |
|-----------|-------|-------------|
| Underlying | AAPL | Apple stock |
| Expiration | 250117 | January 17, 2025 |
| Type | C | Call (bullish) |
| Strike Price | 190 | Your right to buy at $190 |
| Premium | ~$5.20 | What you pay (×100 per contract) |

**Key Point:** 1 contract = 100 shares, so paying $5.20 means actually spending **$520**

---

## 3.4 Moneyness

| Status | Term | Call Condition | Put Condition |
|--------|------|----------------|---------------|
| In the money | ITM | Stock price > Strike | Stock price < Strike |
| At the money | ATM | Stock price ≈ Strike | Stock price ≈ Strike |
| Out of the money | OTM | Stock price < Strike | Stock price > Strike |

**Beginner Tip:** Buy ITM or ATM options — higher probability of profit

---

## 3.5 The Greeks — The Core of Options Pricing

| Greek | Meaning | Plain English |
|-------|---------|---------------|
| **Delta (Δ)** | Change in option price per $1 move in stock | Most important! ITM call ≈ 0.5–0.9 |
| **Theta (Θ)** | Daily time decay | Works against buyers — options lose value each day |
| **Vega (V)** | Impact of 1% change in volatility | Higher uncertainty = more expensive options |
| **Gamma (Γ)** | Rate of change in Delta | Accelerates near expiration |
| **Rho (ρ)** | Impact of interest rate changes | Usually small |

**Deep Learning:**
- [Options Greeks Explained (Video)](https://www.youtube.com/watch?v=kCJcEOFuuZk)
- [Tastytrade Greeks Tutorial](https://tastytrade.com/learn/options-greeks/)

---

## 3.6 Options Pricing — The Black-Scholes Model

Six factors that affect options pricing:

```
Option price RISES when:
  ✓ Underlying price rises (Call) / falls (Put)
  ✓ More time until expiration (more time value)
  ✓ Implied Volatility (IV) rises
  ✓ Risk-free interest rate rises (benefits Calls)
```

**IV (Implied Volatility) is critical:**
- High IV = expensive options; market expects big moves (e.g., before earnings)
- Low IV = cheap options; market is calm

Check IV: [Market Chameleon](https://marketchameleon.com) | [Barchart Options](https://www.barchart.com/options)

---

## 3.7 Beginner-Friendly Strategies

### Strategy 1: Buy a Call (Directional Bet)
```
Scenario: You believe AAPL will rise within 1 month
Action: Buy 1 AAPL ATM Call, expiring in 1 month
Max Loss: Premium paid (e.g., $500)
Max Profit: Unlimited
```

### Strategy 2: Buy a Put (Bearish or Hedge)
```
Scenario: You expect the market to fall, or you hold stocks and want protection
Action: Buy SPY Put
Max Loss: Premium paid
Max Profit: Increases as price falls
```

### Strategy 3: Covered Call (Income on Existing Holdings)
```
Scenario: You hold 100 shares of AAPL and don't plan to sell soon
Action: Sell 1 OTM Call, collect premium
Risk: Shares may be called away at strike price
Reward: Steady monthly premium income (1–3% monthly)
```

### Strategy 4: Cash Secured Put (Buy Stock at a Discount)
```
Scenario: You want to buy AAPL at a lower price
Action: Sell 1 OTM Put, keep enough cash in account to cover assignment
Risk: Stock drops sharply below strike price
Reward: Collect premium; if assigned, you buy at your target price
```

**Strategy Learning:**
- [Tastytrade (best options education platform)](https://tastytrade.com/learn/)
- [Options Playbook](https://www.optionsplaybook.com)
- [Investopedia Options Strategies](https://www.investopedia.com/trading/options-strategies/)

---

## 3.8 Options Trading Platforms

| Platform | Highlights | Best For |
|----------|-----------|---------|
| [Thinkorswim (TD/Schwab)](https://www.tdameritrade.com/tools-and-platforms/thinkorswim.html) | Most professional, paper trading | Serious learners |
| [Tastytrade](https://tastytrade.com) | Built for options, clean UI | Options-focused traders |
| [IBKR](https://www.interactivebrokers.com) | Professional-grade, low fees | Advanced users |
| [Robinhood](https://robinhood.com) | Simple, commission-free | Beginners |

---

## 3.9 Options Risk Matrix

| Action | Max Loss | Max Profit | Beginner-Friendly? |
|--------|----------|------------|--------------------|
| Buy Call | Premium paid | Unlimited | ✅ Yes |
| Buy Put | Premium paid | Stock price − $0 | ✅ Yes |
| Sell Covered Call | Stock called away | Premium | ✅ Yes |
| Sell Cash Secured Put | Strike price − $0 | Premium | ✅ Yes |
| Sell Naked Call | **Unlimited!** | Premium | ❌ Dangerous! |
| Sell Naked Put | Strike price | Premium | ⚠️ Use caution |

---

## ✅ Chapter Checklist

- [ ] Can explain the difference between a Call and a Put
- [ ] Know what Delta represents
- [ ] Have bought a Call option in a paper trading account
- [ ] Can calculate the maximum loss on an options contract

**Next Chapter:** [08 - Trading Strategies →](../08-实战策略/README.md)
