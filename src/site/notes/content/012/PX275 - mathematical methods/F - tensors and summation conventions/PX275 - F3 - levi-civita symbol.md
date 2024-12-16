---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/f-tensors-and-summation-conventions/px-275-f3-levi-civita-symbol/","noteIcon":"1","created":"2024-12-02T12:51:24.952+00:00","updated":"2024-12-02T19:14:05.252+00:00"}
---

- the levi-civita symbol is a tool to write things more concisely in tensor analysis

- in 2D:
$$\varepsilon_{ij} = \begin{cases}
+1 & \text{if } (i,j) = (1,2) \\
-1 & \text{if } (i,j) = (2,1) \\
0 & \text{if } i = j
\end{cases}$$
- arranging this into a $2\times2$ matrix:
$$\varepsilon = \begin{pmatrix}0 & 1 \\ -1 & 0\end{pmatrix}$$

- in 3D:
$$\varepsilon_{ij} = \begin{cases}
+1 & \text{if } (i,j,k) = (1,2,3)\;\text{or } (2,3,1)\;\text{or } (3,1,2) \\
-1 & \text{if } (i,j,k) = (3,2,1)\;\text{or } (1,3,2)\;\text{or } (2,1,3) \\
0 & \text{if } i = j\;\text{or } j=k \;\text{or }  k=i
\end{cases}$$
![Pasted image 20241202190256.png|500](/img/user/pics/Pasted%20image%2020241202190256.png)
## example
- considering a vector cross product:
$$\begin{align*}
\vec{a} \times \vec{b} &= 
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
a_x & a_y & a_z \\
b_x & b_y & b_z
\end{vmatrix} 
= \begin{vmatrix}
x_1 & x_2 & x_3 \\
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3
\end{vmatrix} \\
&= x_1 (a_2 b_3 - b_2 a_3) + x_2 (a_3 b_1 - b_3 a_1) + x_3 (a_1 b_2 - b_1 a_2)
\\
&= \sum_{i=1}^{3} \sum_{j=1}^{3} \sum_{k=1}^{3} \varepsilon_{ijk} \, x_i \, a_j \, b_k
\end{align*}$$