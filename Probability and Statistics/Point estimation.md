#Probability 
Statistics --> Descriptive and Inferential
Function of random sample that doesn't depend on unknown points --> Statistics
## Inference
- to make some conclusion based on incomplete information (educated guess)
- Conclusion about population from sample data
### Parameter estimation
- Point estimation $\rightarrow$ $\hat{\mu}$  = $\bar{X}$ 
- $\theta$ is population parameter 
- $\hat{\theta}$ is function from sample data
# How to get point estimate?
## Method of Moment Estimation
- Method of [[Moment Generating Function|moment]] estimation
- In terms of population parameter
- $\mu_k$ = $m_k$ (Population moment = sample moment)
- ##### When population is continuous
  - $E(X) = \int_{-\infty}^{\infty}{f(x) \cdot x \, dx}$
  - $E(Sample) \rightarrow $\sum{\frac{X_i}{n}} \rightarrow$ Always discrete
- ##### When population is [[Random variables#Discrete Random Variable distribution|discrete]]
  - $E(X) = \sum_{i=1}^{n}{f(x) \cdot x}$
## Maximum likelihood estimation
1. $L(\theta)$ = $\prod_{i = 1}^{n}{f(X_i,\theta)}$
2. *Take $\ln$* $\rightarrow$ $\ln{L(θ)}$ = $\sum_{i = 1}^{n}{\ln{f(X_i,θ)}}$
3. *Derive* $\rightarrow$ $\frac{d\ln{L(\theta)}}{d\theta}$
-  Invariance property
	- New estimators $\rightarrow$ replace the required parameter with the original point estimator $\hat{\theta}$ 

#### Properties of Estimates

## Which Estimator is better?
Need 3 things
1. [[#Bias]]
2. [[#Efficiency]]
3. [[#Consistency]]

## Bias 
- if $\hat{\theta}$ is an estimator $\rightarrow$ $Bias = E(\hat{\theta}) - \theta$ $\rightarrow$ $\theta$ is the true value of the $\mu$ in distribution
- if estimator = the parameter $\rightarrow$ unbiased
## Mean square error 
- $MSE(\hat{\theta}) = E(\hat{\theta} - \theta)^2$
- *proof here*
- $MSE(\hat{\theta}) = Var(\hat{\theta}) + ( bias(\hat{\theta}) )^2$
## Minimum Variance Unbiased Error
- Only for unbiased estimator
- Mean Square error = $Var(\hat{\theta})$
## Efficiency 
- For all cases
- Efficiency $\rightarrow$ compare MSE($\hat{θ}$)
- More efficient when error is less.
- $\hatθ_1$ > $\hatθ_2$ when MSE($\hatθ_1$) < MSE($\hatθ_2$) $\rightarrow$ $\hatθ_1$ better my friend :D

## Consistency
- $\lim_{n\to\infty}$ MSE($\hat{\theta}$)
- if there's n in denominator $\rightarrow$ MSE equals 0 at ∞ $\rightarrow$ gg eg consistent




