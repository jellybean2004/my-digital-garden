---
dg-publish: true
---
## introduction
- the work done by a force, $\vec F$, moving a vector distance, $d\vec l$
$$
E = K + U
$$
- in a conservative system:
$$\begin{align*}
\Delta E &= 0 \\
\Delta K &= -\Delta U \\
W_{a\to b} &= -\Delta U
\end{align*}$$
- from the definition of work:
$$
W = \vec F\cdot d\vec l = F\,dl\cos\theta
$$
- for work along a non-straight path:
	![Pasted image 20240125101458.png](/img/user/pics/Pasted%20image%2020240125101458.png)
	$$\begin{align*}
		dW &= \vec F \cdot d\vec l \\
		W_{a\to b} &= \int_{a}^{b} \vec F \cdot d\vec l
	\end{align*}$$
## [[content/011/PX153 - mathematics for physicists/term 2/PX153 - I - integration/PX153 - I9 - line integrals\|line integrals]]
### closed path
$$
W = \oint \vec F \cdot d\vec l
$$
### path is in the x-direction
$$\begin{align*}
	\vec r &= x\,\hat x \\
	d\vec l &= d\vec r = dx\, \hat x \\\\
	\int_{a}^{b} \vec F \cdot d\vec l &= \int_{x_{a}}^{x_{b}} \vec F \cdot \hat x\,dx \\
	&= \int_{x_{a}}^{x_{b}} F_{x}\,dx
\end{align*}$$

### path is in the radial direction
$$\begin{align*}
	\vec r &= r\,\hat r \\\\
	d\vec l &= d\vec r \\
	&= dr\,\hat r
\end{align*}$$

### path is in the azimuthal direction
- ie: path is a circle in the $x-y$ plane with a radius, $a$
	$\vec r = a\,\hat R(\phi)$
	$d\vec l = d\vec r = a \frac{d\hat{R}}{d\phi} d\phi$
	$\hat R = \cos\phi\,\hat x + \sin\phi\,\hat y$
	$\frac{d\hat{R}}{d\phi} = -\sin\phi\,\hat x + \cos\phi\,\hat y \equiv \hat\phi$
	$d\vec l = a\,\hat\phi\,d\phi$
$$
W_{a\to b} = \int_{a}^{b} \vec F\cdot d\vec l = U_{a}- U_{b}
$$
