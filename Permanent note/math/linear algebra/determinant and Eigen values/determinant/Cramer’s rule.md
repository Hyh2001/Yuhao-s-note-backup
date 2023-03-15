For $Ax = b$, the solution of this linear equations are 
$x_{1}= \frac{det(B_{1})}{det(A)}$, $x_2 = \frac{detB_2}{detA}$, $\ldots$, $x_{n}= \frac{det(B_n)}{det(A)}$
The matrix $B_j$ has the $jth$ column of $A$ replaced by the vector $b$
([“introduction to linear algebra”, p. 284](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=284&annotation=QNYMNZDN))  


# proof of the rule 
The rule is inspected as follow: 
For a linear equation system $Ax = b$. 
If we replace the first column of $I$ the [[identity matrix]] with $x$, then we will get $\begin{bmatrix} x_{1} & 0&0\\x_{2}&1&0\\x_{3}&0&1\end{bmatrix}$ and we denoted is as $M$
Then $AM = \begin{bmatrix}b & A_{2}& A_{3}\end{bmatrix} = B_1$  where $A_2$ and $A_3$ denote the $2$ and $3$ column of $A$. 
We calculate the [[determinant]] of the both sides and we will get $det (A) det (M) = det(B_1)$. 
We can see that $det (M) = x_1$ by using the cofactor method. 
Then $x_{1}= \frac{det(B_1)}{det(A)}$ .
Then iteratively we can get $x_{n}= \frac{det(B_n)}{det(A)}$. 
([“introduction to linear algebra”, p. 283](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=283&annotation=K7YAPH2C))

