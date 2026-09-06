# Comparing Longstaff-Schwartz and Reinforcement Learning for American Option Pricing

This independent project compares Longstaff-Schwartz Monte Carlo (LSMC) with
Least-Squares Policy Iteration (LSPI), a reinforcement-learning approach, for
pricing an American put option.

Both methods are evaluated under the same geometric Brownian motion model and
compared with a Cox-Ross-Rubinstein binomial-tree benchmark.

## Main result

Across Monte Carlo sample sizes from 500 to 100,000 paths, LSMC converged
progressively towards the benchmark. At 100,000 paths, its mean absolute
percentage error was approximately 0.42%, compared with 4.54% for LSPI.

The LSPI policy also learned a lower exercise boundary than the binomial
benchmark, helping explain its persistent downward pricing bias.

## Files

- `paper.pdf` – full research-style report
- `american_option_pricing.ipynb` – Python implementation and experiments
- `paper/` – LaTeX source
- `figures/` – figures used in the paper
