+++
title = "Riemann 映射定理"
tags = ["riemann-theorem"]
draft = false
weight = 1006
+++

## Riemann 映射定理 {#riemann-映射定理}


### 最大模原理 {#最大模原理}

如果函数 \\( w = f(z) \\) 在区域 \\( D \\) 解析, 并且 \\( \left\lvert f(z) \right\rvert \\) 在 \\( D \\) 内某一点达到最大值, 那么 \\( f(z) \\) 在 \\( D \\) 内恒等于一常数.


### Schwartz 引理 {#schwartz-引理}

设 \\( f(z) \\) 是在开圆盘 \\( \left\lvert z \right\rvert < 1 \\) 内的解析函数. 设 \\( f(0) = 0 \\), 并且当 \\( \left\lvert z \right\rvert < 1 \\), \\( \left\lvert f(z) \right\rvert < 1 \\). 那么

-   当 \\( \left\lvert z \right\rvert < 1 \\) 时, \\( \left\lvert f(z) \right\rvert \leq \left\lvert z \right\rvert \\);
-   \\( \left\lvert f'(0) \right\rvert \leq 1 \\);
-   如果对于某一复数 \\( z\_0 ( 0 < \left\lvert z\_0 \right\rvert < 1 ), \left\lvert f(z\_0) \right\rvert = \left\lvert z\_0 \right\rvert \\), 或者如果 \\( \left\lvert f'(0) \right\rvert = 1 \\), 那么在 \\( \left\lvert z \right\rvert < 1 \\) 内,
    \\[
            f(z) = \lambda z
            \\]
    其中 \\( \lambda \\) 是一复常数, 且 \\( \left\lvert \lambda \right\rvert = 1 \\).


### Riemann 映射定理 {#riemann-映射定理}

设 \\( D \\) 是 \\( z \\) 平面 \\( \mathbb{C} \\) 上任何单连通区域, 但不是整个平面; 设 \\( z\_0 \in D \\), 那么有且仅有一个在区域 \\( D \\) 内的单叶函数 \\( w = f(z) \\), 满足 \\( f(z\_0) = 0, f'(z\_0) > 0 \\), 并且把 \\( D \\) 保形双射成 \\( \left\lvert w \right\rvert < 1 \\).
