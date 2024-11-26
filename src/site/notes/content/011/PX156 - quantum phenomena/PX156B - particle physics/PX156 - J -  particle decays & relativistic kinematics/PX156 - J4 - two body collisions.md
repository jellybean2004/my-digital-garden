---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-b-particle-physics/px-156-j-particle-decays-and-relativistic-kinematics/px-156-j4-two-body-collisions/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T20:06:05.113+00:00"}
---

- three common reference frames:
	- centre of momentum (COM) frame 
		- $COM:\vec p_{1}= - \vec p_{2}$
	- fixed target frame
	- lab frame
## mandelstam-s
- if there are a set of particles, $i$, in the initial or final state of a collision interaction, then $s$ is invariant: 
$$s = \left(\sum\limits_{i}E_{i} \right)^{2}- \left|\sum\limits \vec p_{i}c\right|^{2}$$ 
- $s$ is conserved in the initial and final state
- $s$ is invariant and does not depend on reference frame
## interpretation of $s$
- consider a collision in the lab frame
$$\begin{align*}
	s &= (E_{1}+ E_{2})^{2}- |\vec p_{1}c + \vec p_{2}c|^{2} \\
	&= (E_{1}^{2} + E_{2}^{2} + 2E_{1}E_{2}) - (| p_{1}|^{2}c^{2} + |p_{2}|^{2}c^{2} + 2c^{2} \vec p_{1}\cdot \vec p_{2})\\
	&= m_{1}^{2}c^{4} + m_{2}^{2}c^{4} + 2E_{1}E_{2} - 2c^{2}\vec p_{1}\cdot \vec p_{2} \\
	&= m_{1}^{2}c^{4} + m_{2}^{2}c^{4} + 2E_{1}E_{2} - 2c^{2}|p_{1}||p_{2}|\cos(\pi-\theta)
\end{align*}$$
- massless limit: $E_{i}>>m_{i}c^{2}:$ 
$$s \simeq 2E_{1}E_{2} -2E_{1}E_{2}\cos(\pi-\theta)$$
- in $COM$ frame: $\theta=0:$ 
$$s = 4 E_{1}E_{2}$$
- in the massless limit: $E_{1}=E_{2}=E$ in $COM$ frame: 
$$\begin{align*}
	\therefore s &= 4E^{2} \\
	\sqrt{s} &= 2E
\end{align*}$$
- this is the total energy available to make new particles in the final state

- $\sqrt{s_{COM}}\equiv$ '$COM$ energy'
- this tells if the final state can be made in $COM$ frame
- figure of merit for designing accelerators

- why build a collider?
	- $\sqrt{s_{COM}}\simeq 2E$
	- for a fixed target: 
$$\begin{align*}
	s &= (E_{1}+ m_{2}c^{2})- |\vec p_{1}c|^{2} \\
	&= E_{1}^{2}+ 2 E_1m_{2}c^{2}+ m_{2}^{2}c^{4}- |\vec p_{1}c|^{2} \\
	&= m_{1}^{2}c^{4} + 2E_{1}m_{2}c^{2}+ m_{2}c^{4}
\end{align*}$$
	- massless limit: $s\simeq 2E_{1}m_{2}c^{2}$
	- or, $\sqrt{s_{FT}}= \sqrt{2E_{1}m_{2}c^{2}}$

- collider: $\sqrt{s_{COM}}\propto E$
- fixed target: $\sqrt{s_{FT}} \propto \sqrt{E}$

- $\sqrt{s_{collider}}$ scales with $E$, so, colliders are far more efficient to probe high energy effects

- eg: what energy must the initial proton have to produce the final state in fixed target frame considering the interaction: 
$$p + p \to p + p + p + \bar p$$ 
	- to find: $\sqrt{s}$  in the $COM$ system, where the minimum energy of the final state configuration is clear
	- in the $COM$ system, all final state protons are stationary
	- $\sqrt{s}$ of the final state in the $COM$ frame is: $s_{COM}= (\sum\limits_{i}E_{i})^{2} = 16m_{p}^{2}c^{4}$
	$$\therefore \sqrt{s_{COM}} = 4 m_{p}c^{2}$$
	- in the initial state of the fixed target system: 
$$\begin{align*}
	s_{FT} &= (E+m_{p}c^{2})^{2} - |pc|^{2} \\
	&= 2Em_{p}c^{2}+ 2m_{p}^{2}c^{4}
\end{align*}$$
	- if $s$ is invariant: $\sqrt{s_{COM}} = \sqrt{s_{FT}}$
	$$E = 7 m_{p}c^{2}$$
