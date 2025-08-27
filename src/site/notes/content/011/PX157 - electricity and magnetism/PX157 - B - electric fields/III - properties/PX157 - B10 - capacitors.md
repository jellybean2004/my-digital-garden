---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/iii-properties/px-157-b10-capacitors/","noteIcon":"1","created":"2025-08-27T13:14:04.803+01:00","updated":"2024-11-26T20:08:43.000+00:00"}
---

## capacitance
![Pasted image 20240131101020.png](/img/user/pics/Pasted%20image%2020240131101020.png)
$$
C = \frac{Q}{V}
$$
- units: $C\,V^{-1}$ or $farad\,(F)$
## parallel plate capacitor
- electric field:
$$
\vec E = \vec E_{top} + \vec E_{bottom} = - \frac{\sigma}{\epsilon_{0}}\hat{z}
$$
		where, $\sigma= \frac{Q}{A}$ : surface charge density
- potential difference between the plates:
$$
V = E\, d = \frac{\sigma}{\epsilon_{0}}d = \frac{Qd}{\epsilon_{0}A}
$$
- for parallel plates:
$$
C = \frac{Q}{V} = \frac{\epsilon_{0}A}{d}
$$
## cylindrical capacitor
![Pasted image 20240131101036.png](/img/user/pics/Pasted%20image%2020240131101036.png)
$$\begin{align*}
	V_{ab} &= \frac{\lambda}{2\pi\epsilon_{0}} \ln\left(\frac{R_{b}}{R_{a}}\right) \\
	&= \frac{Q}{2\pi\epsilon_{0}L} \ln\left(\frac{R_{b}}{R_{a}}\right) \\
\end{align*}$$
$$
\therefore C = \frac{2\pi\epsilon_{0}L}{\ln(\frac{R_{b}}{R_{a}})}
$$
## spherical capacitor
![Pasted image 20240131101054.png](/img/user/pics/Pasted%20image%2020240131101054.png)
$$
q = \sigma_{a}4\pi r_{a}^{2} = -\sigma_{b}4\pi r_{b}^{2}
$$
$$
V_{ab} = \frac{q}{4\pi\epsilon_{0}} \left(\frac{1}{r_{a}}- \frac{1}{r_{b}}\right)
$$
$$
C = \frac{4\pi\epsilon_{0}}{(\frac{1}{r_{a}}- \frac{1}{r_{b}})}
$$
- single-plate spherical capacitor: **van der graaf generator**
## capacitors in series
![Pasted image 20240131101121.png](/img/user/pics/Pasted%20image%2020240131101121.png)
- conservation of charge: both capacitors have the same charge, $Q:$
$$
V_{1}= \frac{Q}{C_{1}}\;,\;V_{2}=\frac{Q}{C_{2}}
$$
$$
\implies V = V_{1} + V_{2} = Q \left(\frac{1}{C_{1}} + \frac{1}{C_{2}}\right)
$$
- this is equivalent to a circuit with one capacitor, $C_{eq}$:
$$
\frac{1}{C_{eq}} = \frac{1}{C_{1}}+ \frac{1}{C_{2}}
$$
- assume both the capacitors have the same $A$ and $\epsilon_{0}:$
$$\frac{1}{C_{eq}} = \frac{d_{1}}{\epsilon_{0}A} + \frac{d_{2}}{\epsilon_{0}A} = \frac{d_{1}+d_{2}}{\epsilon_{0}A}
$$
## capacitors in parallel
![Pasted image 20240131101149.png](/img/user/pics/Pasted%20image%2020240131101149.png) 
- both capacitors have the same potential drop
$$
Q_{1} =C_{1}V \; ,\; Q_{2}=C_{2}V
$$
- total charge: $Q = Q_{1}+Q_{2} = (C_{1}+C_{2})V$
- equivalent capacitor, $C_{eq}:$
$$
C_{eq} = C_{1}+C_{2}
$$

\1\n\2\n