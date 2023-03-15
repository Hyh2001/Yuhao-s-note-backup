---
sr-due: 2023-06-13
sr-interval: 126
sr-ease: 248
---

#calculus/series #review 
Power [[series]] has the form of: 

$\sum_{n=0}^{\infty} c_nx^n = c_0 + c_1x + c_2x^2 + c_3x^3 + \ldots+c_{n}x^{n}$ 

where $x$ are variables and $c_n$ are ***coefficients ​***of the series.
 ([Stewart, 2016, p. 746](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=778&annotation=G6YJB7SE))
<!--SR:!2023-03-05,1,228-->

When $c_{n}=1$, the series becomes a [[geometric series]]. 

# power series about $a$

We define a power series about $a$ as:
$\sum_{n=0}^{\infty} c_n(x-a)^n = c_0 + c_1(x-a) + c_2(x-a)^2 + c_3(x-a)^3 + ...$
($c_{0}=(x-a)^{0}=1$ which means that even for $x=a$ this requisite still stand. )
This power series converges when $x=a$ 
([Stewart, 2016, p. 747](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=779&annotation=JWNPMLMP))

# [[convergent|convergence]] of power series 
Power series will [[convergent]] or [[divergent]] for specific $x$ values.  ([Stewart, 2016, p. 746](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=778&annotation=AUHDHSNM))
There are only three possibilities 
1. The series converges only when $x=a$ ($R=0$)
2. The series converges for all $x$ ($R=\infty$) 
3. There is a positive number $R$ such that the series converges if $|x-a|<R$ and it diverges if $|x-a|>R$ (The number $R$ will be called the radius of convergence)  
([Stewart, 2016, p. 749](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=781&annotation=68EIRRTS))  

[[interval of convergence]]

[[ratio test]] should be applied to determine the radius of convergence. ([Stewart, 2016, p. 750](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=782&annotation=VQQZRIHI))

# [[differentiate]] of power series 
For a power series, if its radius of convergence $R>0$ then it is [[differentiable]] on the interval $(a-R,a+R)$ 
$f^{\prime}(x) = c_{1}+ 2c_{2}(x-a)+3c_{3}(x-a)^{2}+\ldots = \sum_{n=1}^{\infty}nc_{n}(x-a)^{n-1}$ 
([Stewart, 2016, p. 754](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=786&annotation=54RDU8MJ))
# [[integration]] of power series 
$\int f (x) dx=C+c_{0}(x-a)+c_{1}\frac{(x-a)^{2}}{2}+c_{2}\frac{(x-a)^{3}}{3}+\ldots=C+\sum_{n=0}^{\infty}c_{n}\frac{(x-a)^{n+1}}{n+1}$ 
([Stewart, 2016, p. 754](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=786&annotation=54RDU8MJ))

# application of power series 
## represent functions
The main use of a power series is to represent some functions ([Stewart, 2016, p. 748](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=780&annotation=EGSIUJAZ))
The problem is that we need to find the specific power series that can represent functions. 
We can finally use [[Taylor series]] to represent specific functions.  ([Stewart, 2016, p. 759](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=791&annotation=2PLQR9YN))

The strategy is useful for integrating functions that don’t have elementary [[antiderivative]], for solving differential equations, and for approximating functions by [[polynomial]]. ([Stewart, 2016, p. 752](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=784&annotation=HJZ322ZN))


Below we have listed some functions represented in power series 
1. [[power series - exponential function]]


