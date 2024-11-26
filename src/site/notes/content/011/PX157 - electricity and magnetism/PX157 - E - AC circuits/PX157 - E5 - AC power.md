---
dg-publish: true
---
- power in circuits with inductors and capacitors
- typically, $I$ and $V$ are $\pm90\degree$ out of phase:
$$\begin{align*}
		V(t) &= V_{0}\cos(\omega t)\\
		I(t) &= I_{0}\sin(\omega t)
	\end{align*}$$
- instantaneous power:
$$
P(t) = V(t)I(t) = V_{0}I_{0}\cos(\omega t)\sin(\omega t)
$$
- average power over a cycle:
$$\begin{align*}
		\langle{P}\rangle &= \frac{1}{T}\int_{0}^{T} P(t)\,dt \\
		&= \frac{1}{T} \int_{0}^{T} V_{0}I_{0}\cos(\omega t)\sin(\omega t)\, dt \\
		&= \frac{V_{0}I_{0}}{2T} \int_{0}^{T} \sin(2\omega t)\, dt \\
		&= 0
	\end{align*}$$
- no electrical energy dissipated over a cycle in pure inductors and capacitors

# circuits with a resistive load
- instantaneous power:
$$
P(t) = RI^{2}(t) = RI_{0}^{2}\cos^{2}(\omega t)
$$
- average power:
$$\begin{align*}
		\langle{P} \rangle &= \frac{1}{T} \int_{0}^{T} RI_{0}^{2} \left(\frac{1}{2}+ \frac{1}{2}\cos(2\omega t)\right)\,dt \\
		&= \frac{RI_{0}^{2}}{2}
	\end{align*}$$
- *root-mean-square* current and potential:
$$\begin{align*}
		I_{rms}&= \frac{I_{0}}{\sqrt{2}} \\
		V_{rms}&= \frac{V_{0}}{\sqrt{2}} \\
		\langle{P}\rangle &= R I^{2}_{rms} \\
		&= V_{rms}I_{rms} \\
		&= \frac{V^{2}_{rms}}{R}
	\end{align*}$$
## general power dissipation
- it is expected that the power delivered by the source is equal to the power dissipated in the resistor
### power from source
$$\begin{align*}
	V(t) &= V_{0}\cos(\omega t) \\
	I(t) &= I_{0}\cos(\omega t+\phi) \\
	P(t) &= V_{0}I_{0}\cos(\omega t)\cos(\omega t+\phi) \\
	&= V_{0}I_{0} \cos(\omega t) \, [\cos(\omega t)\cos(\phi)-\sin(\omega t)\sin(\phi)] \\
	&= V_{0}I_{0} \cos^{2}(\omega t)\cos(\phi)- V_{0}I_{0}\sin(\omega t)\cos(\omega t)\sin(\phi) \\\\
	\langle{P}\rangle &= \frac{1}{2}V_{0}I_{0}\cos\phi \\
	&= V_{rms}I_{rms}\cos\phi
\end{align*}$$
- $\cos\phi$ is the *power factor*
### power dissipated in the source
$$\begin{align*}
	P(t) &= V_{R}(t) I(t) \\
	I(t) &= I_{0}\cos(\omega t+\phi) \\
	V_{R}(t) &= V_{R_0}\cos(\omega t+\phi) \\\\
	\langle{P}\rangle &= \langle{V_{R}I}\rangle \\
	&= V_{R_{0}} I_{0} \langle{\cos^{2}(\omega t+\phi)}\rangle \\
	&= \frac{1}{2}V_{R_{0}} I_{0} \\
	&= \frac{1}{2}R I_{0}^{2} \\
	&= R I_{rms}^{2}
\end{align*}$$
- the power factor has disappeared!
![Pasted image 20240322170407.png](/img/user/pics/Pasted%20image%2020240322170407.png)
$$\begin{align*}
	\langle{P}\rangle &= \frac{1}{2}V_{0}I_{0} \cos\phi \\
	&= \frac{1}{2}I_{0} ^{2}Z\cos\phi \\
	&= \frac{1}{2}RI_{0}^{2}
\end{align*}$$

