[English](./04-rebalancing.md) | [中文](./04-再平衡策略.md)

# Chapter 4: Rebalancing Strategy

> Rebalancing is the Permanent Portfolio's "maintenance routine." Executing it correctly is what keeps the strategy effective.

---

## What Is Rebalancing?

As each asset's price changes, the original 25/25/25/25 allocation drifts. **Rebalancing means adjusting the drifted allocations back to 25%.**

### Example

```
Initial state (start of 2023):
Stocks 25% | Long bonds 25% | Gold 25% | Cash 25%

One year later (stocks surged, gold rose slightly):
Stocks 35% | Long bonds 20% | Gold 28% | Cash 17%
            ↑ sell            ↑ buy       ↑ sell     ↑ buy

Rebalancing actions:
1. Sell excess stocks (35% → 25%; sell 10%)
2. Sell excess gold (28% → 25%; sell 3%)
3. Buy long bonds (20% → 25%; buy 5%)
4. Buy cash (17% → 25%; buy 8%)
```

---

## Rebalancing Triggers: Two Approaches

### Approach 1: Time-Based (Calendar Rebalancing)

**Check and rebalance once per year on a fixed date.**

```
Recommended date: First trading day of January each year
Reasons:
- Prior year's taxes are settled
- Psychologically resets with the new year
- Avoids year-end tax-loss considerations
```

**Execution Process:**
1. Open your investment account; record each asset's current value
2. Calculate total portfolio value
3. Calculate each asset's deviation from 25%
4. If any asset deviates more than 5%, rebalance
5. If all assets are within 5%, **do nothing**

---

### Approach 2: Threshold-Based (Band Rebalancing)

**Trigger when any asset's allocation moves more than ±15 percentage points from the target.**

Harry Browne's original threshold rule:
```
Target: 25%
Lower trigger: 25% − 15% = 10% (buy when any asset falls below 10%)
Upper trigger: 25% + 15% = 40% (sell when any asset rises above 40%)
```

**More practical common version:**
```
Trigger threshold: Any asset deviates ±10 percentage points from target
i.e., trigger when below 15% or above 35%
```

---

### Comparing the Two Approaches

| | Time-Based | Threshold-Based |
|--|-----------|----------------|
| **Frequency** | Fixed; once per year | Variable; could be 0 or multiple times |
| **Simplicity** | ★★★★★ | ★★★☆☆ |
| **Tax planning** | Predictable | Unpredictable |
| **Market adaptability** | Lower | Higher |
| **Best for** | Passive investors | Cost-conscious investors |

**Recommendation: Use time-based (once per year) + threshold monitoring (trigger only in extreme cases).**

---

## Rebalancing in Practice

### Calculation Example

```
Current total portfolio value: ¥120,000

Asset        Current Value   Current %   Target %   Difference
Stocks        ¥42,000         35%         25%       −¥12,000 (need to sell)
Long bonds    ¥24,000         20%         25%       +¥6,000 (need to buy)
Gold          ¥33,600         28%         25%       −¥3,600 (need to sell)
Cash          ¥20,400         17%         25%       +¥9,600 (need to buy)
```

**Actions:**
1. Sell ¥12,000 worth of stock ETF
2. Sell ¥3,600 worth of gold ETF
3. Total cash raised: ¥15,600
4. Buy ¥6,000 worth of bond ETF
5. Buy ¥9,600 worth of money market fund

---

### Using New Contributions to Rebalance (Tax-Efficient Technique)

If you have new money to invest (e.g., a year-end bonus), direct it toward underweighted assets rather than selling overweighted ones:

```
Scenario: ¥20,000 year-end bonus ready to invest

Current deviations:
- Stocks: overweight (excess ¥5,000)
- Long bonds: underweight (short ¥8,000)
- Cash: underweight (short ¥12,000)

Action:
Direct all ¥20,000 to underweighted assets:
- Bond ETF: buy ¥8,000
- Money market fund: buy ¥12,000

Result: No selling required → No taxable event triggered
```

---

## Tax Considerations

### Mainland China Investors

```
A-share ETF transactions:
- Capital gains: Currently exempt from capital gains tax (2024 policy)
- Dividends/interest: 10% withholding tax
- Money market fund income: Tax-free

Implication: Chinese investors face minimal tax friction; main rebalancing cost is trading commissions
```

### U.S. Tax Residents

```
Short-term capital gains (held < 1 year): Taxed as ordinary income; up to 37%
Long-term capital gains (held ≥ 1 year): 0% / 15% / 20%

Strategies:
1. Hold each ETF for 1+ year before selling for rebalancing
2. Rebalance preferably inside IRA/401(k) accounts (tax-free)
3. Use new contributions to buy underweighted assets; minimize selling
4. Tax-Loss Harvesting: sell losing positions at year-end; buy similar ETFs
```

### Overseas Chinese (Non-U.S. Tax Residents)

```
W-8BEN holders:
- Capital gains: Not taxed by the U.S. (taxed by country of residence)
- Dividends: 30% withholding tax (some countries have treaties to reduce to 10–15%)

Recommendations:
- Prefer ETFs that pay little or no dividends
- Consult a local tax advisor
```

---

## Rebalancing Cost Analysis

Costs per rebalancing event:

| Cost Item | A-shares | U.S. Stocks |
|-----------|---------|-------------|
| Trading commission | 0.025–0.03% | $0 (most brokers) |
| Bid/ask spread | ~0.01–0.05% | ~0.01–0.02% |
| Tax cost | 0% (currently exempt) | Depends on holding period |
| **Total per rebalance** | **~0.1%** | **~0.05%** |

**Annual average cost (once per year): ~0.05–0.1%**

---

## The Psychology of Rebalancing: Overcoming Common Urges

### Urge 1: "Stocks have risen so much — shouldn't I hold on?"

**Answer: No.** Rebalancing forces you to "sell high, buy low" — exactly what most retail investors fail to do.

### Urge 2: "Gold keeps falling — did I make a mistake allocating to it?"

**Answer: No.** Gold can underperform for 5–10 consecutive years, but it does its job during crises. When U.S. stocks dropped 30% in 2022, gold was nearly flat — that's the protection it provided.

### Urge 3: "Interest rates are so high — shouldn't I hold more cash?"

**Answer: No.** Any deviation from 25/25/25/25 means you're making a macro timing prediction, and timing the market almost always fails. Stick to the ratios.

---

## Rebalancing Checklist

```
✓ Check during the first week of January each year
✓ Record current value and weight of each asset
✓ If any asset deviates > 10%, execute rebalancing
✓ Prioritize using new contributions (rather than selling) to rebalance
✓ Confirm all four assets are approximately 25% after rebalancing
✓ Record the action log (date, amounts bought/sold, rationale)
✓ Verify ETFs still meet standards (AUM and expense ratios unchanged)
```

---

**Next Chapter:** [Historical Backtesting & Risk Analysis](./05-backtesting.md)
