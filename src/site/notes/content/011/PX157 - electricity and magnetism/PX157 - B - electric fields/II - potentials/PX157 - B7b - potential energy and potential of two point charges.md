---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/ii-potentials/px-157-b7b-potential-energy-and-potential-of-two-point-charges/","created":"2024-10-01T18:27:10.091+01:00","updated":"2024-11-26T20:08:24.650+00:00"}
---

![Pasted image 20240123181201.png](/img/user/pics/Pasted%20image%2020240123181201.png)
$$
F_{12} = \frac{q_{1}q_{2}}{4\pi\epsilon_{0}} \frac{\hat{r}}{r^{2}}
$$
- the path is described by position: $\vec r = r\,\hat r \implies d\vec l = d\vec r = dr\,\hat r$
$$\begin{align*}
	W_{a\to b} &= \int_{r_{a}}^{r_{b}} \frac{q_{1}q_{2}}{4\pi\epsilon_{0}} \frac{\hat{r}}{r^{2}} \cdot \hat r\,dr \\
	&= \frac{q_{1}q_{2}}{4\pi\epsilon_{0}} \int_{r_{a}}^{r_{b}} \frac{1}{r^{2}}\, dr \\
	&= \frac{q_{1}q_{2}}{4\pi\epsilon_{0}}\left(\frac{1}{r_{a}}- \frac{1}{r_{b}}\right) \\
	W_{a\to b} &= U_{a} - U_{b} \\
	\implies U_{a} &= \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r_{a}}
\end{align*}$$
- defining that potential energy tends to zero as $r\to\infty: \lim_{r_{b}\to\infty} U_{12}(b)=0$:
$$
\implies U_{12}= \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r}
$$
- **note:** $U_{12}= U_{21}$, because $\vec F_{12}=-\vec F_{21}$, and $d\vec l_{12}= -d\vec l_{21}$

- if there are $N$ charges interacting with a charge, $q_{0}$, total potential energy:
$$
U_{0} = \sum\limits_{i=1}^{N} U_{i0} = \sum\limits_{i=0}^{N} \frac{q_{i}q_{0}}{4\pi\epsilon_{0}|\vec r_{0}-\vec r_{i}|}
$$
