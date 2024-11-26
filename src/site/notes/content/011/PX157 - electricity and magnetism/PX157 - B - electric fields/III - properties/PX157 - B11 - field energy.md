---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/iii-properties/px-157-b11-field-energy/","created":"2024-10-01T18:27:10.117+01:00","updated":"2024-11-26T20:08:46.049+00:00"}
---

## total potential energy
![Pasted image 20240131100955.png](/img/user/pics/Pasted%20image%2020240131100955.png)
$$
U_{12}= \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r}
$$
- the potential at $q_{1}$ due to $q_{2}: V_{1}(r)= \frac{q_{2}}{4\pi\epsilon_{0}e}$
- the potential at $q_{2}$ due to $q_{1}: V_{2}(r)= \frac{q_{1}}{4\pi\epsilon_{0}e}$
$$\begin{align*}
	\implies U_{12} &= \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r} \\
	&= \frac{1}{2}\frac{q_{1}q_{2}}{4\pi\epsilon_{0}r} + \frac{1}{2}\frac{q_{1}q_{2}}{4\pi\epsilon_{0}r} \\
	&= \frac{1}{2} q_{1}V_{1} + \frac{1}{2}q_{2}V_{2}
\end{align*}$$
- also true for $n$ charges:
$$\begin{align*}
		U &= \sum\limits_{i=1}^{n} \frac{1}{2}q_{i}V_{i}\\
		V_{i} &= \sum\limits_{j=1, j\neq i}^{n} \frac{U_{ij}}{q_{i}}
	\end{align*}$$
- eg: potential energy of pour point charges
	![Pasted image 20240131100933.png](/img/user/pics/Pasted%20image%2020240131100933.png)
	$$U = U_{12} + U_{13}+ U_{14} + U_{23}+ U_{24} + U_{34}$$
	- since $U_{ij}= u_{ji}:$
$$
U = \frac{1}{2}(U_{12} + U_{13}+ U_{14} +U_{21}+ U_{23}+ U_{24}+ U_{31}+ U_{32} + U_{34} + U_{41} + U_{42} + U_{43})
$$
## energy stored in a capacitor
![Pasted image 20240207103547.png](/img/user/pics/Pasted%20image%2020240207103547.png)
$$
U = \frac{1}{2}(+Q)V_{+} + \frac{1}{2}(-Q)V_{-} = \frac{1}{2}Q(V_{+}-V_{-})
$$
$$
U = \frac{1}{2}QV = \frac{1}{2}CV^{2} = \frac{1}{2}\frac{Q^{2}}{C}
$$
- **recap**: in a spring:
$$
U= \frac{1}{2}kx^{2}
$$
## energy density of the electric field
- energy density:
$$
u = \frac{U}{V}
$$
- for parallel plate capacitor:
$$
u = \frac{\frac{1}{2}CV^{2}}{Ad}
$$
- also, $C=\frac{\epsilon_{0}A}{d}$, $V=Ed:$
$$
u = \frac{1}{2}\epsilon_{0}E^{2}
$$
- also, $U = mc^{2}$, $U = \frac{1}{2}\epsilon_{0}E^{2}V$ 

- eg: a capacitor is connected to a fully charged battery with potential, $V$, that carries charge, $Q$. it is then disconnected. the separation between the plates is doubled ($d\to2d$). what happens to the associated quantities?
![Pasted image 20240207103703.png](/img/user/pics/Pasted%20image%2020240207103703.png)

|                    before                    |                                     after                                     |
|:--------------------------------------------:|:-----------------------------------------------------------------------------:|
|     
$$
C_{0}= \frac{\epsilon_{0}A}{d}
$$
$$
C_{new}= \frac{\epsilon_{0}A}{2d} = \frac{1}{2}C_{0}
$$
|
$$
U_{0} = \frac{1}{2} \frac{Q^{2}}{C_{0}}
$$
$$
U_{new}= \frac{1}{2} \frac{Q^{2}}{C_{new}} = \frac{Q^{2}}{C_{0}} = 2U_{0}
$$
|                
$$
V_{0}=V
$$
$$
V_{new} = \frac{U_{new}}{Q} = 2V_{0}
$$
|        
$$
E_{0} = \frac{V_{0}}{d}
$$
$$
E_{new} = \frac{V_{new}}{2d} = \frac{2V}{2d} = E_{0}
$$
|
$$
u_{0} = \frac{1}{2}\epsilon_{0}E_{0}^{2}
$$
$$
u_{new} = \frac{1}{2}\epsilon_{0} E_{new}^{2} = u_{0}
$$
|            
$$
Volume_{0} = Ad
$$
$$
Volume_{new}=2Ad = 2\,Volume_{0}
$$
