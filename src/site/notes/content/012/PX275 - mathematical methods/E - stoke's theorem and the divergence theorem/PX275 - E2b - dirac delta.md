---
dg-publish: true
---

- considering a sphere
![Pasted image 20241121124446.png](/img/user/pics/Pasted%20image%2020241121124446.png)
- for a point charge, $Q$, at the origin, a distance, $r$, from $Q$, the electric field is given by: 
$$\vec E = \frac{Q}{4\pi\varepsilon_{0}r^{2}} \hat e_{r}$$
- for the divergence theorem: 
$$\iint_{S} \vec E \cdot d\vec s = \iiint_{B}(\vec\nabla \cdot \vec E)\, dV$$
### the volume integral
$$\iiint_{V}(\vec\nabla\cdot\vec E) \, dV = \frac{Q}{4\pi\varepsilon_{0}} \iiint_{V} \frac{1}{r^{2}} \underbrace{\frac{\partial }{\partial r}(r^{2} \frac{1}{r^{2}})}_{\frac{\partial}{\partial r}(1)=0}\,dV = 0$$
### the surface integral
$$\vec E = \frac{Q}{4\pi\varepsilon_{0}r^{2}} \hat e_{r}$$
$$\begin{align*}
	\iint_{S} \vec E \cdot \vec ds &= \frac{Q}{4\pi\varepsilon_{0}} \iint_{S} \frac{1}{r^{2}}r^{2}\sin\theta\,d\theta\,d\phi \\
	&= \frac{Q}{4\pi\varepsilon_{0}} \int_{0}^{2\pi}\int_{0}^{\pi} \sin\theta\,d\theta\,d\phi \\
	&= \frac{Q}{4\pi\varepsilon_{0}} 2\pi \,[-\cos\theta]_{0}^{\pi} \\
	\therefore \iint_{S} \vec E \cdot \vec ds&= \frac{Q}{\epsilon_{0}}
\end{align*}$$

- these results are not consistent
## the dirac delta
- in order to define $\vec\nabla\cdot\vec E$ across all space including $r=0:$
$$\vec\nabla\cdot\vec E = \frac{Q}{\varepsilon_{0}} \delta(r)$$
	where, $\delta(r)$ is the **dirac delta**
- in 3D, it is written as $\delta^{3}(r)$
![Pasted image 20241125122420.png](/img/user/pics/Pasted%20image%2020241125122420.png)
- the function is a distribution of infinite height and zero width
$$\int_{-x_{1}}^{x_{2}} \delta(x) \,dx = 1$$
- from the divergence , if $Q$ is within a volume, $V$, then:
$$\iiint_{V} \frac{Q}{\varepsilon_{0}} \delta(\vec r) \, dV = \frac{Q}{\varepsilon_{0}} \iint_{V}\delta(\vec r) \, dV = \frac{Q}{\varepsilon_{0}}$$
- more generally, if the charge, $Q$, is at a position $\vec a$, then define: 
$$\delta (\overrightarrow{r-a}) = 0, \;\forall r\neq 0$$
