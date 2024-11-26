---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-a-coulomb-s-law/px-157-a3-principle-of-super-position/","created":"2024-10-01T18:50:56.350+01:00","updated":"2024-11-26T20:07:05.965+00:00"}
---

- total force, $\vec F_{0}$, on charge, $q_{0}$ :
$$
\vec F_{0} = \sum\limits_{i=1}^{N} \vec F_{i0} = \frac{q_{0}}{4\pi\epsilon_{0}} \sum\limits_{i=0}^{N} q_{i} \frac{\vec r_{0} - \vec r_{i}}{|\vec r_{0} - \vec r_{i}|^{3}}
$$
- eg: ![Pasted image 20240110093525.png](/img/user/pics/Pasted%20image%2020240110093525.png)
	$q_{1}=q_{2}=q$
	$\vec r_{1}= d \hat y$ and $\vec r_{2} = -d \hat y$
	$\vec r_{Q}= x \hat x$
	$$\begin{align}

    \vec F_{Q} &= \frac{Q q_{1}}{4\pi\epsilon_{0}} \frac{\vec r_{Q} - \vec r_{1}}{|\vec r_{Q} - \vec r_{1}|^{3}} + \frac{Q q_{2}}{4\pi\epsilon_{0}} \frac{\vec r_{Q} - \vec r_{2}}{|\vec r_{Q} - \vec r_{2}|^{3}} \\
    
	&= \frac{Q q_{1}}{4\pi\epsilon_{0}} \left\{ \frac{x\hat x -d\hat y}{(x^{2}+d^{2})^{\frac{3}{2}}} + \frac{x\hat x +d\hat y}{(x^{2}+d^{2})^{\frac{3}{2}}}\right\} \\
	
	\therefore \vec F_{Q} &= \frac{Q q_{1}}{4\pi\epsilon_{0}} \frac{2x\hat x}{(x^{2}+d^{2})^{\frac{3}{2}}} 
	\end{align}$$
 