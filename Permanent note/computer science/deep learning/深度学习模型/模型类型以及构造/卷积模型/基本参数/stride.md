---

aliases: [步幅]

---

每次滑动元素的数量

## 输出形状

$[(n_k -k_h +p_h +s_h)/s_h] \times [(n_w -k_w + p_w  +s_w)/s_w]$

## pytroch 实现

	nn.Conv2d(1, 1, kernel_size=(3, 5), padding=(0, 1), stride=(3, 4))
