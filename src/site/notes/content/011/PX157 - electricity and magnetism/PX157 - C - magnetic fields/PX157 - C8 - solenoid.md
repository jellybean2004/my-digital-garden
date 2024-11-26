---
dg-publish: true
---
![Pasted image 20240221100822.png](/img/user/pics/Pasted%20image%2020240221100822.png)
- a helical winding of wire, usually a cylinder

- assuming the solenoid is long, so the edge effects can be neglected
- assuming the number of turns per unit length, $n$, is large, ${} n>>1$, so axial symmetry can be assumed
- assuming the wire is wound forward and backward so there is no net current along the axis

- using cylindrical coordinates, $(R,\phi,z)$, with $z$-direction along the axis
- the solenoid has radius, $a$, and the current flows in the positive $\phi$-direction

- by symmetry, $|\vec B|$ is a function of $R$ alone
$$
\vec B (R) = B_{R}(R)\,\hat R+ B_{\phi}(R)\,\hat\phi + B_{z}(R)\,\hat z
$$

- **step 1:**
	![Pasted image 20240221100852.png](/img/user/pics/Pasted%20image%2020240221100852.png)
	- applying [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C4a - ampere's law\|ampere's law]] to path $C:$
$$
\oint_{C}\vec B \cdot d\vec l = \mu_{0}I_{encl.}
$$
	- $d\vec l = dl\,\hat \phi \implies \vec B \cdot d\vec l = B_{\phi}dl:$
$$
\oint_{C}\vec B\cdot d\vec l = \oint_{C}B_{\phi}\,dl = B_{\phi}2\pi R
$$
	- $I_{encl.}=0$, no current passing though the cross-section:
$$
B_{\phi} 2\pi R = 0\implies B_{\phi}=0
$$
- **step 2:** solenoidal condition
	![Pasted image 20240221100910.png](/img/user/pics/Pasted%20image%2020240221100910.png)
	$$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}
	  \oiint_{S}\vec B\cdot d\vec S =0$$
	$$\oiint_{S}\vec B\cdot d\vec S = \iint_{left}\vec B \cdot (-\hat z)dS + \iint_{right} \vec B\cdot (+\hat z)dS + \iint_{curved}\vec B \cdot \hat R\,dS$$
	- left and right cancel due to symmetry as solution does not depend on z
	$$\iint_{curved}\vec B \cdot \hat R\,dS=0 \implies \iint B_{R}\,dS = B_{R} 2\pi RL \implies B_{R}=0$$

- **step 3:**
	![Pasted image 20240221100927.png](/img/user/pics/Pasted%20image%2020240221100927.png)
	- choosing a rectangular path in the plane of constant $\phi$ outside the solenoid and applying [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C4a - ampere's law\|ampere's law]]:
$$\begin{align*}
		\oint_{C} \vec B\cdot d\vec l &= \int_{a}^{b} \vec B\cdot d\vec l + \int_{b}^{c} \vec B\cdot d\vec l + \int_{c}^{d} \vec B\cdot d\vec l + \int_{d}^{e} \vec B\cdot d\vec l\\
		&=\int_{0}^{L} \vec B\cdot \hat z\,dz + \int_{R_{1}}^{R_{2}} \vec B\cdot \hat R\,dR + \int_{L}^{0} \vec B\cdot \hat z\,dz + \int_{R_{2}}^{R_{1}} \vec B\cdot \hat R\,dR \\
		&= \int_{L}^{0} B_{z}(R_{1})\,dz + \int_{R_{1}}^{R_{2}} B_{R}\,dR + \int_{0}^{L} B_{z}(R_{2})\,dz + \int_{R_{2}}^{R_{1}} B_{R}\,dR \\\\
		since\; B_{R} &= 0: \\\\
		\oint_{C} \vec B\cdot d\vec l &= B_{z}(R_{1})L - B_{z}(R_{2})L = \mu_{0}I_{encl.}
	\end{align*}$$
	- outside the solenoid, $I_{encl.}=0:$
$$
B_{z}(R_{1}) = B_{z}(R_{2})
$$
	- $B_{z}$ is constant outside
	- taking $R_{2}\to \infty: B_{z}(R_{2}\to \infty) =0$ 
	- $B_{z}=0$ outside

- **step 4:**
	![Pasted image 20240221100940.png](/img/user/pics/Pasted%20image%2020240221100940.png)
	- choosing a rectangular path in a plane of constant $\phi$, in and out of the solenoid and applying [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C4a - ampere's law\|ampere's law]]:
$$
\oint_{c}\vec B\cdot d\vec l = B_{z}(R_{1})L - B_{z}(R_{2})L
$$
	- since $R_{2}>a$ (outside) $: B_{z}(R_{2})=0:$
$$\begin{align*}
			\oint_{C} \vec B \cdot d\vec l = B_{z}(R_{1})L &= \mu_{0}NI = \mu_{0}nLI \\
			B_{z}(R_{1}) &= \mu_{0}nI
		\end{align*}$$
$$\therefore \vec B = \begin{cases}
     & \vec 0 & outside \\
     & \mu_{0}nI \hat z & inside
\end{cases}$$

- for a solenoid that is not infinitely long, all field lines must pass though the cross-section, $\pi a^{2}$, but outside the solenoid, the field lines can pass though anywhere. therefore, the field density outside is much smaller in comparison to that inside the solenoid. hence, the above result is sensible
