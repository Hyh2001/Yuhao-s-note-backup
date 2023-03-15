For a **[[continuity|continuous]]** function $f(x)$ on $[a,b]$ with **$f (a) f (b)<0$.** (This prerequisite makes sure that the function has one or more than one [[root]] ) ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=13&annotation=CAT3PTVA))
# Procedure
The procedure of the method for situation with only one root is as follow: 
1. We take **$x_{0}= \frac{a+b}{2}$** and if **$x_{0} = 0$** then we can say that we have found the root. 
2. If $f(x_0)f(a)>0$ then we let **$a_{1}= x_0$ and $b_{1}= b$**
3. If $f (x_{0}) f (a) < 0$ then we let **$a_{1}=a$ and $b_{1} = x_0$**
4. Then repeat the procedure with $[a_1,b_1]$ where $b_{1} -a_{1} = \frac{b-a}{2}$ 
5. We can define an $\epsilon$ as the stopping criterion where the error between the final result gotten by the algorithm $x^{*}= \frac{a_n+b_n}{2}$ and the real result $x$ will have the relationship: **$|x-x^*|<\epsilon$**  
 ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=16&annotation=BS844USS))
# advantages of the method 
1. The method at least converges **linearly** ([[order of convergence]] )
2. It only needs to assume that $f$ is [[continuity]] and no restriction on **derivatives**. 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=83&annotation=T77Q84IQ))
# Program implementation
```matlab
f = inline('x^3 -x-1');
LoopTime = 0; a = -1; b= 1.5; x= (a+b)/2; 
while abs(b-a)/2 >= 0.005  
	% The criterion can be understood in this way:
	% If we want the error less then 0.005 then we can make the length of half of the domain less than it because the error is |x - x^*|
	% In this way, the biggest error will be (b-a)/2 
	if sign(f(x)) == sign(f(b))
		b = x
	else 
		a = x
	end  
	LoopTime = LoopTime + 1
	x = (a+b)/2
	if f(x) == 0, break
end 
```
<!--SR:!2023-03-09,3,250-->








