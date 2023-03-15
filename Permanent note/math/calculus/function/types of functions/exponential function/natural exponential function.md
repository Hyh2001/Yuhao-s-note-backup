$f(x) = e^x$ where $e$ is the [[Euler's number]] and

 $e^h = lim_{h \to 0} (h+ 1)^{\frac{1}{h}}$  

Proof: we can use $\frac{de^x}{dx} = e^x$ which means that by definition: $lim_{h \to 0}\frac{e^{x+h} - e^x}{h} = e^x$ and $e^h \to h+1$

## [[Tailor expansion]] of exponential function

$e^{at} = 1 + at + \frac{(at)^2}{2!} + \frac{(at)^3}{3!} + ... = \sum_{k = 0}^ {\infty} \frac{(at)^k}{k!}$
([Lynch 和 Park, 2017, p. 98](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=98&annotation=2BHGVLW2))  

#### proof 

​ #todo #​ 
## natural exponential function for [[complex variable]]s

$e^{j\theta} = 1+ j\theta - \frac{\theta^2}{2} - \frac{j\theta^3}{3!} + ...$ where $\theta j \in \mathbb{C}$

And when we compare this expansion with Taylor expansions of $cos(\theta)$ and $sin(\theta)$, we can proof [[Euler's formula]]

# natural exponential function program

```julia
exp(x) 
```

[[Matlab natural exponential function]]
‍