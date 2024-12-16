---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-d-induction/px-157-d1f-a-falling-magnet-in-a-pipe/","noteIcon":"1","created":"2024-10-01T18:27:10.235+01:00","updated":"2024-11-26T20:10:44.174+00:00"}
---

![Pasted image 20240229165845.png](/img/user/pics/Pasted%20image%2020240229165845.png)
- **TLDR:** 
	- flux at the top decreases, and at the bottom increases
	- emf at the top is positive, and at the bottom is negative
	- eddy currents are generated in each part: CCW at the top and CW at the bottom
	- magnetic fields induced: same polarity as magnet at the top, and opposite polarity at the bottom
	- the top part attracts the magnet as it falls into the pipe
	- once inside, the top part keeps attracting the magnet while the bottom part repels it, slowing it down
	- reaches a terminal velocity once the deceleration equals $g$
	- there is also a radial force, but they cancel out

- a magnet with a [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C9 - magnetic dipole moment#^e299a3\|magnetic dipole moment]] , $\vec\mu_{M}$, in the $z$-direction, and a surface current, $I_{M}$, is in the $\phi$-direction
- the magnet has a mass, $m$, and falls due to gravity, $\vec g = -g\,\hat z$

- [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C1b - magnetic flux\|magnetic flux]]:
	- at $z=z_{a}:$ the magnetic flux decreases, $\frac{d\phi_{B}}{dt}(z_{a})<0$ 
	- at $z=z_{b}:$ the magnetic flux increases, $\frac{d\phi_{B}}{dt}(z_{b})>0$ 

![Pasted image 20240229165917.png](/img/user/pics/Pasted%20image%2020240229165917.png)
- from [[content/011/PX157 - electricity and magnetism/PX157 - D - induction/PX157 - D1a - faraday's law\|faraday's law]]: 
	- at $z=z_{a}:$ an emf, $\epsilon$, generated is counter-clockwise
	- at $z=z_{b}:$ and emf, $\epsilon$, generated is clockwise

- from [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/III - properties/PX157 - B13b - resistance#^9e9b04\|ohm's law]]:
	- the material has a finite resistance, $R$
	- $\epsilon$ drives a circular (eddy) current in the same direction
		- at $z=z_{a}: I=\frac{\epsilon}{R}$ counter-clockwise
		- at $z=z_{b}: I=\frac{\epsilon}{R}$ clockwise

![Pasted image 20240229170740.png](/img/user/pics/Pasted%20image%2020240229170740.png)
- from [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C4a - ampere's law\|ampere's law]]:
	- at $z=z_{a}: \vec\mu_{i} \sim \hat z$
	- at $z=z_{b}: \vec\mu_{i} \sim -\hat z$

![Pasted image 20240229170633.png](/img/user/pics/Pasted%20image%2020240229170633.png)
- force on the magnet:
$$\begin{align*}
	\vec F_{i}\sim I_{M}\,\hat\phi \times \vec B_{i} &= I_{M}\,\hat\phi \times (B_{iR}\,\hat R + B_{iz} \,\hat z) \\
	&= -I_{M}B_{iR}\,\hat z + I_{M}B_{iz}\,\hat R
\end{align*}$$
- $I_{M}B_{iz}\,\hat R=0:$ forces in the radial direction cancels out 
- because $B_{iR}<0:$
$$
\vec F_{i}= I_{M}|B_{iR}|\,\hat z
$$
- the magnet feels an additional force pushing it upwards, acting as a frictional force whose strength is dependent on the resistivity of the material, and is proportional to the magnet's velocity

![Pasted image 20240229171506.png](/img/user/pics/Pasted%20image%2020240229171506.png)
