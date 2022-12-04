#Probability 
# Continous Random variables
## Definition
> ### Random variables denoting range of values: Length , Time , Distance
> ### Probability of a range of functions rather than a single value

## General Notes
> ### This case uses Integration instead of summation
> CDF -> $F(x)$ (Uppercase)
> PDF -> $f(x)$ (Lowercase)
> ### To obtain CDF from PDF
> - Integrate PDF from start to end
> ### To obtain PDF from CDF
> - Take the derivative (differentiation)
## Probability density function
> ### To be valid pdf 
> 1. $f(x) \geqslant 0$ for all values of x
> 2. $P(a<x<b) = \int^{b}_{a}{f(x) \, dx}$
> 3. Integral from negative infinity to infinity (Start , end)

## Cumulative distribution function (CDF)
> #### from start till x (Probability of less than)
> 1. rename $x \rightarrow t$ in pdf 
> 2. Integral of start till $x$

## Mean and Variance
> $\mu = E(x)  = \int^{start}_{end}{f(x) \cdot x \,dx}$ 
> $V(X) = E(x^2) - \mu^2$

## [[Special Continous Random Variables]]
