#Probability 
Statistics --> Descriptive and Inferential
Function of random sample that doesn't depend on unknown points --> Statistics
## Inference
- to make some conclusion based on incomplete information (educated guess)
- Conclusion about population from sample data
### Parameter estimation
- Point estimation --> $\hatµ$  = $\bar X$ 
- θ is population parameter 
- $\hatθ$ is function from sample data
# How to get point estimate?
## Method of Moment Estimation
- Method of [[Moment Generating Function|moment]] estimation
- In terms of population parameter
- µ$_k$ = m$_k$ (Population moment = sample moment)
- ##### When population is continuous
  - E(X) = $\int_{-\infty}^{\infty}{f(x).x}$
  - E(Sample) --> $\sum{\frac{X_i}{n}}$ --> Always discrete
- ##### When population is [[Random variables#Discrete Random Variable distribution|discrete]]
  - E(X) = $\sum_{i=1}^{n}{f(x) * x}$
## Maximum likelihood estimation
1. L(θ) = $\prod_{i = 1}^{n}{f(X_i,θ)}$
2. *Take $\ln$* --> $\ln{L(θ)}$ = $\sum_{i = 1}^{n}{\ln{f(X_i,θ)}}$
3. *Derive* --> $\frac{d\ln{L(θ)}}{dθ}$

#### Properties of Estimates