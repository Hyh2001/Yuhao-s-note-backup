#calculus/integral 

There are several methods to integrate [[trigonometric function]]

# for sin(x)cos(x) like

$\int sin^m(x)cos^n(x)dx$

1. if $n = 2k +1$
   $\int sin^m(x)cos^{2k+1}(x)dx = \int sin^m(x)cos^{2k}(x)cos(x)dx = \int sin^m(x)(1-sin^2(x))^kcos(x)dx$, then substitute $u =sin(x)$
2. if m = 2k + 1
   $\int sin^{2k+1}(x)cos^n(x)dx = \int sin^{2k}(x)cos^n(x)sin(x)dx = \int (1-cos^2(x))^kcos^n(x)sin(x)dx$, then substitute $u =cos(x)$
3. both n and m are even
   use $sin(x)cos(x) = \frac{1}{2}sin(2x)$

# for tan(x)sec(x) like

1. n is even
   $\int tan^m(x)sec^{2k}(x) dx = \int tan^m(x)sec^{2k-2}(x) sec^{2}(x)dx = \int tan^{m}x(1+tan^2(x))^{k-1}sec^2(x) dx$
2. m is odd
   $\int tan^{2k+1}(x)sec^{n}(x) dx = \int tan^{2k}(x)sec^{n-1}(x) sec(x)tan(x)dx = \int (sec^2(x)-1)^k sec^{n-1}(x)sec(x)tan(x) dx$
