---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/f-tensors-and-summation-conventions/px-275-f2-summation-conventions/","noteIcon":"1","created":"2025-08-27T13:14:32.612+01:00","updated":"2024-12-02T18:56:21.000+00:00"}
---

- taking a vector $\vec a:$
$$\vec a = a_{x}\hat i  + a_{y}\hat j + a_{z}\hat k = \sum\limits_{i=1}^{3} a_{i}x_{i}$$
	where, $x_{1} = \hat i$, $a_{1} = a_{x}$, and so on
- this can be written as:
$$\vec a = a_{i}\,x_i$$

- considering two vectors:
$$\vec a = a_{i}x_{i} \;;\; \vec b = b_{j}x_{j}
$$
- the dot product:
$$\vec a \cdot \vec b = a_{x}b_{x}+ a_{y}b_{y}+ a_{z}b_{z} = \delta_{ij}a_{i}b_{j}$$
	where, the kronecker delta, $\delta_{ij} = \begin{cases} 1 & \text{if } i=j \\ 0 & \text{if } i \neq j\end{cases}$
