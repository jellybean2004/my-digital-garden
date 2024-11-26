---
dg-publish: true
---

- operations on the description of a system which leaves the physics unchanged
- eg: adding a zero point to a potential does not change the physics

|      symmetry       | conserved quantity |
| :-----------------: | :----------------: |
| wavefunction phase  |  electric charge   |
| upness and downness | electroweak charge |
|       colour        |   colour charge    |
- these are known as *gauge symmetries*

- in quantum mechanics, a particles is described using a complex valued [[content/011/PX154 - physics foundations/PX154 - F - waves/PX154 - F1b - the wave function\|wavefunction]], $\psi$
- it holds all the information about the state of the particle
- probability of the particle being in the state is: 
$$P = |\psi|^{2} = \psi^{*}\psi$$
- the probability is an observable but $\psi$ can be changed without changing the probability
- define: $\psi' = e^{i\chi}\psi$, where, $\chi=$ constant
- but: 
$$\begin{align*}
	P(\psi') &= |\psi'|^{2} \\
	&= \psi'^{*}\psi \\
	&= (e^{-i\chi}\psi^{*})(e^{i\chi}\psi) \\
	&= \psi^{*}\psi \\
	&= |\psi|^{2} \\
	\therefore P(\psi') &= P(\psi)
\end{align*}$$
- changing the **global phase** doesn't affect the physics
- this is a 'global' symmetry as it appears at every point in space-time by the same amount, $\chi$ 

- global changes do not agree with special relativity
- want to change the phase by different amounts at different space-time points and have no effect on the physics, ie: $\chi\to\chi(\vec x, t)$ 
- the physics should be unchanged when a change, $\psi' = e^{i\chi(\vec x,t)}\psi$, is made
- this is called **'local' symmetry**
- this will still satisfy $|\psi'|^{2} = |\psi|^{2}$ 
- $\psi$ obeys the [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - C - quantum mechanics/PX156 - C1 - the schrodinger equation\|the schrodinger equation]], so should $\psi'$
$$\begin{align*}
		\vec\nabla\psi &= -ih \frac{\partial \psi}{\partial t} \\\\
		\vec\nabla\psi' &= \vec\nabla (e^{i\chi(\vec x,t)}\psi) \\
		&= e^{i\chi(\vec x,t)}\vec\nabla\psi + \psi e^{i\chi(\vec x,t)} \vec\nabla\chi(\vec x,t)
	\end{align*}$$
- the second term spoils the invariance of the symmetry

- to make the physics invariant to local changes, new things need to be added to the theory, which cancel the effect of the $\vec\nabla\chi(\vec x,t)$ term
- these new things are *boson fields* $\implies$ bosons are needed $\implies$ interactions of particles and bosons $\implies$ charge conservation
- charge conservation comes from symmetries to phase changes
- ***the standard model*** is a "*gauge theory*"
- this idea lies at the heart of theoretical particle physics