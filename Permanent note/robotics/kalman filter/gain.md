#control
express the tradeoff

## characteristics

extreme values:
1.when g=1, previous state doesn't matter.
2.when g=0,observation has no effect, xk=xk-1

	As a result, with g bigger, obesrvation matters more, with g smaller, previous state matters more.

### computation of gain

from average noise r.
![[Pasted image 20211008110623.png]]

	with pk-1 small, gk is samll -> previous state matters more,
	with pk-1 big,gk is big -> observation matters more.

pk is prediction error that is computed recursively
![[Pasted image 20211008110648.png]]

	when gk is small, difference between two error is small.
