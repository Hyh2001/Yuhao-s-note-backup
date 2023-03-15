#probability 

Permutation is defined as follow. A permutation of $n$ distinct elements taken $r$ at a time is an arrangement of the $r$ elements. It is a counting[^1] that the order matters. Its calculation formula is represented as follow.

# calculation formula

$P^{n}_{r} = \frac{n!}{(n-r)!}$

If typically the data drawn is needed to be arranged into a circle, the situation will be as follow:

# arrange in circle

The number of permutations of $n$ distinct objects arranged in a circle is $(n − 1)!$

We can use excel to calculate permutations. The function us as follow:

# excel

```excel
PERMUTATIONA(number,number_chosen)
```

[^1]: # counting

    ​#probability#​

    Counting can be defined as follow. In general, if $n$ operations $O_1, O_2, · · · , O_n$ are performed in order, with possible number of outcomes $n_1, n_2, · · · , n_k$ respectively, then there are $n_1n_2 · · · n_k$ possible combined outcomes of the operations performed in the given order. This is also the basic principle of counting. There are two types of countings which based on whether ordered arrangements will include in the counting. They are permutation[^2] and combination[^3].


[^2]: # permutation

    Permutation is defined as follow. A permutation of $n$ distinct elements taken $r$ at a time is an arrangement of the $r$ elements. It is a counting[^1] that the order matters. Its calculation formula is represented as follow.

    # calculation formula

    $P^{n}_{r} = \frac{n!}{(n-r)!}$

    If typically the data drawn is needed to be arranged into a circle, the situation will be as follow:

    # arrange in circle

    The number of permutations of $n$ distinct objects arranged in a circle is $(n − 1)!$

    We can use excel to calculate permutations. The function us as follow:

    # excel

    ```excel
    PERMUTATIONA(number,number_chosen)
    ```

[^3]: # combination

    The definition of combination is as follow. The number of combinations of $n$ distinct objects taken $r$ at a time is
    $C^{n}_{r} = \frac{n!}{r!(n-r)!}$
    $0 \leq r \leq n$

    # properties

    There are some properties of combinations and they are as follow:

    1. $C^{n}_{r} = C^{n}_{n-r}$
    2. $P^{n}_{r} = C^{n}_{r}  \cdot P^{r}_{r}$

    # excel

    We can use excel to help us calculate combinations. The usage of excel is as follow.

    ```excel
    COMBIN(number,number_chosen)
    ```
