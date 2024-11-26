---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/i-field/px-157-b3-electrical-dipoles/","created":"2024-10-01T18:27:10.060+01:00","updated":"2024-11-26T20:07:16.710+00:00"}
---

![Pasted image 20240115132703.png](/img/user/pics/Pasted%20image%2020240115132703.png)
- a pair of charges, $+q$ and $-q$, separated by a fixed distance, $d$
- the electrical dipole moment is:
$$
\vec p = q \vec d
$$
- in an external electric field, $\vec E$, force on the dipole is:
$$
\vec F = +q\vec E + (-q)\vec E = 0
$$
![Pasted image 20240115132729.png](/img/user/pics/Pasted%20image%2020240115132729.png)
- total force is zero, but there is a *torque*
	angular momentum: $\vec L = \vec r \times m\vec v$
	angular force (torque): $\vec\tau = \vec r \times \vec F$
![Pasted image 20240115132825.png](/img/user/pics/Pasted%20image%2020240115132825.png)
- here:
$$\begin{align*}
	\vec\tau &= \vec r \times (+q)\vec E + (-\vec r) \times (-q)\vec E \\
	&= 2q\,\vec r \times \vec E \\
	&= q \, \vec d \times E \\
	\therefore \vec \tau &= \vec p \times \vec E\\
	or, |\vec \tau| &= q \, d \, E \, \sin\phi
\end{align*}$$
- for linear motion: $W = \vec F \cdot \vec d$
- for rotation: $dW = \tau \, d\phi = -pE\sin{\phi} \, d\phi$
- rotate from $\phi_{1} \to \phi_{2}$:
$$\begin{align*}
	W &= - \int\limits_{\phi_{1}}^{\phi_{2}} pE \sin\phi .d\phi \\
	&= +pE(\cos{\phi_{2}} - \cos{\phi_{1}}) \\\\
	&= -\Delta(-pE\cos\phi)
\end{align*}$$
- $\Delta E = \Delta K + \Delta U = 0 \implies W = -\Delta U$
- define potential energy:
$$\begin{align*}
	U(\phi) &= -p \, E \, \cos\phi \\
	U(\phi) &= -\vec p \cdot \vec E
	\end{align*}$$
![Pasted image 20240115132908.png](/img/user/pics/Pasted%20image%2020240115132908.png)