+++
title = "解析函数及其例子"
tags = ["analytic-function"]
draft = false
weight = 1002
+++

## 解析函数及其例子 {#解析函数及其例子}


### 复函数可微的定义 {#复函数可微的定义}

设 \\( f(z) \\) 是在区域 \\( D \\) 内确定的单值函数, 并且 \\( z\_0 \in D \\) 如果
\\[
       \lim\limits\_{z \to z\_0, z \in D} \frac{f(z) - f(z\_0)}{z - z\_0}
     \\]
存在, 并且等于复数 \\( \alpha \\), 那么我们说 \\( f(z) \\) 在 \\( z\_0 \\) 可微或可导, 或者有导数 \\( \alpha \\), 记作 \\( f'(z\_0) \\).


### Cauchy-Riemann 条件 {#cauchy-riemann-条件}

设函数 \\( f(z) = u(x, y) + iv(x, y) \\) 在区域 \\( D \\) 内确定, 那么 \\( f(z) \\) 在点 \\( z = x + iy \in D \\) 可微的必要充分条件是: 在点 \\( z = x + iy, u(x, y), v(x, y) \\) 可微, 并且
\\[
       \frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \quad
       \frac{\partial u}{\partial y} = - \frac{\partial v}{\partial x}.
     \\]
且, \\( f(z) \\) 有导数的条件下, 有
\\[
       f'(z) = a + ib = \frac{\partial u}{\partial x} + i \frac{\partial v}{\partial x} = \frac{\partial v}{\partial y} - i \frac{\partial u}{\partial y}.
     \\]

{{< hint info >}}
将 \\( z, \bar z \\) 看成独立变量, 记 \\( \frac{\partial f}{\partial z} = \frac{1}{2} \left( \frac{\partial f}{\partial x} - i\frac{\partial f}{\partial y} \right), \frac{\partial f}{\partial \bar z} = \frac{1}{2} \left( \frac{\partial f}{\partial x} + i\frac{\partial f}{\partial y} \right) \\), 那么 Cauchy-Riemann 条件等价于 \\( \frac{\partial f}{\partial \bar z} = 0 \\), 而 \\( f'(z) = \frac{\partial f}{\partial z} \\).
{{< /hint >}}
