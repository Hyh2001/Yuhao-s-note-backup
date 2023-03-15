由命题([[proposition]])组合而成的式子。值只有T（true）或F（false）

## 组合方式

### NOT（—）

$T \to F$
$F \to T$

### AND（&&）

$T \quad T \to T$
$T \quad F \to F$
$F \quad T \to F$
$F \quad F \to F$

### OR（||）

$T \quad T \to T$
$T \quad F \to T$
$F \quad T \to T$
$F \quad F \to F$

### XOR ($\oplus$)

$T \quad T \to F$
$T \quad F \to T$
$F \quad T \to T$
$F \quad F \to F$

### IFF 当且仅当($\iff$)

$T \quad T \to T$
$T \quad F \to F$
$F \quad T \to F$
$F \quad F \to T$

### IMPLIES（$\to$)

$T \quad T \to T$
$T \quad F \to F$
$F \quad T \to T$
$F \quad F \to T$

## truth table（ 真值表）

被用于表达命题的真假
真值相同的表达式是等价的

### 简化逻辑表达式

加快执行速度

## properties

### 等价性

#### 逆否

逆否命题等价于蕴涵

#### 逆否 AND 蕴涵

$P \quad IFF \quad Q = (P \quad IMIPLIES \quad Q) AND (Q \quad IMPLIES \quad P)$

### 永真性

总是为真的公式

### 可满足性

有时侯为真的公式
式$P$是可满足的，当且仅当 $NOT(P)$不是永真式
