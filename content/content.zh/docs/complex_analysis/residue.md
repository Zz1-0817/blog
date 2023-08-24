+++
title = "余数及其应用"
tags = ["residue"]
draft = false
weight = 1005
+++

## 余数及其应用 {#余数及其应用}


### 留数 {#留数}

设 \\( f(z) \\) 在 \\( 0 < \left\lvert z - z\_0 \right\rvert < R \\) 内解析, 其中 \\( z\_0 \\) 为 \\( f(z) \\) 的孤立奇点. 令 \\( 0 < r < R \\), 那么下式
\\[
      \frac{1}{2 \pi i} \int\_{ \left\lvert z - z\_0 \right\rvert = r } f(z) \mathrm{d} z
     \\]
称为函数 \\( f(z) \\) 在 \\( z\_0 \\) 处的留数. 并记作 \\( \mbox{Res}(f, z\_0) \\).


### 留数的计算 {#留数的计算}

容易看出, \\( \mbox{Res}(f, z\_0) \\) 就是 \\( f(z) \\) 在 \\( z\_0 \\) 的 Laurent 展式中 \\( \frac{1}{z - z\_0} \\) 的系数. 那么, \\( z\_0 \\) 为 \\( k \\) 阶极点时, 有
\\[
      \mbox{Res}(f, z\_0) = \frac{1}{(k - 1)!} \lim\limits\_{z \to z\_0} \frac{\mathrm{d}^{k - 1}\left[(z - z\_0)^{k}f(z)\right]}{\mathrm{d}z^{k - 1}} \tag{1}\label{residue}
     \\]

{{< expand >}}
设 \\( f(z) = \sum\_{n = -\infty}^{\infty} \alpha\_n(z - z\_0)^{n} \\), 那么,

\begin{aligned}
\mbox{Res}(f, z\_0) &= \frac{1}{2 \pi i} \int\_{ \left\lvert z - z\_0 \right\rvert = r } f(z) \mathrm{d} z\\\\
&= \frac{1}{2 \pi i}\int\_{ \left\lvert z - z\_0 \right\rvert = r } \sum\_{n = -\infty}^{\infty} \alpha\_n(z - z\_0)^{n} \mathrm{d} z\\\\
&= \frac{1}{2 \pi i} \sum\_{n = -\infty}^{\infty} \int\_{ \left\lvert z - z\_0 \right\rvert = r }  \alpha\_n(z - z\_0)^{n} \mathrm{d} z\\\\
&= \alpha\_{-1}
\end{aligned}

同时, 若 \\( z\_0 \\) 是 \\( f \\) 的 \\( k \\) 阶极点, 则可以设 \\( f(z) = \alpha\_{-k}\left(\frac{1}{z - z\_0}\right)^{k} + \alpha\_{-k + 1}\left(\frac{1}{z - z\_0}\right)^{k - 1} + \cdots \\), 考虑 \\( (z - z\_0)^{k}f(z) \\), 其 \\( k - 1 \\) 阶导数为
\\[
     (k - 1)!\alpha\_{-1} + k! \alpha\_0 (z - z\_0) + (k + 1)!(z - z\_0)^{2} + \cdots
     \\]
立刻得到了公式\ref{residue}.
{{< /expand >}}


### 留数的应用 {#留数的应用}
