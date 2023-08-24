+++
title = "样卷"
tags = ["sample"]
draft = false
+++

1.1 \\( f(z) = x^2 + i y \\), 求 \\( f'( \frac{1}{z} ) \\).

{{< expand >}}
解1. 把 \\( f(z) \\) 看成关于 \\( x, y \\) 的函数, 其中 \\( z = x + iy \\). 那么 \\( f(x + iy) =  f(x, y) = x^2 + iy \\). 记 \\( \overline f = f\left( \frac{1}{z} \right) \\), 故

\begin{aligned}
  \overline f(z) &= f\left( \frac{1}{z} \right) = f\left( \frac{1}{x + iy} \right) \\\\
  &= f\left( \frac{x}{x^2 + y^2} - i\frac{y}{x^2 + y^2} \right) \\\\
  &= f\left( \frac{x}{x^2 + y^2}, -\frac{y}{x^2 + y^2} \right)\\\\
  &= \frac{x^2}{\left(x^2 + y^2\right)^2} -i \frac{y}{x^2 + y^2}
\end{aligned}

根据 Cauchy-Riemann 条件, 上式可微当且仅当
\\[
    \frac{\partial}{\partial x} \left(\frac{x^2}{\left(x^2 + y^2\right)^2}\right) = \frac{\partial}{\partial y} \left(\frac{-y}{x^2 + y^2}\right), \quad
    -\frac{\partial}{\partial y} \left(\frac{x^2}{\left(x^2 + y^2\right)^2}\right) = \frac{\partial}{\partial x} \left(\frac{-y}{x^2 + y^2}\right),
  \\]
也就是
\\[
    (x - 1)^2 + y^2 = 1, x \neq 0
  \\]
故
\\[
    f'\left( \frac{1}{z} \right) = \overline f' (z) = \left( \frac{1}{x^2 + y^2} \right)^2 (-x^2 + y^2 +2xy).
  \\]
解2. 把 \\( z, \bar z \\) 看成独立变量, 则
\\[
    f(z) = x^2 + i y = \left( \frac{z + \bar z}{2} \right)^2 + i \left( \frac{z - \bar z}{2i} \right) =
    \frac{1}{4}\left(z^2 +\bar z ^2 + 2z - 2\bar z + 2z \bar z \right)
  \\]
此时
\\[
    f\left( \frac{1}{z} \right) =
    \frac{1}{4}\left( \frac{1}{z^2} + \frac{1}{\bar z ^2} + \frac{2}{z} - \frac{2}{\bar z} + \frac{2}{z \bar z} \right)
  \\]
由 Cauchy-Riemann 条件有,
\\[
    \frac{\partial}{\partial \bar z} f\left( \frac{1}{z} \right) = 0
  \\]
此时,
\\[
    \frac{\partial}{\partial z}f\left( \frac{1}{z} \right) =
    -\frac{1}{2z^3} - \frac{1}{2z^2} - \frac{1}{2\bar z z^2}
  \\]
{{< /expand >}}

1.2 \\( \int\_{-i}^{i} \left\lvert z \right\rvert \mathrm{d} z = \underline{\hspace{2cm}} \\)  ( \\( -i \\) 到 \\( i \\) 的直线 ).

{{< expand >}}
令 \\( z = it \\), 则
\\[

\begin{aligned}
  \int\_{-i}^{i} \left\lvert z \right\rvert \mathrm{d} z &=
  \int\_{-1}^{1} \left\lvert it \right\rvert i\mathrm{d} t\\\\
  &= i
\end{aligned}

\\]
{{< /expand >}}

1.3 \\( \frac{z^{2023}}{\cos xz} \\) 在 \\( z = -2023 + i \\) 处展开为泰勒级数的收敛半径.

{{< expand >}}
函数 \\( \frac{1}{\cos z} \\) 在 \\( P = \left\lbrace z \neq \frac{\pi}{2} + n \pi, n \in \mathbb{Z} \right\rbrace \\) 时处处可微. 故 \\( \frac{1}{\cos z} \\) 在 \\( z = -2023 + i \\) 收敛半径为 \\( \mathrm{d}(z, \mathbb{C} / P) \\).
所以,\\( \frac{1}{\cos xz} \\) 在 \\( x \neq 0 \\) 时,  收敛半径 为 \\( \frac{ \mathrm{d}(z, P) }{ \left\lvert x \right\rvert } \\);  \\( x = 0 \\) 时, 收敛半径为 \\( \infty \\).
所以, \\( \frac{z^{2023}}{\cos xz} \\) 同理.
{{< /expand >}}

1.4 \\( z^8 - 4z^5 + z^2 -1 \\) 在圆环 \\( 1 < z < 2 \\) 上的零点个数.

{{< expand >}}
应用鲁歇定理, 当 \\( \left\lvert z \right\rvert = 1 \\) 时, \\( \left\lvert -4z^5 \right\rvert > \left\lvert z^8 + z^2 -1 \right\rvert \\), 故 \\( z < 1 \\) 时, 原多项式解个数为 \\( 5 \\).
同理, \\( \left\lvert z \right\rvert = 2 \\) 时, \\( \left\lvert z^8 \right\rvert > \left\lvert -4z^5 + z^2 -1 \right\rvert \\), 故 \\( z < 2 \\) 时, 原多项式解个数为 \\( 8 \\).
不难看出, \\( z = 1 \\)时, 原多项式无解. 故答案为 \\( 3 \\).
{{< /expand >}}

1.5 给出分段线性函数的定义.

{{< expand >}}
形如下面的函数
\\[
    w = \frac{\alpha z + \beta}{\gamma z + \delta}
  \\]
其中, \\( \alpha, \beta, \gamma, \delta \in \mathbb{C} \\).
{{< /expand >}}

1.6 \\( \mbox{Res}\left(z^{2023} \cos ( \frac{1}{z} ), 0\right) = \underline{\hspace{2cm}} \\)  .

{{< expand >}}
即求 \\( z^{2023}\cos \left( \frac{1}{z} \right) \\) Laurent 展式 \\( \frac{1}{z} \\) 项系数, 而
\\[
    z^{2023} \cos ( \frac{1}{z} ) = z^{2023}\left(\sum\_{i = 0} \frac{(-1)^{i}}{(2i)!} \left( \frac{1}{z} \right)^{2i}\right)
  \\]
故答案应为 \\( \frac{1}{2024!} \\)
{{< /expand >}}

2 \\( f(z) = \left\lvert z \right\rvert \\), 问 \\( f \\) 是否可微, 求其解析点.

{{< expand >}}
\\( f(z) = \sqrt{x^2 + y^2} \\).

1.  \\( z \neq 0 \\) 时, 由 Cauchy-Riemann 定理知, \\( f \\) 在 \\( \frac{x}{\sqrt{x^2 + y^2}} = 0, \frac{y}{\sqrt{x^2 + y^2}} = 0 \\) 有 \\( x = y = 0 \\) 矛盾. 即, \\( f \\) 不可微.
2.  \\( z = 0 \\) 时, 极限 \\( \lim\limits\_{z \to 0} \frac{\lvert z \rvert - 0}{z - 0} \\) 不存在, 故也不可微.

综上, \\( \left\lvert f \right\rvert \\) 无处可微.
{{< /expand >}}

3 证明: \\( \left\lvert \oint\_{ \left\lvert z \right\rvert = 1 } \left( x^{2023} + i y^{2023} \right) \mathrm{d} z \right\rvert \leq 2 \pi \\).

{{< expand >}}
\begin{aligned}
  \left\lvert \oint\_{ \left\lvert z \right\rvert = 1 } \left( x^{2023} + i y^{2023} \right) \mathrm{d} z \right\rvert &=
  \left\lvert \int\_{0}^{2\pi} \left(\mathrm{Re}^{2023} \left(e^{it}\right) + i\mathrm{Im}^{2023} \left( e^{it} \right)\right) i e^{it} \mathrm{d} t \right\rvert \\\\
  &= \int\_{0}^{2 \pi} \left\lvert \mbox{Re}^{2023}\left( e^{it} \right) \right\rvert + \left\lvert \mbox{Im}^{2023}\left( e^{it} \right) \right\rvert \mathrm{d} t\\\\
  &= \int\_{0}^{2 \pi} \left\lvert \mbox{Re}^{2}\left( e^{it} \right) \right\rvert + \left\lvert \mbox{Im}^{2}\left( e^{it} \right) \right\rvert \mathrm{d} t\\\\
  &\leq 2\pi.
\end{aligned}
{{< /expand >}}

4 求 \\( \left\lvert z - 1 \right\rvert > 1 \\) 时 \\( f(z) = \frac{1}{z^2} \\) 的洛朗展开.

{{< expand >}}
\begin{aligned}
  f(z) &= \frac{1}{z^2}\\\\
       &= \frac{1}{(z - 1)^2 (1 + \frac{1}{(z - 1)})^2}\\\\
       &= \frac{1}{(z - 1)^2} \left(\sum\_{i = 0} (-1)^i \left(\frac{1}{z - 1}\right)^{i}\right)^2
\end{aligned}
{{< /expand >}}

5 设整函数 \\( f: \mathbb{C} \to D \\), \\( D \\) 为单连通. 若 \\( D \neq \mathbb{C} \\), 证: \\( f \\) 为常数.

{{< expand >}}
由 Riemann 映射原理知, 对任意点 \\( z \in \mathbb{C} \\), 存在单叶函数 \\( g \\), 使得 \\( g \circ f: \mathbb{C} \to O = \left\lbrace z \mid \left\lvert z \right\rvert < 1 \right\rbrace \\), 且 \\( g'(f(z)) > 0 \\).
再由 Liouville 定理知, \\( (g \circ f)' = 0 \\), 这只能 \\( f'(z) = 0 \\). 再由 \\( z \\) 的任意性, 知 \\( f'(z) = 0 \\) 恒成立, 也就是 \\( f(z) \\) 为常数.
{{< /expand >}}

6 \\( f(z) = \frac{1}{ \cos z - \cos \alpha } \\) 在复平面上的所有奇点, 类型, 及其留数.

{{< expand >}}
\\( \alpha = n\pi, n \in \mathbb{Z} \\) 时, 极限 \\( \lim\limits\_{z \to \pm \alpha + 2m \pi} \frac{\left(z - (\pm \alpha + 2m\pi)\right)^2}{\cos z - \cos \alpha} \\) 存在, 其中 \\( m \in \mathbb{Z} \\), 故 \\( 2m\pi \pm \alpha \\) 为二阶极点. 其留数为:
\\[
      \lim\limits\_{z \to \pm \alpha + 2m \pi} \frac{\mathrm{d}(z - (\pm \alpha + 2m \pi))^2 f(z)}{\mathrm{d} z}
    \\]
\\( \alpha \neq n\pi, n \in \mathbb{Z} \\), 极限 \\( \lim\limits\_{z \to \pm \alpha + 2m \pi} \frac{(z - (\pm \alpha + 2m\pi))}{\cos z - \cos \alpha} \\) 存在, 故 \\( \cdots \\) 一阶奇点, 其留数为:
\\[
      \cdots
    \\]
{{< /expand >}}

7 求 \\( \oint\_{ \left\lvert z \right\rvert = 2023 } \tan \pi z \mathrm{d} z \\) 和 \\( \int\_{-\infty}^{\infty} \frac{\cos x}{x^2 + a^2} \mathrm{d} x, (\alpha > 0) \\).

{{< expand >}}
1.  设 \\( \tan \pi z \\) 在 \\( z \leq 2023 \\) 的奇点集为 \\( P \\), 那么
    \\( \oint\_{ \left\lvert z \right\rvert = 2023 } \tan \pi z \mathrm{d} z = 2\pi i\sum\_{p \in P} \mathrm{Res}(f, p) \\).
2.  \\( \cdots \\).
{{< /expand >}}
