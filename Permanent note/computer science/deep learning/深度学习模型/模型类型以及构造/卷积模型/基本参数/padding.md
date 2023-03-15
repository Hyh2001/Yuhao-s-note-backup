---

aliases: [填充]

---

# definition

在输⼊图像的边界填充元素（通常填充元素是0）

## method

[[卷积]]核的⾼度和宽度通常为奇数，填充时上下填充相同数量的行，左右填充相同数量的列
$p_h = k_h - 1$
$p_w = k_w -1$

### 输出形状

$(n_k -k_h +p_h +1) \times (n_w -k_w + p_w  +1)$

## pytorch 实现

```python 
nn.Conv2d(1, 1, kernel_size=(5, 3), padding=(2, 1)) # padding = (m,n) m表示单边填充的列数，n表示单边填充的行数。总共填充数为2m列，2n行
```
