+++
title = "解析函数的性质"
tags = ["property"]
draft = false
weight = 1003
+++

## 解析函数的性质 {#解析函数的性质}


### Cauchy 定理 {#cauchy-定理}

设 \\( f(z) \\) 是单连通区域 \\( D \\) 内的解析函数, 那么
设 \\( C \\) 是 \\( D \\) 内的一条简单闭合曲线, 那么
\\[
	\int\_C f(z) \mathrm{d} z = 0
    \\]


### Cauchy 公式 {#cauchy-公式}

设 \\( D \\) 是以有限条简单闭合曲线为边界的有界区域. 设 \\( f(z) \\) 在 \\( D \\) 及 \\( C \\) 所组成的闭区域 \\( \overline D \\) 上解析, 那么在 \\( D \\) 内任意点 \\( z \\), 下式
\\[
    f(z) = \frac{ 1 }{ 2\pi i } \int\_C \frac{ f(\xi) }{ \xi - z } \mathrm{d} \mathrm{d} \xi
    \\]
称为 Cauchy 公式. 而且, \\( f(z) \\) 在 \\( D \\) 内有任意阶导数
\\[
    f^{(n)}(z) = \frac{ n! }{ 2\pi i } \int\_C \frac{f(\xi)}{(\xi - z)^{n + 1}} \mathrm{d}\xi, \quad n = 1, 2, \cdots
    \\]


### Liouville 定理 {#liouville-定理}

有界整函数一定恒等于整数
