# softmax

## 数学表示

$o_i = x_1w_{1i}+x_2w_{2i} +...+x_nw_{ni}+b_i$
$y = [y_1,y_2,...y_n]^T = [0,0,0,0,1,0,..,0]$
$yi = 1$ if $i = y, yi =0$ otherwise
$y_i^\hat{} = argmax o_i$
置信度需要：
$o_y - o_i \geq \delta(y,i)$

## 输出匹配概率（加和为1）

$y^\hat{} = softmax(o)$
$y^\hat{}_i = exp(o_i)/\sum_{}^kexp(o_k)$

### 损失函数：交叉熵（用于概率）

$l(y,y^\hat{}) = -log(y^\hat{}_y)$
$\partial_{oi}l(y,y^\hat{}) = softmax(o)_i- y_i$

## pytorch 实现

	import torchvision
	from torchvision import transforms
