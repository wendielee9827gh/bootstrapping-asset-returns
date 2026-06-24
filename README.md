### Overview
This project addresses a fundamental challenge in quantitative finance: assessing the statistical confidence of empirical asset return metrics. While sample statistics (e.g., mean, standard deviation, and correlation) are straightforward to compute, drawing investment decisions solely from these point estimates is unreliable without quantifying their sample variance. This study implements a rigorous computational **Bootstrapping (Monte Carlo resampling with replacement)** framework in Python to stress-test financial metrics and measure the underlying certainty of key return statistics.

### Key Outcome

By generating $B = 5,000$ independent bootstrapped samples across historical asset returns, the simulation successfully mapped the time-varying joint distribution of benchmark indices (e.g., NASDAQ 100 vs. Dow Jones Industrial Average). The empirical models successfully calculated the **Bootstrapped Standard Error (SE)** and established dynamic, rolling 95% confidence intervals ($\hat{\theta}_N \pm 1.96 \times SE$). This granular boundary mapping uncovers hidden statistical regime shifts, revealing periods where asset correlations were structurally unstable despite strong point-estimate averages.

---

### Tech Stack & Libraries
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Scipy
* **Methods:** Bootstrapping, Monte Carlo Simulation, Rolling-Window Inference, Non-parametric Estimation
