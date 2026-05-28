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

> **Key Takeaway:** Shifting capital away from the flat, saturated end of the Research curve into the linear Scale engine generates a **16.73% expansion in raw gross capacity** before the speed rank advantage is even applied.

## Round: 3
