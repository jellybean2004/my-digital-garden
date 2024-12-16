---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-e-ac-circuits/px-157-e3-kirchhoff-s-laws-for-ac-circuits/","noteIcon":"1","created":"2024-10-01T18:27:10.275+01:00","updated":"2024-11-26T20:11:17.495+00:00"}
---

[[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/IV - circuits/PX157 - B14a - circuits - kirchhoff's rules\|kirchhoff's rules]] are valid if:
	- the size of the circuit is much smaller than the wavelength of the source
	- the transit time of the electromagnetic radiation is much less than the period of the AC source
	- **note**: for $50\,Hz$ AC supply: $\lambda f = c \implies \lambda = 6\times10^{6}\,m$

- impedance in series:
$$
\tilde Z_{eq} = \tilde Z_{1}+ \tilde Z_{2}
$$
- impedance in parallel:
$$
\frac{1}{\tilde Z_{eq}} = \frac{1}{\tilde Z_{1}} + \frac{1}{\tilde Z_{2}}
$$
- eg: 
![Pasted image 20240311182400.png](/img/user/pics/Pasted%20image%2020240311182400.png)
- all elements are in series:
$$\begin{align*}
			\tilde Z_{eq} &= \tilde Z_{R} + \tilde Z_{C} + \tilde Z_{L} \\
			&= R + \frac{1}{j\omega C} + j\omega L \\
			&= R + j(\omega L - \frac{1}{\omega C})
		\end{align*}$$

- eg:
![Pasted image 20240311182427.png](/img/user/pics/Pasted%20image%2020240311182427.png)
$$\begin{align*}
	\tilde Z_{eq} &= \tilde Z_{R} + \left(\frac{1}{\tilde Z_{C}} + \frac{1}{\tilde Z_{L}}\right)^{-1} \\
	&= R + \left(j\omega C + \frac{1}{j\omega L}\right)^{-1} \\
	&= R + \left(j\left(\omega C - \frac{1}{\omega L}\right) \right)^{-1} \\
	&= R + \frac{j}{\left(\frac{1}{\omega L}-\omega C\right)}
\end{align*}$$
