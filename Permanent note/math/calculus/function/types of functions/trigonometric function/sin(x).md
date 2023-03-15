# sin(x)

​#calculus/function#​

## sin(x)

### arcsin(x)

inverse function of $sin(x)$

#### derivative

$\frac{1}{\sqrt{1-x^2}}$

### derivate 

$\frac{d(sin(x))}{dx} = -cos(x)$

### sinc(x)

$sinc(x) = \frac{sin(x)}{x}$

#### properties

$lim_{x \to 0}sinc(x) = 1$
prove:
we know $\frac{-1}{x} \leq \frac{sin(x)}{x} \leq \frac{1}{x}$
And we know that for $x \to 0$
![[Pasted image 20220707202814.png]]
$sin(\theta) \to \theta$

‍

# programming implementation

```julia
sin(x) 
```
