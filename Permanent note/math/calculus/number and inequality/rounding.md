Rounding is a process to estimate a particular number in a context. There are two types of rounding: 
**1. Round up**
**2. Round down**
0.7957 rounded down to 3 digit is 0.795, rounded down to 3 digit is 0.796.  <!--SR:!2023-03-15,3,250-->

The process of rounding a number $a$ to $m$ decimals starts with finding the interval of length $10^{-m}$. 


# Round for comparing numbers
The operation of rounding makes it clear by how much two numbers in decimal form differ. 
## Theorem   
If $a$ and $b$ are two numbers given in decimal form and if one of the two roundings of $a$ to $m$ digits agrees with one of the two roundings of $b$ to $m$ digits, then **$|a − b| < 2 \times 10^{−m}$.** <!--SR:!2023-03-14,1,210-->

Conversely, if we are given the difference between two numbers, we can predict their roundings. 

If the distance between a and b is less than $10^{-m}$, then one of the roundings of $a$ to $m$ digits agrees with one of the roundings of $b$ to $m$ digits.

# Rounding and computer algorithms
The implementation of computer algorithms always involves rounding errors. ([Lax 和 Terrell, 2014, p. 17](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=30&annotation=EMW9HVS2))
## rounding for [[floating point number]] 
If $m \leq |x| \leq M$, then the floating point number representation of $x$ is $fl (x) = min_{f \in F}|f-x|$  
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=38&annotation=QAK7W7DP))



1. Rounding up and down ([Lax 和 Terrell, 2014, p. 16](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=29&annotation=BQ6JKWES))
2. Find rounding  ([Lax 和 Terrell, 2014, p. 16](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=29&annotation=EZQPPI33))
3. Rounding for comparing numbers ([Lax 和 Terrell, 2014, p. 16](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=29&annotation=6DHGLACZ))
4. Theorem for comparing numbers ([Lax 和 Terrell, 2014, p. 16](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=29&annotation=85LG52UW))
5. Converse theorem ([Lax 和 Terrell, 2014, p. 16](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=29&annotation=J2Z9DEIT))

