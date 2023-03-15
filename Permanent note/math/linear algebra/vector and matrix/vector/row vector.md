It is the [[vector]]  that writes from left to right

‍

‍

‍

‍

‍

1. [ROB_101_December_2021_Grizzle - Excerpt of: ROB_101_December_2021_Grizzle, p27](lt://open/DrIEJEfByU2irEG8s2PqjA)

‍

[^1]: # vector

    ​#linear algebra#​ #calculus#​

    It is the special objects that can be added together and multiplied by scalars to produce another object of the same kind. It is in a form of a finite **ordered** list of numbers or unknowns. $^{[2]}$ Same vector can have different endpoints, they only need to have the same magnitude and direction. There are two types of vectors. column vector[^2]s and row vector[^3]s

    ## real life counterparts:

    1. Audio signals
    2. $R^n$
    3. array[^4] (used in Machine learning[^6])
    4. place of a point in a space

    ## representation of vector

    1. a line with directions in the space
    2. use coordinates in $n$-dimensional spaces

    # calculation law:

    ## vector addition

    Vector addition obeys parallelogram rule[^7]

    In coordinates form, $\vec{a} + \vec{b} = (a_1 + b_1, a_2 + b_2,...a_n+b_n)$ where $a_1,a_2,... b_1,b_2,..$ are coordinates of $\vec{a}, \vec{b}$

    ## vector multiplication

    ### by scalars

    $c \cdot \vec{a} = c\vec{a}$  

    In coordinates form, $c\vec{a} = (ca_1 , ca_2 ,...,ca_n)$ where $a_1,a_2,...$ are coordinates of $\vec{a}$

    #### parallel vectors

    Two vectors $\vec{s},\vec{t}$ are parallel to each other if and only if there exists a real number $a$ such that $\vec{s} = a\vec{t}$. Based on the principle, we can find that the zero vector[^8] $O$ is parallel to all vectors.

    ### dot product[^9]

    $v \cdot w = v_1w_1 + v_2w_2$  

    ### cross product[^11]

    # special vectors:

    1. unit vector[^14] : $u = v/||v||$
    2. zero vector[^8]

    # programming impletation of vector

    ## Julia

    ```julia
    a = [1 -2 4 8.1 2^0.5] # 1 * 5 matrix 
    b = [1, -2, 4, 8.1, 2^0.5] # 5 * 1 matrix 
    c = [1; -2; 4; 8.1; 2^0.5] # another representation of 5 * 1 matrix
    ```
    ## 

    ‍

    ‍

    1. ‍
    2. [ROB_101_December_2021_Grizzle - Excerpt of: ROB_101_December_2021_Grizzle, p27](lt://open/Awf0qGUlxEaKidzJdZ0Qtw)
    3. [mathematical analysis - Excerpt of: Second Year Calculus From Celestial Mechanics t... (z-lib.org), p17](lt://open/5-xhoqEwDEyWwLPg5Yg6bA)

    ‍


[^2]: # column vector

    It is the vector[^1] that writes from up to down.

    ‍

    ‍

    ‍

    ‍

    1. [ROB_101_December_2021_Grizzle - Excerpt of: ROB_101_December_2021_Grizzle, p27](lt://open/fCadEsmSx06gQU5oPTMgtA)


[^3]: # row vector

    It is the vector[^1] that writes from left to right

    ‍

    ‍

    ‍

    ‍

    ‍

    1. [ROB_101_December_2021_Grizzle - Excerpt of: ROB_101_December_2021_Grizzle, p27](lt://open/DrIEJEfByU2irEG8s2PqjA)

    ‍


[^4]: # array

    Array are scalar[^5]s that have been organized into lists. They could be columns of numbers or rows of numbers.

    ‍

    ‍

    ‍

    # reference 

    1. [ROB_101_December_2021_Grizzle - Excerpt of: ROB_101_December_2021_Grizzle, p27](lt://open/oN2H8AYGtk2C60MO1QqmrQ)


[^5]: # scalar

    ‍


[^6]: # Machine learning

    ‍


[^7]: # parallelogram rule

    Parallelogram rule is used to add two vectors. 

    ​![image](assets/image-20221214121843-95tdyw1.png)​

    # properties of parallelogram rule

    1. commutative

        $\vec{r} + \vec{s} = \vec{s} + \vec{r}$
    2. associative

        $(\vec{r} + \vec{s}) + \vec{t} = \vec{r} + (\vec{s} + \vec{t})$
    3. distributive

        $(a+b)\vec{r} = a\vec{r} + b\vec{r}$

    ‍


[^8]: # zero vector

    ‍


[^9]: # dot product

    Dot product is denoted as $\vec{a} \cdot \vec{b}$ where $\vec{a} \cdot \vec{b} = |a||b|cos\theta$ where $\theta$ is the angle between the two vectors.

    ## properties of dot product

    1. Dot product is $0$ if two vectors are perpendicular[^10] to each other.
    2. Dot product is commutative

        $\vec{s} \cdot \vec{r} = \vec{r} \cdot \vec{s}$

    ## dot products for finding angles between two vectors

    $u \cdot v /||u||||v||= cos \theta$  

    ## dot products for finding length of a vector

    $||v|| = \sqrt[]{v \cdot v}=\sqrt[]{v_1^2+v_2^2+...+v_n^2}$  where $v_1,v_2,...,v_n$ are coordinates of a vecotr

    ### properties

    $|v \cdot w| \leq ||v||||w||$  
    ​$||v + w|| \leq ||v|| + ||w||$  

    proof: 


[^10]: # perpendicular

    ​#todo#​ 


[^11]: # cross product

    ​#calculus#​ #linear algebra#​ 

    ‍

    # bracket notation of cross product

    We can use a skew-symmetric matrix[^12] to represent cross product of two vectors. It can be done as follow:

    For $\omega \times R$, we can have $[w]$ as the skew-symmetric matrix of $w$ and $\omega \times R = [\omega]R$  

    ## why cross product can be represented by skew-symmetric matrix?

    ​#todo#​ 


[^12]: # skew-symmetric matrix

    Given a vector $x = [x_1 \quad x_2 \quad  x_3]^T \in \mathbb{R}^3$ 

    we can define: 

    $[x] = \begin{bmatrix}0 & -x_3 & x_2 \\ x_3 & 0 & -x_1 \\ -x_2 & x_1 & 0 \end{bmatrix}$ This is a skew-symmetric matrix

    # property

    It has the property that: $[x] = -[x]^T$. The set of all 3 by 3 real skew-symmetric matrices is called $so(3)$(Lie algebra[^13]).

    # programming implementation

    ```matlab
    % find the skew-symmetric form of a vector omg
    so3mat = VecToso3(omg)
    % find the  3 by 3 vector correspond to a skew-symmetric matrix
    omg = so3ToVec(so3mat)
    ```

[^13]: # Lie algebra

    ‍


[^14]: # unit vector

    A vector whose length equals one.

    ## properties

    $v \cdot v =1$
