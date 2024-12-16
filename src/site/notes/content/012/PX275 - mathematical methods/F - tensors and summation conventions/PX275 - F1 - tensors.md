---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/f-tensors-and-summation-conventions/px-275-f1-tensors/","noteIcon":"1","created":"2024-12-02T12:09:35.780+00:00","updated":"2024-12-02T18:52:07.064+00:00"}
---

- considering the angular momentum of a simple system:
$$\vec L = I \vec \omega$$
	where, $I$ is the moment of inertia, and	$\vec \omega$ is the angular velocity
- considering two masses, $m_1$ and $m_2$, on the end of a stiff rod with negligible mass, attached to a string, and making an angle, $\theta$, to the horizontal
![Pasted image 20241202184427.png|500](/img/user/pics/Pasted%20image%2020241202184427.png)
- the angular momentum of masses in general:
$$\vec L = \vec r \times \vec p = m(\vec r \times \vec v)$$
- the total angular momentum:
$$\vec L = \vec L_{1} + \vec L_{2}$$
- for the system of two masses:
$$\vec L = \sum\limits_{i=1}^{2} \vec r_{i}\times \vec p_{i} = \sum\limits_{i=1}^{2} m_{i}(\vec r_{i}\times \vec v_i)$$ $$\vec  L = \sum_{i=1}^{2} m_{i}(\vec r_{i} \times (\vec \omega_{i} \times \vec r_{i}))$$
- for one mass:
	$\vec r = x\hat i + y \hat j + z\hat k$
	$\vec \omega  = \omega_{x} \hat i + \omega_{y}\hat j + \omega_{z}\hat k$
$$\begin{align*}
	\vec{\omega} \times \vec{r} &= \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ \omega_x & \omega_y & \omega_z \\ x & y & z \end{vmatrix} \\
	 & = (\omega_y z - \omega_z y) \hat{i}
	 + (\omega_z x - \omega_x z) \hat{j} 
	 + (\omega_x y - \omega_y x) \hat{k}
\end{align*}$$
- hence, the angular momentum:
$$\begin{multlined}  \vec{r} \times (\vec{\omega} \times \vec{r}) = \\\big(\boxed{(y^2 + z^2)\omega_x} - (xy)\omega_y - (xz)\omega_z \big) \hat{i} \\+ \big((-xy)\omega_x + \boxed{(x^2 + z^2)\omega_y} - (yz)\omega_z \big) \hat{j} \\+ \big((-xz)\omega_x - (yz)\omega_y + \boxed{(x^2 + y^2)\omega_z} \big) \hat{k}\end{multlined}$$
- the boxed terms represent the **principal moments of inertia**
- the components of the angular momentum vector can be written as:
$$\begin{align*}
L_{x} = \omega_{x} I_{xx} + \omega_{y}I_{xy} + \omega_{z}I_{xz} \\
L_{y} = \omega_{x} I_{yx} + \omega_{y} I_{yy} + \omega_{z} I_{yz} \\
L_{z} = \omega_{x} I_{zx} + \omega_{y} I_{zy} + \omega_{z} I_{zz}
\end{align*} $$
- in matrix notation:
$$\begin{bmatrix} L_x \\ L_y \\ L_z \end{bmatrix} = \begin{bmatrix} I_{xx} & I_{xy} & I_{xz} \\ I_{yx} & I_{yy} & I_{yz} \\ I_{zx} & I_{zy} & I_{zz} \end{bmatrix} \begin{bmatrix} \omega_x \\ \omega_y \\ \omega_z \end{bmatrix}$$
- this can be written more concisely as:
$$L_{j} = \sum\limits_{i=1,2,3} I_{ij} \,\vec\omega_{j}$$
	where, $L_1 = L_x$, and so on
$$L_{1}= (I_{11} + I_{21}+ I_{31}) \omega_{x} = I_{ij}\omega_x$$
- $I$ is the moment of inertia tensor, a $2^{nd}$ rank/order tensor with $9$ components
