---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/g-additional-interactions/px-262-g7c-weak-field-zeeman-effect/","noteIcon":"1","created":"2025-08-27T13:14:26.308+01:00","updated":"2024-12-21T15:15:17.000+00:00"}
---

- investigating the regime where both spin-orbit coupling and zeeman effect are important
$$\hat H '  = \underbrace{f(r) (\hat J^{2} - \hat L^{2} - \hat S^{2})}_\text{LS coupling} +\underbrace{\frac{e}{2m}B_{0} (\hat L_{z} + 2 \hat S_{z})}_\text{zeeman effect} $$
- in calculations, ${} (\hat {\vec L} + 2\hat{\vec S})$ and $(\hat{\vec L} + \hat{\vec S})$ are needed, which do not align
- semi-classically, for the interaction energy:
$$\delta E = B \mu_{jz}$$
	where, $\mu_{jz}$ is the $z$-component of the total magnetic moment, $\vec \mu_{j}$
$$\begin{gather}
\vec j = \vec l + \vec s \tag{i} \\
\vec j \cdot \vec s = \frac{1}{2}(j^{2}- l^{2}-s^{2}) \tag{ii}
\end{gather}$$
$$\begin{align*}
\vec\mu_{j} &= \frac{\vec j}{j} \cdot \vec\mu \\
&= \frac{e}{2mj} \vec j \cdot (\vec l + 2\vec s) \\
&= \frac{e}{2mj} (j^{2}+ \vec j \cdot \vec s)  \; \big[\because (i) \big]\\
&= \frac{ej}{2m}\left(1+ \frac{\vec l\cdot\vec s + s^{2}}{j^{2}}\right) \\
&= \frac{ej}{2m}\left(1 + \frac{j^{2}-l^{2}-s^{2}}{2j^{2}}\right) \big[ \because (ii) \big]
\end{align*}$$

- therefore, the interaction energy:
$$\delta E = \frac{eBj_{z}}{2m} \left(1 + \frac{j^{2}-l^{2}-s^{2}}{2j^{2}}\right)$$
- replacing the classical expressions for the magnitudes of the angular momenta by the eigenvalues of the correponding operators:
$$\delta E = g \mu_{B}m_{j}B$$
	where, 
		$\mu_{B} = \frac{e\hbar}{2m}$ is the **bohr magneton**
		$m_{j}$ is the $z$-component of the total angular momentum
		$g = 1 + \frac{j(j+1)-l(l+1)+s(s+1)}{2j(j+1)}$ is known as the **landé g-factor**
	
- if $s=0$, $j=l$, $g=1$, which corresponds to all the angular momentum being orbital
- conversely, if $l=0$, $j=s$, $g=2$, which corresponds to no orbital angular momentum
