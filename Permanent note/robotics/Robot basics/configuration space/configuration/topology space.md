# topology space

a topological space is a set[^1] whose elements are called [points](https://en.wikipedia.org/wiki/Point_(geometry)) "Point (geometry)"), along with an additional structure called a topology[^3].

# one-dimensional spaces

There are several types of one-dimensional spaces:

1. circle($S$)
2. line($\mathbb{E}$)(It equals to a line with open interval) and
3. a closed interval of the line($[a,b] \subset \mathbb{R}$, $\mathbb{R}$ means a point in $\mathbb{E}$) Also $n$-dimensional spaces.

# two-dimensional spaces

1. plane($\mathbb{E}^2$)
2. sphere($S^2$)
3. torus($T^2 = S^1 * S^1$)
4. sphere($E^1 * S^1$)

# n-dimensional spaces

$\mathbb{R}^n$ is the $n$-dimensional Euclidean space. $S^n$ is the $n$-dimensional surface of a sphere in $(n+1)$-dimensional space

[^1]: # set

    集合(set)就是一堆对象，对象称为集合中的元素(element)

    ## representation

    $A = \{ \quad \}$

    ## properties

    1. 元素没有顺序
    2. 元素各不相同

    ## 集合间关系

    ### 并集(union)

    $x \in A \cup B$  IFF $x \in A$  OR  $x \in B$

    ### 交集（intersection）

    $x \in A \cap B$  IFF $x \in A$  AND  $x \in B$

    ### 差集（difference）

    $x \in A - B$  IFF $x \in A$  OR  $x \notin B$

    ### 补集（complement)

    认为所有集合是一个已知全域$D$的子集，对于$D$的任意子集$A$，定义$\bar{A}$表示$D$中所有不属于$A$的元素

    ### 相等

    如果两个集合拥有完全相等的元素，它们相等
    $A = B$  IFF  $\forall x \in A, \exists y \in B, x =y$  AND  $\forall x \in B, \exists y \in A, x =y$

    #### 集合相等证明

    用iff定理形式化证明

    ## 幂集（power set)

    集合$A$所有的子集构成的集合
    $B \in pow(A)$  IFF $B \subseteq A$

    ### 幂集的个数

    $A$有$n$个元素，则幂集有$2^n$个集合

    ## 集合构造器标记（set builder notation)

    使用谓词(predicate[^2])定义集合  
    例子  
    ​$A = \{ n \in \mathbb{N} |  n 是 质数\}$  

    ## 集合运算

    ### 笛卡尔积（Cartesian product）

    $S_1 \times S_2 \times ... S_n$，是一个由序列构成的新集合序列的第一个组件来自$S_1$，第二个组件来自$S_2$ ....

    #### 理解

    <font color="00FF00" size="3">从相乘的每个集合中每次抽出一个元素置于一个序列中。这个元素的位置由该集合是第几个乘数决定</font>
    ### distributive laws of sets
    $A \cap (B \cup C)) = (A \cap B) \cup (A \cap C)$
    ### DeMorgan's laws:
    $\bar{(A \cap B)} = \bar{A} \cup \bar{B}$
    $\bar{(A \cup B)} = \bar{A} \cap \bar{B}$

[^2]: # predicate

    ### predicate

    The part which tells something about the subject

    #### object


[^3]: # topology

    Topology is a structure which allows defining continuous deformation of subspaces. *It is independent of how we choose coordinates to represent points in the ​*topology space[^4]. We define some spaces are topologically equivalent[^5].

    ‍

    “topology” ([Lynch 和 Park, 2017, p. 21](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=21&annotation=RG8BIS2P)) 

    ‍


[^4]: # topology space

    a topological space is a set[^1] whose elements are called [points](https://en.wikipedia.org/wiki/Point_(geometry)) "Point (geometry)"), along with an additional structure called a topology[^3].

    # one-dimensional spaces

    There are several types of one-dimensional spaces:

    1. circle($S$)
    2. line($\mathbb{E}$)(It equals to a line with open interval) and
    3. a closed interval of the line($[a,b] \subset \mathbb{R}$, $\mathbb{R}$ means a point in $\mathbb{E}$) Also $n$-dimensional spaces.

    # two-dimensional spaces

    1. plane($\mathbb{E}^2$)
    2. sphere($S^2$)
    3. torus($T^2 = S^1 * S^1$)
    4. sphere($E^1 * S^1$)

    # n-dimensional spaces

    $\mathbb{R}^n$ is the $n$-dimensional Euclidean space. $S^n$ is the $n$-dimensional surface of a sphere in $(n+1)$-dimensional space


[^5]: # topologically equivalent

    we can define topologically equivalent between two surfaces as: if one can be continuously deformed into the other without cutting or gluing.
