---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/k-phonons/px-284-k1-einstein-model/","noteIcon":"1","created":"2025-01-23T15:15:39.086+00:00","updated":"2025-01-23T15:33:15.683+00:00"}
---

- considering lattice vibrations in a crystalline solid, eg: sound waves
- thinking about normal modes of masses connected by springs
- at high temperatures: $C_{V} \to 3Nk_{B}$ 

## assumptions
- each atom is an independent simple harmonic oscillator
	- lattice vibrations are quantized, **phonons**
	- in a crystal of $N$ atoms, there are $3N$ independent modes
- all atoms oscillate with the same frequency, $\omega_{E}$
	- making a very simple DOS
	- thus, $Z = (Z_{SHO})^{3N}$
$$U = 3N \,U_{SHO} = 3N \hbar\omega_{E }\left(\frac{1}{2} + \frac{1}{\exp(\beta \hbar \omega_{E})-1}\right)$$
- ignoring ZPE and replacing $\hbar \omega_{E}$ with $k_{B}\theta_{E}$, where, $\theta_{E}$ is the einstein temperature
$$U = \frac{3Nk_{B}\theta_{E}}{\exp(\beta \hbar \omega_{E})-1}$$
$$\begin{align*}
C_{V} &= \left(\frac{\partial U}{\partial T}\right)_{V} \\
&= 3Nk_B \frac{x^{2}\,e^{x}}{(e^{x}-1)^{2}}
\end{align*}$$
	where, $x = \theta_{E}/T$
- at low $T: x\to \infty, \; C_{V} \to 3Nk_{B}x^{2}e^{-x}$
- at high $T: x \to 0 ,\; e^{x}\to 1+ x , \; C_{V} \to 3N k_{B}$

- this works really well at high and intermediate temperatures, but usually not great at low temperatures
