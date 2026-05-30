# IMC-Prosperity-4-Manual-Trading-write-up
![Rank](https://img.shields.io/badge/Rank-%2373%20Overall-gold?style=for-the-badge&logo=github)
![Region](https://img.shields.io/badge/India-%2311-orange?style=for-the-badge)
### Post competition write-up for IMC Prosperity 4's Manual Trading Challenge where I ranked #11 India and #73 Overall out of 18000+ teams.
First of all, thank you <a href="https://www.linkedin.com/in/parth-sharma9913/">Parth Sharma</a> (lead Algorithmic Strategy) and <a href="https://www.linkedin.com/in/aatman-patel-a28208371/">Aatman Patel</a> (lead mental support) who helped me, <a href="https://www.linkedin.com/in/patrank-rai-681549378/">Patrank Rai</a> (lead Manual Trading Desk), with all the late nights, the brainstorming sessions, and the technical foundation that allowed us to secure this result as only mere undergrad freshers.

To all the participants and future me for the subsequent rounds of Prosperity and other such competitions.
## 📈IMC Prosperity 4
![Event](https://img.shields.io/badge/Competition-IMC%20Prosperity%204-blue?style=flat-square)
![Category](https://img.shields.io/badge/Challenge-Manual%20Trading-brightgreen?style=flat-square)
### What is IMC Prosperity?
Prosperity is the flagship annual global trading challenge hosted by IMC Trading, one of the world’s leading quantitative market-making firms. Designed by IMC’s top quantitative researchers, traders, and software engineers, the competition provides STEM university students with a highly rigorous, life-like simulation of electronic financial markets.  
The challenge tests core competencies required in high-frequency trading (HFT) and quantitative finance: statistical arbitrage, market making, derivative pricing, mathematical optimization, and risk management under severe constraints.  
### The Prosperity 4 Frontier
The Prosperity 4 edition shifted from traditional terrestrial market setups to a cosmic, outer-space environment. Over a grueling 16-day period, competing teams navigated five distinct rounds of increasing complexity, trading unique foreign market assets using the game's virtual currency, XIRECs.  Each round was split into two parallel tracks:
- Algorithmic Trading: Building, backtesting, and deploying automated Python trading strategies to capture market inefficiencies, manage inventory skews, and execute market-making models.
- Manual Trading: Solving time-constrained, highly complex mathematical, probabilistic, and game-theoretic puzzles that replicate discretionary trading and structural boundary analysis.

***This write-up covers only the Manual Trading Challenge of IMC Prosperity 4 and all the recommendations are for the manual traders though some apply to the algorithmic side as well.
## 💡Some very important tips
- Read the Prosperity wiki very well. It is of utmost importance that you understand the challenge in front of you.
- Use AI to understand the challenges, not to find answers.
- Don't get lost in the community discord, very little of what is discussed there is of use to you.
- Write-ups are gold, read the previous year wikis and find the logic in the write-ups of that year. This will help you develop the correct thought processes to ace the challenges in front of you.

## Round: 1 
I am not going to lie—I completely relied on AI (Gemini PRO) for this round. My literal first thought was, *"Why would anyone even waste their time on this?"* and oh boy, was I wrong. Turns out, you can't just prompt for direct answers and expect the correct strategy straight away. 

> [!NOTE]
> **Key Takeaway:** This round taught me to use AI as a conceptual guide. Using AI strictly to break down and thoroughly understand the problem is the winning move. 

Skipping the Prosperity Wiki for this round was another major blunder on my part, but it set the foundation for how I tackled the rest of the challenge.
## Round: 2
The objective was to allocate a finite budget of 50,000 XIRECs across three growth pillars—**Research**, **Scale**, and **Speed**—to maximize net Profit and Loss (PnL).

### My Allocation Strategy: `17 / 47 / 36`

| Pillar | Allocation (%) | Focus Area |
| :--- | :---: | :--- |
| **Research** | **17%** | Quantitative edge, alpha generation, ML infrastructure |
| **Scale** | **47%** | Strategy deployment, exchange access, volume capacity |
| **Speed** | **36%** | Low-latency execution, hardware (FPGA, RF, Microwave) |

---

### Strategy Breakdown & Mathematical Proof

The final PnL score is governed by the following objective function:

$$ PnL = (Research * Scale * Speed) - Budget Used $$

#### 1. Research: Capturing the Logarithmic Alpha (17%)
Research determines the fundamental edge of the market-making operation, modeled by the function:

$$ R(x) = 200,000 * [ ln(1+x) / ln(101) ] $$

Evaluating my allocation of x = 17:

$$ R(17) = 200,000 * [ ln(18) / ln(101) ] = 125,256.32 $$

By investing just **17%** of my budget, I successfully capture **62.63%** of the maximum theoretical trading edge. Pushing further down this curve yields severe diminishing marginal returns, making any additional allocation highly inefficient.

#### 2. Scale: Linear Capital Amplification (47%)
Scale dictates market coverage and volume capacity, growing linearly according to:

$$ S(x) = 0.07 * x $$

For my allocation of x = 47, the multiplier evaluates directly to:

$$ S(47) = 0.07 * 47 = 3.29 $$

Because Scale does not suffer from diminishing returns, every percentage point I moved from Research into Scale acts as a pure, constant amplifier on my captured alpha.

---

### Game-Theoretic Analysis of Speed (36%)

The Speed pillar determines execution hit rate by mapping ordinal player ranks linearly to a multiplier interval between 0.1 and 0.9. This creates a competitive tournament where you must anticipate crowd psychology.

I selected **36%** to intentionally front-run two primary player cohorts:
* **The Naive Splitters (33.3%):** Participants who default to an even three-way split.
* **The Round-Number Bias (35%):** Participants who cluster at standard 5% psychological intervals.

Bidding 36% allows me to jump ahead of these massive baseline clusters to secure a high execution multiplier (projected at 0.65 - 0.78) while conserving maximum residual capital for Scale.

---

### Portfolio Optimization vs. Naive Benchmark

Before factoring in the competitive rank-based speed multiplier, my optimized portfolio vastly outperforms a standard equal-split baseline:

| Strategy Allocation | Research Value | Scale Multiplier | Gross Product (R * S) | Budget Spent |
| :--- | :--- | :--- | :--- | :--- |
| **Naive Split (33 / 33 / 34)** | 152,827.67 | 2.31 | 353,031.91 | 50,000 XIRECs |
| **My Optimized (17 / 47 / 36)** | **125,256.32** | **3.29** | **412,093.30** | **50,000 XIRECs** |
| **Delta** | *-18.04%* | *+42.42%* | **+16.73%** | *0%* |

> [!NOTE]
> **Key Takeaway:** Shifting capital away from the flat, saturated end of the Research curve into the linear Scale engine generated a **16.73% expansion in raw gross capacity** before the speed rank advantage was even applied.

## Round: 3
In Round 3, I optimized a dual-bid architecture for trading Ornamental Bio-Pods against counterparties (Gardeners). Rather than relying on standard, static mathematical midpoints, my strategy was explicitly engineered around **behavioral game theory and competitor psychological profiling**. 

By diagnosing the market's collective risk-aversion and predicting how the crowd would react to an aggressive, asymmetric penalty structure, I successfully anticipated the global trading sentiment. This psychological arbitrage allowed me to out-maneuver the herd, capturing a total manual trading P&L of **78,090**.

---

### Part I: Establishing the Psychological Anchor

To out-think my competitors, I first isolated the theoretical baseline that every rational market participant would use as their starting reference point. 

Given the uniform distribution of reserve prices $R \sim U(670, 920)$, the base Expected Profit function $E[\Pi(b)]$ for an unpenalized bid $b$ is defined by the product of execution probability and the captured trading spread:

$$E[\Pi(b)] = \left(\frac{b - 670}{250}\right) \cdot (920 - b)$$

I evaluated the first derivative with respect to $b$ to pinpoint the vertex of this profit parabola:

$$\frac{d}{db} E[\Pi(b)] = \frac{1}{250} \cdot (1590 - 2b)$$

Setting the derivative to zero locates the exact unpenalized mathematical peak:

$$1590 - 2b = 0 \implies b = 795$$

Although a standard optimization model points to **795** as the peak, I treated this value purely as a psychological benchmark. I factored in how participant sentiment and the defensive reaction to the cubic penalty would shift the competitive herd away from this static midpoint.

---

### Part II: Deconstructing Competitor Sentiment

The introduction of the global average tracking system fundamentally transformed this challenge into a **Keynesian Beauty Contest**. My entire strategy relied on predicting how the market's collective sentiment would shift away from the 795 anchor.

#### 1. The First Bid: Capitalizing on Value-Seeking Behavior
For the first bid, there was no penalty for falling below the global average. I anticipated that the dominant sentiment here would be pure margin-maximization. Traders would aggressively underbid the 795 mathematical optimum to secure deep value on low-reserve counterparties. 

* **My Psychological Adjustment:** Expecting a dense cluster of bids below the optimum, I leaned into this conservative sentiment and positioned my first bid at **765**. This allowed me to front-run the ultra-low bidders while maintaining an incredibly high profit margin of **155 units** per trade.

#### 2. The Second Bid: Anticipating the Cubic Penalty Panic
The second bid introduced a severe, asymmetric cubic penalty for teams falling below the global second-bid average ($avg\_b2$):

$$\text{Penalty Factor} = \left(\frac{920 - avgb_2}{920 - b_2}\right)^3$$

I recognized that this specific mathematical phrasing would trigger widespread **loss aversion**. Traders would realize that being even slightly under the average would destroy their P&L, sparking an aggressive upward bidding spiral as everyone tried to out-climb each other. 

* **My Psychological Adjustment:** I deduced that the herd would completely abandon the 795 anchor and panic-shift their bids deep into the 800s. To guarantee safety from this psychological feedback loop, I over-indexed on security and aggressively priced my second bid at **865**. I was willing to sacrifice a small amount of theoretical spread to completely insure my trades against the crowd’s panic.

---

### Part III: Empirical Validation of the Strategy

The post-round market results perfectly validated my behavioral thesis, proving that my intuition regarding competitor sentiment was remarkably accurate.

#### Performance Summary

| Metric | Lowest Bid ($b_1$) | Highest Bid ($b_2$) | Total / Average |
| :--- | :--- | :--- | :--- |
| **My Bid Price** | **765** | **865** | — |
| **Global Average Bid** | 768 | 859 | — |
| **Accepted Trades** | 353 | 425 | **778** |
| **Rejected Trades** | 647 | 575 | **1,222** |
| **Total Block P&L** | **54,715** | **23,375** | **78,090** |

#### Visual Strategy Alignment

```text
               MARKET OUTCOME HISTOGRAM & STRATEGY ALIGNMENT

       [First Bid Cluster]                      [Second Bid Cluster]
  Traders maximize profit margin.           Traders panic over cubic penalty.
       
           My Bid: 765                                  Global Avg: 859
                │                                            │
   ┌───┐ ┌───┐  ▼  ┌───┐                               ┌───┐ ▼ ┌───┐
   │   │ │   │  ┆  │   │                               │   │ ┆ │   │ ┌───┐
───┴───┴─┴───┴─────┴───┴───────────────────────────────┴───┴───┴───┴─┴───┴───
  670          768 (Global Avg)                       855     865 (My Bid) 920
```

> [!NOTE]
> **Key Takeaways:**
>
> *First Bid Validation:* The global first-bid average landed at 768. My instinct was flawless here; the market heavily discounted their bids just as I predicted. Bidding 765 placed me directly inside the meat of the volume curve, pulling a massive 54,715 P&L out of the lower block.
>
> *Second Bid Validation:* The global second-bid average surged to an astonishing 859, driven entirely by the collective panic I anticipated. Because I correctly foresaw this hyper-inflation and positioned myself at 865, I cleared the global average line with precision. This insulated my P&L from the catastrophic cubic penalty that wiped out a significant portion of the grid, locking in a clean, unpenalized secondary return.

## Round: 4
Instead of trying to predict the chaotic directional movements of Aether Crystals (which had a fixed annualized volatility of 251%), this strategy focused entirely on quantitative arbitrage. We isolated and captured mathematical discrepancies between market prices and theoretical fair values, maintaining a perfectly market-neutral portfolio.
### 1. Structural Arbitrage: The Chooser Loop

The most profitable mispricing on the board was the Chooser option (`AC_50_CO`), which was trading at a heavy premium. A chooser option allows the holder to decide at Week 2 whether the contract becomes a 3-week Call or a 3-week Put. 

Mathematically, the value of this choice at Week 2 is $\max(C_{3w}, P_{3w})$. By applying standard put-call parity substitution, this functional identity simplifies perfectly to:

$$\text{Chooser Value} = \text{3-week Call} + \text{2-week Put}$$

The market was buying the Chooser for **22.2**, but the individual replication pieces (the 3-week Call and 2-week Put) could be bought together for just **21.80** (12.05 + 9.75). 

**The Play:** We shorted 50 Chooser contracts and bought 50 pairs of the underlying components. This locked in a risk-free spread of **0.40 per contract** at day zero. Because the hedges perfectly mirror the chooser's payoff at the decision date, this profit was entirely decoupled from market direction.

---

### 2. Statistical Edge (Volatility Arbitrage)

The challenge documentation explicitly fixed the annualized volatility at **251%**. This allowed us to calculate the exact theoretical fair value for every contract on the board using a standard Black-Scholes pricing model. 

Since all positions were held to expiration across 100 independent simulations, the final cash settlement payouts were statistically guaranteed to converge toward their expected mathematical values (Law of Large Numbers). We deployed capital strictly where the market price deviated from this expected value:

* **Buying Underpriced Variance:** `AC_35_P`, `AC_40_P`, and `AC_50_C_2` were trading below their statistical worth. Buying these contracts meant we collected more cash at settlement on average than we spent upfront.
* **Selling Overpriced Premium:** `AC_40_BP` (Binary Put) and `AC_60_C` were irrationally expensive. We shorted these to harvest the overvalued premium.

> [!NOTE]
> **Avoiding the Trap:** We completely avoided the Knock-Out Put (`AC_45_KO`). Given 251% volatility simulated across 60 discrete daily steps, the probability of the underlying asset hitting the 35.0 barrier at some point is nearly 100%. Paying any premium for a contract structurally bound to expire worthless is a negative-EV gamble.

---

### 3. Direction-Blind Hedging (Delta Neutrality)

To ensure our profits came solely from these mathematical mispricings rather than luck, we had to eliminate our exposure to the raw price movements of the Aether Crystals.

After aggregating the directional sensitivities (Deltas) of all our long and short option positions, the net portfolio left us slightly **Short Delta**. This meant a sudden upward spike in the crystal price would harm our net margins. 

**The Fix:**
To perfectly balance the scales, we executed a spot hedge by **buying 11 units of the underlying Aether Crystal** at 50.025. This brought our net portfolio Delta to zero. Whether the crystal rallied or crashed during the 100 simulation runs, the gains and losses between our spot and options legs washed out, leaving our mathematical edge perfectly intact.

---

### Final Execution Portfolio

| Product | Action | Target Price | Volume | Strategy Component |
| :--- | :--- | :--- | :--- | :--- |
| **AC_50_CO** | SELL | 22.2 | 50 | Structural Arbitrage |
| **AC_50_C** | BUY | 12.05 | 50 | Arb Hedge |
| **AC_50_P_2** | BUY | 9.75 | 50 | Arb Hedge |
| **AC_40_BP** | SELL | 5.0 | 50 | Vol Arb (Overpriced) |
| **AC_35_P** | BUY | 4.2 | 50 | Vol Arb (Underpriced) |
| **AC_50_C_2** | BUY | 9.75 | 50 | Vol Arb (Underpriced) |
| **AC_40_P** | BUY | 6.45 | 50 | Vol Arb (Underpriced) |
| **AC_60_C** | SELL | 8.8 | 50 | Vol Arb (Overpriced) |
| **Aether Crystal**| BUY | 50.025 | 11 | Delta Hedge |

## Round: 5
