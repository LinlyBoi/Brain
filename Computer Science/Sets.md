#Discrete 
## Sets
  Principal for [[Databases|databases]]
  No duplications
  No order
 $\lvert A \rvert$ = number of elements
 Power set $\rightarrow$ Set of all possible subsets
 Order = Tuple = record in database 
 $A \times B$ $\rightarrow$ Cartesian Product
 Union ($\cup$) $\rightarrow$ Everything in both
 Symmetric Difference  $\rightarrow$ Union without the intersection
 
---

## Multi-Sets
  Allow duplication
  Ordered pairs of (element,n) n -> times repeated in set
  Not very common or approved of
## Partially Ordered Sets
  Reflexive
  Transitive
  Anti Symmetric

---
## Representing Sets
### 1. Curly Braces
 Pretty Standard
### 2. Matrix (For Products)
  $A\times B$ 
  Domain (A) is the column , CoDomain (B) is the row
  $$
  \begin{bmatrix}
  & b_1& b_2& b_3&\\
  a_1\\
  a_2\\
  a_3\\
  \end{bmatrix}
  $$
### 3. Bit String (for subsets)
  Very Cool
  1s and 0s
  $U$ = $\{x_1, x_2, x_3, x_4\}$
  $A$ $\subset$ $U$ = $\{x_1, x_4\}$
  A = 1001