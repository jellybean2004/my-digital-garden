---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/i-field/px-157-b5b-electric-field-from-a-uniformly-charged-sphere/","noteIcon":"1","created":"2024-10-01T18:27:10.071+01:00","updated":"2024-11-26T20:07:23.704+00:00"}
---

![Pasted image 20240117152740.png](/img/user/pics/Pasted%20image%2020240117152740.png)
$$
\rho = \frac{Q}{V} = \frac{Q}{\frac{4}{3}\pi a^{3}}
$$
- **step 1: symmetry**
	- $\vec E$ points radially outwards if $Q>0$ , ie: $\vec E = E \, \hat r$
	- $|\vec E|$ is constant on a sphere centred on the charged sphere, ie: $E(r)$
- **step 2: gaussian surface**
	- sphere of radius, $r$, centred on the charged sphere
	$$\begin{align*}
	d\vec S &= dS \, \hat r \\
	\vec E \cdot d\vec S &= E \, \hat r \cdot dS \, \hat r = E \, dS \\
	\therefore \;\oiint \vec E \cdot d\vec S &= \oiint E \, dS = E \, 4\pi r^{2}
	\end{align*}$$
- **step 3:** 
	- if $r>a: Q_{encl.} = Q$ 
	- if $r\leq a : Q_{encl.} = \rho V_{GS} = \rho \frac{4\pi}{3}r^{3}= Q (\frac{r}{a})^{3}$
- **step 4:**$$\begin{align*}
E \, 4\pi r^{2} &= \begin{cases}
\frac{Q}{\epsilon_{0}} & r>a \\
\frac{Q}{\epsilon_{0}}(\frac{r}{a})^{3} & r \leq a
\end{cases}\\
E &= \begin{cases}
\frac{Q}{4\pi r^{2}\epsilon_{0}} & r>a \\
\frac{Q}{4\pi a^{2}\epsilon_{0}}(\frac{r}{a}) & r \leq a
\end{cases} \\
\therefore \vec E &= \begin{cases}
\frac{Q}{4\pi r^{2}\epsilon_{0}} \hat r & r>a \\
\frac{Q}{4\pi a^{2}\epsilon_{0}}\left(\frac{r}{a}\right)\hat r & r \leq a
\end{cases} \\
\end{align*}$$
![Pasted image 20240125100945.png](/img/user/pics/Pasted%20image%2020240125100945.png)
