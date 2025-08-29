---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-a-quantum-phenomena/px-156-d-time-independent-schrodinger-equation/px-156-d5-the-finite-potential-barrier/","noteIcon":"1","created":"2025-08-27T13:14:00.867+01:00","updated":"2024-11-26T20:02:24.000+00:00"}
---

![Pasted image 20240311185330.png](/img/user/pics/Pasted%20image%2020240311185330.png)
- in regions $1$ and $3$, the corresponding [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - D - time independent schrodinger equation/PX156 - D1 - time independent schrödinger equation\|TISEs]] are: 
$$\begin{align*}
		\frac{d^{2}\phi_{1}}{dx^{2}} + \frac{2mE}{\hbar^{2}}\phi_{1} &= 0 \\
		\frac{d^{2}\phi_{3}}{dx^{2}} + \frac{2mE}{\hbar^{2}}\phi_{3} &= 0
	\end{align*}$$
- solutions to these are: 
$$\begin{align*}
		\phi_{1} &= Ae^{ikx}+Be^{-ikx} \\
		\phi_{3} &= Fe^{ikx}+Ge^{-ikx} \\
		k &= \frac{\sqrt{2mE}}{\hbar}
	\end{align*}$$
![Pasted image 20240311185800.png](/img/user/pics/Pasted%20image%2020240311185800.png)
- the incident wave is $\phi_{1+} = Ae^{ikx}$
- the reflected wave is $\phi_{1-} = Ae^{-ikx}$
- the transmitted wave is $\phi_{3+} = Fe^{ikx}$
- there is no left travelling wave in region $3$, therefore $G=0$

- the transmission probability: 
$$T = \frac{|\phi_{3+}^{2}|}{|\phi_{1+}^{2}|} = \frac{FF^{*}}{AA^{*}}$$
- in region 2, the *TISE* is: 
$$\frac{d^{2}\phi_{2}}{dx^{2}} + \frac{2m}{\hbar^{2}}(E-V)\phi_{2} =0$$
- the solution is: 
$$\begin{align*}
	\phi_{2} &= Ce^{ik'x}+De^{-ik'x} \\
	k' &= \frac{\sqrt{2m(E-V)}}{\hbar}
\end{align*}$$
- since $E<V$, $k'$ must be imaginary, therefore define another wavenumber: 
$$k_{2}= -ik' = \frac{\sqrt{2m(V-E)}}{\hbar}$$
- the solution: 
$$\phi_{2} = Ce^{-k_{2}x}+De^{k_{2}x}$$
- boundary conditions at $x=0: \phi_{1}=\phi_{2}\;,\; \frac{d\phi_{1}}{dx}= \frac{d\phi_{2}}{dx}$
- boundary conditions at $x=L: \phi_{2}=\phi_{3}\;,\; \frac{d\phi_{2}}{dx}= \frac{d\phi_{3}}{dx}$

- hence: 
$$\begin{align*}
	A+B &= C+D \\
	ik_{1}A - ik_{1}B &= -k_{2}C + k_{2}D \\
	Ce^{-k_{2}L} + De^{k_{2}L} &= F e^{ik_{3}L} \\
	-k_{2}Ce^{-k_{2}L} + k_{2}De^{k_{2}L} &= ik_{3}Fe^{ik_{3}L}
\end{align*}$$
- a general solution for $A/F$ ratio is possible, but assuming a large barrier (relative to the particle energy) and that the barrier is fairly wide, a good approximation is: 
$$\frac{A}{F} = \left(\frac{1}{2}+ \frac{ik_{2}}{4k_{i}}\right)e^{(ik_{1}+k_{2})L}$$
- this leads to transmission probability: 
$$T = \frac{FF^{*}}{AA^{*}} = \frac{16e^{-2k_{2}L}}{4+\left(\frac{k_{2}}{k_{1}}\right)^{2}}$$
- but: 
$$\left(\frac{k_{2}}{k_{1}}\right)^{2} = \frac{\frac{2m(V-E)}{\hbar^{2}}}{\frac{2mE}{\hbar^{2}}} = \frac{V}{E}-1$$
- therefore, the leading term in the transmission probability is given y the exponent and: 
$$T \propto e^{-2k_{2}L} \propto \exp\left(- \frac{2L\sqrt{2m(V-E)}}{\hbar}\right)$$
![Pasted image 20240311191457.png](/img/user/pics/Pasted%20image%2020240311191457.png)