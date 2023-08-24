+++
title = "Taylor 展开和 Laurent 展开"
tags = ["expansion"]
draft = false
weight = 1004
+++

## Taylor 展开和 Laurent 展开 {#taylor-展开和-laurent-展开}


### 幂级数收敛半径的求职公式 {#幂级数收敛半径的求职公式}

如果下列条件之一成立

\begin{aligned}
  &l = \lim\limits\_{n \to +\infty} \left\lvert \frac{ \alpha\_{n + 1} }{ \alpha\_{n}} \right\rvert,\\\\
  &l = \lim\limits\_{n \to +\infty} \sqrt[n]{\left\lvert \alpha\_n \right\rvert}, \\\\
  &l = \overline\lim\limits\_{n \to +\infty} \sqrt[n]{\left\lvert \alpha\_n \right\rvert},
\end{aligned}


### Taylor 级数 {#taylor-级数}

设函数 \\( f(z) \\) 在圆盘 \\( U: \left\lvert z - z\_0 \right\rvert < R \\) 内解析, 那么在 \\( U \\) 内有

\begin{aligned}
 f(z) &= f(z\_0) + \frac{f'(z\_0)}{1!}(z - z\_0) + \frac{f^{(2)}(z\_0)}{2!}(z - z\_0)^2 + \cdots \\\\
      &= \frac{f^{(n)}(z\_0)}{n!}(z - z\_0)^n + \cdots
\end{aligned}


### Laurent 级数 {#laurent-级数}

设函数 \\( f(z) \\) 在圆环 \\( D: R\_1 < \left\lvert z - z\_0 \right\rvert < R\_2, ( 0 \leq R\_1 < R\_2 \leq +\infty \\) 内解析, 那么在 \\( D \\) 内,
\\[
     f(z) = \sum\_{n = -\infty}^{+\infty}  \alpha\_n (z - z\_0)^n
    \\]
这里
\\[
     \alpha\_n = \frac{1}{2 \pi i} \int\_{\gamma} \frac{f(z)}{(z - z\_0)^{n + 1}}\mathrm{d} z, \quad (n = 0, \pm 1, \pm 2)
    \\]


### Taylor 级数和 Laurent 级数的唯一性 {#taylor-级数和-laurent-级数的唯一性}

-   在圆盘 \\( U: \left\lvert z - z\_0 \right\rvert < R \\)中, 幂级数 \\( \sum\_{n = 0}^{\infty} \alpha\_n(z - z\_0)^{n} \\) 的和函数没有另一种形如 \\( \sum\_{n = 0}^{\infty} \beta\_n(z - z\_0)^{n} \\) 的幂级数.
-   在圆环 \\( U: 0 < \left\lvert z - z\_0 \right\rvert < R \\)中, 幂级数 \\( \sum\_{n = -\infty}^{\infty} \alpha\_n(z - z\_0)^{n} \\) 的和函数没有另一种形如 \\( \sum\_{n = -\infty}^{\infty} \beta\_n(z - z\_0)^{n} \\) 的幂级数.


### 孤立奇点 {#孤立奇点}

设函数 \\( f(z) \\) 在去心圆盘 \\( D = \left\lbrace 0 < \left\lvert z - z\_0 \right\rvert < R \right\rbrace, (0 < R < +\infty) \\) 内确定并解析, 而在 \\( z\_0 \\) 不解析, 那么称 \\( z\_0 \\) 为 \\( f(z) \\) 的孤立奇点. 在 \\( D \\) 中 \\( f(z) \\) 有 Laurent 展式
\\[
     f(z) = \sum\_{n = -\infty}^{+\infty}  \alpha\_n (z - z\_0)^n
    \\]

-   \\( n = -1, -2, -3, \cdots \\) 时, \\( \alpha\_n = 0 \\). 我们称 \\( z\_0 \\) 是一个可去奇点;
-   如果有有限个 \\( n < 0 \\), 使 \\( \alpha\_n \neq = 0 \\), 那么我们称 \\( z\_0 \\) 是一个极点. 若 \\( \alpha\_m \neq 0, \alpha\_n = 0, \forall n < m \\) 那么我们称 \\( z\_0 \\) 是一个 \\( m \\) 阶极点.
-   若有无限个 \\( n < 0 \\), 使 \\( \alpha\_n \neq 0 \\) 我们称 \\( z\_0 \\) 是 \\( f(z) \\) 的本质奇点.


### 判断孤立奇点类型的充要条件 {#判断孤立奇点类型的充要条件}


#### 可去奇点 {#可去奇点}

设函数 \\( f(z) \\) 在 \\( 0 < \left\lvert z - z\_0 \right\rvert < R, 0 < R \leq +\infty \\) 内解析, \\( z\_0 \\) 是 \\( f(z) \\) 的奇点, 那么以下等价

-   \\( z\_0 \\) 是 \\( f(z) \\) 的可去奇点;
-   存在极限 \\( \lim\limits\_{z \to z\_0}f(z) = \alpha\_0, \alpha\_0 \in \mathbb{C} \\);
-   \\( f(z) \\) 在 \\( z\_0 \\) 的某个邻域内有界.


#### 极点 {#极点}

-   设函数 \\( f(z) \\) 在 \\( 0 < \left\lvert z - z\_0 \right\rvert < R, 0 < R \leq +\infty \\) 内解析, \\( z\_0 \\) 是 \\( f(z) \\) 的极点当且仅当 \\( \lim\limits\_{z \to z\_0}f(z) = \infty \\).
-   设函数 \\( f(z) \\) 在 \\( 0 < \left\lvert z - z\_0 \right\rvert < R, 0 < R \leq +\infty \\) 内解析, \\( z\_0 \\) 是 \\( f(z) \\) 的 \\( m \\) 阶极点当且仅当 \\( \lim\limits\_{z \to z\_0}(z - z\_0)^{n}f(z) \\) 存在且有限.


### 亚纯函数 {#亚纯函数}

如果一个函数在有限复平面上除去极点外处处解析, 那么这个函数称为亚纯函数.
