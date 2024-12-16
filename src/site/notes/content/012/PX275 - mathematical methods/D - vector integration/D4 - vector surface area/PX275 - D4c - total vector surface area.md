---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/d-vector-integration/d4-vector-surface-area/px-275-d4c-total-vector-surface-area/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-27T23:01:50.626+00:00"}
---

- to evaluate the **vector area**: 
$$\vec S = \iint d\vec s$$
![Pasted image 20241118124714.png](/img/user/pics/Pasted%20image%2020241118124714.png)
### the total vector surface area of the flat disc
$$\vec S_{1} = \iint d\vec s = \iint \hat n\,dA$$
$$d\vec s = dA\,\hat k = \rho\,d\phi\,d\rho\,\hat k$$
$$\begin{align*}
	\vec S_{1} &= \int_{\rho=0}^{a}\int_{\phi=0}^{2\pi} \rho\,d\phi\,d\rho\,\hat k \\
	&= \left[2\pi \frac{\rho^{2}}{2} \hat k\right]_{0}^{a} \\
	\vec S_{1} &= \pi a^{2}\hat k
\end{align*}$$
### the total vector surface area of the dome of the hemisphere
 $$\vec S_{2} = \iint d\vec s = \iint \hat n\,dA$$
- considering the $\hat i, \hat j, \hat k$ components individually for the hemisphere
#### the $\hat k$-component
$$\begin{align*}
	\vec S_{2(k)} &= \iint r^{2} \sin\theta \, d\theta\, d\phi \cos\theta \, \hat k \\
	&= \int_{0}^{\frac{\pi}{2}} \int_{0}^{2\pi} a^{2} \sin\theta \cos\theta\, d\phi \, d\theta \, \hat k \\
	&= 2\pi a^{2}\, \hat k \int_{0}^{\frac{\pi}{2}} \sin\theta\cos\theta\, d\theta \\
	&= 2\pi a^{2} \left[\frac{\sin^{2}\theta}{2}\right]_{0}^{\frac{\pi}{2}}\, \hat k \\
	&= \pi a^{2} \, \hat k 
\end{align*}$$
#### the $\hat i$-component
- the $\hat i$-component of ${} \hat e_{r}$ is $\sin\theta\cos\phi$
$$\begin{align*}
	\vec S_{2(i)} &= \iint dA \sin\theta\cos\phi \, \hat i \\
	&= \int_{0}^{\frac{\pi}{2}}\int_{0}^{2\pi} r^{2}\sin\theta\, d\theta\, d\phi \sin\theta\cos\phi\, \hat i \\
	&= \int_{0}^{\frac{\pi}{2}} a^{2}\sin^{2}\theta\, d\theta \int_{0}^{2\pi}\cos\phi\, d\phi \, \hat i \\
	
	&= 0
\end{align*}$$
#### the $\hat j$-component
- it can be deduced from symmetry that $S_{2(i)}, S_{2(j)} =0$
$$\begin{align*}
	\vec S_{2(j)} &= \iint r^{2}\sin\theta\,d\theta\,d\phi  \sin\theta\sin\phi\,\hat j \\
	&= \int_{0}^{\frac{\pi}{2}}a^{2}\sin^{2}\theta\,d\theta \int_{0}^{2\pi}\sin\phi\,d\phi \, \hat j\\
	&= 0
\end{align*}$$
- hence, the total vector surface area of the hemisphere is: 
$$\vec S_{2} = \pi a^{2}\,\hat k$$
