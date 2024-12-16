---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-h-waves-at-boundaries/px-154-h3-standing-waves-and-normal-modes/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:52:43.389+00:00"}
---

## introduction 
- a wave perfectly reflecting from a fixed end. now, the other end is fixed too
- for sinusoidal waves: 
$$u_{total} = A\cos(kx-\omega t)- A\cos(-kx-\omega t)$$
- using trig identity: 
$$u_{total} = 2A\sin(kx)\sin(\omega t)$$
	- $\sin(kx)$ shows position dependence
	- when $\sin(kx)=0$, ie $kx=n\pi$, then, $u_{total}$ is always zero, for $x = \frac{1}{2}\lambda, \lambda, \frac{3}{2}\lambda...$
![Pasted image 20231129102344.png](/img/user/pics/Pasted%20image%2020231129102344.png)
- points with no vibration are *nodes*
- points with maximum/minimum vibrations are *antinodes*

- ***comments***: for a standing wave there is no transfer of power
## modes
- a string of length, $L$, fixed at $x=0$, and $x=L$
- we can only have waves if $u(x,t)|_{x=L}=0$
$$\begin{align*}
	kx &= n\pi \\
	x &= \frac{n\lambda}{2}
\end{align*}$$

- fundamental: ![Pasted image 20231129103153.png](/img/user/pics/Pasted%20image%2020231129103153.png)
		$n=1 \implies \lambda = 2L$
		$f = \frac{v}{2L}$
- first harmonic: ![Pasted image 20231129103736.png](/img/user/pics/Pasted%20image%2020231129103736.png)
		$n=2 \implies \lambda = L$
		$f= \frac{v}{L}$
- second harmonic: ![Pasted image 20231129103832.png](/img/user/pics/Pasted%20image%2020231129103832.png)
		$n=3 \implies \lambda = \frac{2}{3}L$
		$f = \frac{3v}{2L}$	
- third harmonic: ![Pasted image 20231129103957.png](/img/user/pics/Pasted%20image%2020231129103957.png)
		$n=4 \implies \lambda = \frac{1}{2}L$
		$f = \frac{2v}{L}$	
- more in [YF fig 40.11]
- power in the wave: 
$$P= \frac{1}{2}A^{2}\omega^{2}z \propto f^{2}$$
	- the higher modes are more energetic
	- the wavelengths, frequencies, and energies are quantized
	- if a note is played on a piano, the fundamental and combinations of harmonics is produced - requires [fourier analysis]
## waves in open pipes
[YF 16.4]
- check *[[content/011/PX154 - physics foundations/PX154 - G - mechanical waves/PX154 - G5 - waves in bulk gases - sound waves#speed of sound in a ideal gas\|this]]*
- for a both-ends-open pipe, the density and pressure of air at the ends are fixed by the room conditions.
	- density and pressure at the ends of the pipe remain constant, which gives the boundary condition
	- standing waves are obtained
