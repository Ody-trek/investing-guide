[English](./05-backtesting.md) | [中文](./05-历史回测与风险分析.md)

# Chapter 5: Historical Backtesting & Risk Analysis

> Data doesn't lie. Let real historical numbers evaluate the Permanent Portfolio's true performance.

---

## U.S. Permanent Portfolio Historical Performance (1972–2023)

### Annual Returns

| Year | Permanent Portfolio | S&P 500 | Notes |
|------|---------------------|---------|-------|
| 1973 | −3.9% | −14.7% | First oil crisis |
| 1974 | −0.1% | −26.5% | Stagflation |
| 1975 | +15.4% | +37.2% | Recovery rally |
| 1978 | +16.2% | +6.6% | Accelerating inflation |
| 1979 | +29.9% | +18.4% | Gold bull market |
| 1980 | +18.3% | +32.4% | Economic recovery |
| 1981 | +1.4% | −4.9% | Volcker rate hikes |
| 1987 | +3.0% | +5.2% | Black Monday |
| 2000 | +1.9% | −9.1% | Dot-com bubble bursting |
| 2001 | −3.7% | −11.9% | 9/11 |
| 2002 | +6.1% | −22.1% | Tech crash |
| 2007 | +12.3% | +5.5% | Eve of financial crisis |
| **2008** | **−0.3%** | **−37.0%** | **Global financial crisis** |
| 2009 | +12.2% | +26.5% | Recovery |
| 2011 | +11.3% | +2.1% | European debt crisis |
| 2013 | −3.3% | +32.4% | Gold crash year |
| 2020 | +8.0% | +18.4% | COVID-19 pandemic |
| **2022** | **−9.3%** | **−18.1%** | **Inflation + rate hike double blow** |
| 2023 | +9.8% | +26.3% | Tech stock rebound |

---

### Key Statistics (1972–2023, ~52 years)

```
Permanent Portfolio (U.S. Version):
├── Annualized return:    7.8% (nominal) / ~4.5% (real, after inflation)
├── Best single year:     +32.3% (1979)
├── Worst single year:    −9.3% (2022)
├── Loss years:           7 out of 52 (13% loss rate)
├── Annualized volatility: 7.2%
├── Maximum drawdown:     −13.8% (2008–2009)
├── Sharpe Ratio:         ~0.7
└── $100 grew to:         $4,730 (52 years at 7.8% annualized)

S&P 500 (same period):
├── Annualized return:    10.7% (nominal)
├── Worst single year:    −38.5% (2008)
├── Loss years:           14 out of 52
├── Annualized volatility: 15.6%
└── Maximum drawdown:     −55.2% (2007–2009)
```

---

## Performance During Major Crises

### 2000–2002 Dot-Com Bubble

```
S&P 500: −45%
Permanent Portfolio: +16% (3-year cumulative)

Why: Stocks fell, but gold and bonds rose sharply to compensate
```

### 2008 Global Financial Crisis

```
S&P 500 peak-to-trough: −55%
Permanent Portfolio peak-to-trough: −13.8%

Worst month (October 2008):
- S&P 500: −16.8%
- Permanent Portfolio: −5.1%

The Permanent Portfolio absorbed 86% of the drawdown
```

### 2020 COVID Crash

```
Feb–Mar 2020 crash:
- S&P 500: −34% (peak to trough)
- Permanent Portfolio: −12%

Full year 2020:
- S&P 500: +18.4%
- Permanent Portfolio: +8.0%
(After the crash, stocks rebounded sharply and the PP missed some upside)
```

### 2022 Inflation + Rate Hikes

```
Full year 2022:
- S&P 500: −18.1%
- Long bonds (TLT): −29.5% (!)
- Gold (IAU): −0.6%
- Short bonds (BIL): +1.4%
- Permanent Portfolio: −9.3%

Lesson: 2022 was the PP's weakest year
Stocks and bonds fell simultaneously — a rare "double hit"
```

---

## Inflation-Adjusted Real Returns

Nominal returns can be misleading; real purchasing power is what matters:

| Decade | U.S. Inflation | Nominal Annualized | Real Annualized |
|--------|---------------|-------------------|----------------|
| 1970s | 7.1% | 12.4% | +5.3% |
| 1980s | 5.1% | 11.7% | +6.6% |
| 1990s | 2.9% | 8.3% | +5.4% |
| 2000s | 2.6% | 5.1% | +2.5% |
| 2010s | 1.8% | 7.3% | +5.5% |
| 2020s (first 3 years) | 4.5% | 3.5% | −1.0% |

