---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/d-equipartition-theorem/px-284-d2-applications-of-the-equipartition-theorem/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-23T21:54:30.838+00:00"}
---

## translational motion of a monatomic gas
- considering a helium atom with three degrees of freedom: 
$$E = \frac{1}{2}m v_{x}^{2} + \frac{1}{2}m v_{y}^{2} + \frac{1}{2}m v_{z}^{2}$$
$$\therefore \langle{E}\rangle = \frac{3}{2}k_{B}T$$
- $C_{V} = \frac{3}{2}k_{B}$ per atom or $\frac{3}{2}N_{A}k_{B}$ per mole, where $N_{A}$ is avogrado's constant
## mass on a spring
$$\begin{gather*}
	E = \frac{1}{2}kx^{2} + \frac{1}{2}m\dot x^{2} \\\\
	\therefore \langle{E}\rangle = k_{B}T
\end{gather*}$$
## two masses connected by a spring
$$\begin{gather*}
	E = \frac{1}{2}k(|\vec r_{1} - \vec r_{2}|^{2})+ \frac{1}{2}\mu (\dot {\vec r}_{1}- \dot{\vec r}_{2})^{2} + \frac{1}{2}(m_{1}+ m_{2})\dot{\vec r}_{COM}^{2} \\\\
	\therefore \langle{E}\rangle = \frac{3}{2}k_{B}T
\end{gather*}$$
where, $\mu = \frac{m_{1}m_{2}}{m_{1}+m_{2}}$
## lattice vibrations
- a 3D arrangement of masses and springs
- for a cubic lattice, there are 3 springs per ion: 
$$\langle{E}\rangle = 3 k_{B}T$$
- $C_{V} = 3k_{B}$ per atom or $2N_{A}k_{B}$ per mole
## diatomic molecules
[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C9 - heat capacity of the ideal gas\|PX154 - C9 - heat capacity of the ideal gas]]
- translational motion: 
$$ \begin{gather}
E = \frac{1}{2}m v_{x}^{2} + \frac{1}{2}m v_{y}^{2} + \frac{1}{2}m v_{z}^{2} \\ 
\implies\langle{E_{trans}}\rangle = \frac{3}{2}k_{B}T
\end{gather}$$
- vibrational motion: 
$$\langle{E_{vib}}\rangle \approx k_{B}T$$
- rotational motion: 
$$\begin{gather*}
	E_{rot} = \frac{1}{2} \frac{L_{1}^{2}}{I_{1}} + \frac{1}{2} \frac{L_{2}^{2}}{I_{2}} \\ 
	\langle{E_{rot}}\rangle = k_{B}T
\end{gather*}$$
	where, $L$ is the angular momentum, $I$ is the moment of inertia, and $1$ and $2$ represent rotation along the $z$ and the $y$-axes respectively for a molecule along the $x$-axis

- the average energy of the molecule: 
$$\langle{E}\rangle = \langle{E_{trans}}\rangle + \langle{E_{vib}}\rangle + \langle{E_{rot}}\rangle = \frac{3}{2}k_{B}T + k_{B}T + k_{B}T = \frac{7}{2}k_{B}T$$
- $C_{V} = \frac{7}{2}k_{B}$ per molecule or $\frac{7}{2}N_{A}k_{B}$ per mole
