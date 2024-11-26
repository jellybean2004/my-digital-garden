---
dg-publish: true
---

- to determine the electric field outside a charged hollow sphere
![Pasted image 20241125124204.png](/img/user/pics/Pasted%20image%2020241125124204.png)
- using the divergence theorem:
$$\iint_{S} \vec F \cdot d\vec s = \iiint_{V}(\vec\nabla \cdot \vec E)\,dV$$
- defining:
$$\vec\nabla\cdot\vec E = \frac{\sigma}{\varepsilon_{0}} \delta(\vec r- \vec a)$$
- **remember:** $\delta(\vec r- \vec a) = 0$ for $r\neq a$
$$\iint_{S}\vec E \cdot d\vec s = \iiint_{V} \frac{\sigma}{\varepsilon_{0}} \delta(\vec r- \vec a) \,dV$$
$$\iiint \delta(\vec r - \vec a)\,dV = 1 \;\text{at} \;\vec r = \vec a$$
$$\begin{align*}
	\iint_{S}\vec E \cdot d\vec s &= 4\pi r^{2} E = \iiint_{V} \frac{\sigma}{\varepsilon_{0}} (\delta(\vec r - \vec a))\,dV \\
	&= \frac{\sigma}{\varepsilon_{0}}4\pi a^{2} \\
	\therefore E&= \frac{\sigma}{\varepsilon_{0}} \frac{a^{2}}{r^{2}}
\end{align*}$$

