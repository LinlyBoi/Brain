#Probability 
```ad-tldr
## Functions we use
### **r(func)**: random sample
### **p(func)**: CDF
### **q(func)**:  PDF
### **optim**: Optimisation algorithm function

```
## [[Point estimation#Method of Moment Estimation|Method of Moments Estimation]]
1. E(pop)
2. E(Sample)
3. E(pop) = E(Sample)
-  Method of moments with Bernoulli distribution usually has 0 bias
## Maximum Likelihood Estimation
```ad-hint
title: Steps

 ### 1. L(X) = $\prod_{i=1}^n{f(X, θ)}$ <br><br>
 ### 2. ln(L(x)) = $\sum_{i=1}^n{ln(f(X, θ))}$
 ### 3. Optimisation instead of derivative
```

^427909

#### Optimisation Algorithm
```ad-important
title: Syntax
optim(par = c(var1=,var2=...),fn=Negative Log-Likeliehood Function, data = sample,control = list(parscale = c(var1 = , var2=....)))
```
- starts at random point (0, 0) by default
- Random movements till it reaches goal
- Trial and error
- If movement is closer to goal move to it
- [[R]] does the movements for us faster than deriving 
- Else move back to it
- What is needed:
  1. Initial start
  2. Function ([[#^427909|PDF]])

```ad-info
Sometimes we can have a stopping criteria (Time, relative error, number of iterations)


Local minimum or maximum are enough in some cases
```

```ad-seealso
title: See also
[[Point estimation]]

[[Interval Estimation]]

[[R]]
```