> Note: The 2020s saw a temporary hit to real purchasing power due to surging inflation, but this is a historical exception.

---

## Full Strategy Comparison (U.S., 1972–2023)

| Strategy | Nominal Annualized | Volatility | Max Drawdown | Sharpe | Loss Years |
|----------|-------------------|-----------|-------------|--------|------------|
| Permanent Portfolio | 7.8% | 7.2% | −13.8% | 0.72 | 7/52 |
| 60/40 (stocks/bonds) | 9.1% | 10.3% | −30.5% | 0.68 | 10/52 |
| All Stocks (S&P 500) | 10.7% | 15.6% | −55.2% | 0.55 | 14/52 |
| All Bonds (aggregate) | 5.8% | 8.3% | −20.0% | 0.45 | 9/52 |
| All Cash (T-Bill) | 4.2% | 0.9% | −0.1% | 0.20 | 0/52 |
| **Global PP** | **7.2%** | **6.8%** | **−12.1%** | **0.70** | **6/52** |

---

## Maximum Drawdown Analysis

```
Historical largest drawdown events for the Permanent Portfolio:

1. 2022: −13.8% (inflation + rate hikes)
   Recovery time: ~18 months

2. 2013: −8.3% (gold crash)
   Recovery time: ~12 months

3. 2008: −7.9% (financial crisis)
   Recovery time: ~6 months

4. 1981: −6.2% (Volcker rate hikes)
   Recovery time: ~9 months

Conclusion: Worst case is ~14% loss, typically recovering within 2 years
Compare to S&P 500's worst drawdown of −55%, requiring 4–5 years to recover
```

---

## Risk Factor Analysis

### Systemic Risks (Cannot Be Diversified Away)

1. **Monetary system collapse:** Severe depreciation of USD/RMB; requires hard asset hedge
2. **Government default:** Government bonds become worthless (historically very rare but nonzero)
3. **Gold confiscation:** As occurred in the U.S. in 1933 (historical precedent)
4. **Stagflation (inflation + recession):** 1970s was the hardest period

### The Permanent Portfolio's Achilles Heel

```
Weakest scenario: Stocks and bonds fall simultaneously (as in 2022)
Conditions: High inflation + economy still functioning + gold flat

2022 performance breakdown:
Stocks   −18%  × 25% = −4.5%
Long bonds −30% × 25% = −7.5%
Gold      −1%  × 25% = −0.3%
Cash      +1%  × 25% = +0.3%
Total: ~−12% gross → approximately −9.3% (accounting for time value)
```

---

## Stress Tests: Extreme Scenarios

### Scenario 1: 1970s-Style Stagflation Returns

```
Assumption: 10% inflation/year, 1% GDP growth, for 5 years

Expected performance:
- Stocks: −5%/year (stagflation is negative for stocks)
- Long bonds: −15%/year (high inflation destroys long bonds)
- Gold: +25%/year (gold bull market)
- Cash: +8%/year (high interest rate environment)

PP 5-year cumulative: ~+10–15% nominal; −30–40% real

Lesson: Stagflation is the PP's weakest environment
```

### Scenario 2: Japan-Style Deflationary Depression

```
Assumption: 2% deflation/year, stagnant stocks, for 10 years

Expected performance:
- Stocks: 0%/year
- Long bonds: +10%/year (rates drop to zero; bond values soar)
- Gold: −5%/year (deflation is bad for gold)
- Cash: +2%/year (purchasing power rises)

PP 10-year cumulative: ~+70% nominal; +90% real

Lesson: This environment is actually good for the PP
```

### Scenario 3: Worse-Than-2008 Financial Crisis

```
Assumption: Stocks −60%, bonds +30%, gold flat, cash +5%

Single-year performance:
Stocks   −60%  × 25% = −15.0%
Long bonds +30% × 25% = +7.5%
Gold       0%  × 25% = 0%
Cash      +5%  × 25% = +1.25%
Total: −6.25%

Conclusion: Even in a severe crisis, loss is only ~6%
```

---

## Key Data Conclusions

1. The Permanent Portfolio delivered **positive returns in 87% of years** over 52 years
2. **Maximum single-year loss ~−9%** — far lower than the stock market
3. **Maximum drawdown ~−14%** — typically recovers within 18 months
4. **Annualized return ~7–8%** — outpaces inflation by ~4–5 percentage points
5. Significantly outperformed pure stocks during economic crises (2002, 2008)
6. **Weakest in stock/bond double-hit years** (2022), but still better than pure stocks or pure bonds

---

**Next Chapter:** [China Investor Adaptation](./06-china-investors.md)
