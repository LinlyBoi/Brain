#Probability 
## Moment Generating Function
### Definition
> The mean of random variable is referred to as first moment of prob distribution
> In general rth moment is $E(x^r)$
> Derive MGF to get $E(x^r)$, $r$ amount of times

#### General Steps to do the thing
>1. $\mu x(t) = E(e^{xt})$
>2. Get function form of $M_x(t)$ using series simplification
>3. Derive $n$ amount of times to get $n^{th}$ moment $\rightarrow$ $E(x^n)$
### Used to calculate $E(x)$ using differentiation instead of sigma and integrations
>$M_x(t) = E(e^{tx})$
>$E(x^r) = \frac{dr}{dt} M_x(t)$ where t = 0 <- rth moment
>apply Maclaurin to Mx(t) = E(e^xt)
>1+t(E(x)) + t^2/2! . E(X^2)......
>derive with respect to t , t gets yeeted and put t = 0, only the rth t doesn't have a t and the rest are 0s so its E(x^r)
>![[Screenshot_20220427_145258.png]]
>just to understand^

### Usage in [[Special Discrete probablity distributions]]
#### Binomials
>$M_x(t) = E(e^{tx})$
>$\sum{e^{xt} \cdot f(x)}$
>$f(x) = ^nCx \cdot p^x \cdot q^{n-x}$
>$\sum_{x}^{n}{^nC_x \cdot {(e^{tp})}^x \cdot q^{n-x}}$ $\leftarrow$ this is binomial
>$M_x(t) = (pe^t + q)^n$ $\leftarrow$ Whole function

#### Geometric
> refer to Geometric sequence f(x) etc
> ## Proof:
>  ![[Screenshot_20220427_151017.png]]