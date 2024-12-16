---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/g-measurement-of-angular-momentum/px-262-g6d-weak-field-zeeman-effect/","noteIcon":"1","created":"2024-11-26T11:41:04.286+00:00","updated":"2024-11-26T12:18:56.448+00:00"}
---

- investigating the regime where both the effects are important
- in calculations, ${} (\hat {\vec L} + 2\hat{\vec S})$ and $(\hat{\vec L} + \hat{\vec S})$ are needed, which do not align
- semi-classically, for the interaction energy:
$$\delta E = B \mu_{jz}$$
	where, $\mu_{jz}$ is the $z$-component of the total magnetic moment, $\vec \mu_{j}$
$$\begin{align*}
\vec\mu_{j} &= \vec j \cdot \frac{\vec\mu}{j} \\
&= \frac{e}{2mj} \vec j \cdot (\vec l + 2\vec s) \\
&= \frac{e}{2mj} (j^{2}+ \vec j \cdot \vec s) \\
&= \frac{ej}{2m}\left(1+ \frac{\vec l\cdot\vec s + s^{2}}{j^{2}}\right) \\
&= \frac{ej}{2m}(1 + \frac{j^{2}-l^{2}-s^{2}}{2j^{2}})
\end{align*}$$
- the energy:
$$\delta E = \frac{eB}{2m} j_{z} (1 + \frac{j^{2}-l^{2}-s^{2}}{2j^{2}})$$
- using the same functional form in quantum mechanics:
$$\delta E = g \mu_{B}m_{j}B$$
	where, 
		$\mu_{B} = \frac{e\hbar}{2m}$ is the **bohr magneton**
		$m_{j}$ is the $z$-component of the total angular momentum
		$g = 1 + \frac{j(j+1)-l(l+1)-s(s+1)}{2j(j+1)}$ is the landé g-factor
- in such situations, the orbital quantum number is not a good quantum number, bit states are the eigenstates of total angular momentum operator
- the existence of LS coupling removes degeneracy of the energy levels
