#Probability 
```ad-tldr
#### For 1 Population
### $\bar X  - Z_\frac{α}{2} . \sqrt{\frac{σ}{n}} ≤ µ  ≤\bar X  + Z_\frac{α}{2} . \sqrt{\frac{σ}{n}}$
<br>

#### For 2 Population
### $(\bar X_1 - \bar X_2) - Z_\frac{α}{2} . \sqrt{\frac{σ}{n}} ≤ µ_1 - μ_2 ≤(\bar X_1 - \bar X_2) + Z_\frac{α}{2} . \sqrt{\frac{σ}{n}}$
<br>

#### Replace σ depending on case (S, [[T distribution|t]]$\frac{a}{2}$,[[Pooled Variance|Sp]])
```

```ad-note
- L -> Lower confidence limit
- U -> Upper confidence limit
- θ -> Parameter
- 1 - α  refers to confidence level -> 95% by default
```

## Confidence interval 
If P(L ≤ θ ≤ U) = 0.95 = 1 - α
- Φ$(Z_{\frac{α}{2}})$ = 1 - $\frac{α}{2}$
- P(-$Z_{\frac{α}{2}}$ ≤ Z ≤$Z_{\frac{α}{2}}$) = 1 - α
- Range = U - L = 2 $Z_{\frac{α}{2}} \frac{σ}{\sqrt(n)}$
- When 1-α increases -> $Z_{\frac{α}{2}}$ increases
- As 1-α increases we get a wider confidence interval
- $Z_{\frac{α}{2}} \frac{σ}{\sqrt(n)}$ -> Error (E)
- Things needed to calculate interval
  1. Sample mean
  2. Confidence 
  3. Sample variance
  4. Sample size
```ad-example
Sample size of n = 25 is  drawn from normal population with unknown mean µ and variance 16, have $\bar{X}$ = 15

Find a 95% and 99% confidence interval of n = 25, σ² = 16, σ = 4, $\bar{X}$ = 15

```
-  Choosing Sample size
	There is a relation between sample size and maximum error (E)
	- n = E²
```ad-note
Take n in form of integer (always ceil it up to be safe)

## σ ≈ $\frac{R}{4}$ ≈ $\frac{|Max_{obs}-Min_{obs}| }{4}$

[U,L] -> Confidence limit

1-α -> Confidence level
Sp² -> [[Pooled Variance]]
```

### Confidence interval for Difference of means
- For two populations $µ_1 - µ_2$
- For comparison
- Refer to [[Studying 2 Populations]]
```ad-tip
title: Pooled variance rule
## Sp² = $\frac{(n_1 - 1) S^2_1+(n_2- 1)S^2_2 }{n_1+n_2-2}$
- given Sample variances and sizes
```



```ad-seealso
title: See also
[Hypothesis test and confidence reference](https://blog.minitab.com/en/adventures-in-statistics-2/understanding-hypothesis-tests-confidence-intervals-and-confidence-levels)

[[Normal (Gaussian) Distribution]]

[[Sampling Distribution]]

```
