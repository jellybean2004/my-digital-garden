---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/q-maxwell-s-equations-in-matter/px-284-q4-boundary-conditions/","noteIcon":"1","created":"2025-02-27T15:11:21.337+00:00","updated":"2025-02-27T15:50:47.496+00:00"}
---

#fig 

- using faraday-lenz law and stokes' theorem:
$$\begin{gather}
\iint_{S} \vec\nabla \times \vec E \cdot d\vec S = \oint_{C }\vec E\cdot d\vec l = \iint_{S} \left(- \frac{\partial \vec B}{\partial t}\right) \cdot d\vec S \\
= (E_{2,\parallel} - E_{1,\parallel}) \times L + O(d)
\end{gather}$$
where, $O(d)$ is the order of $d$, ie. it goes linearly with $d$

- in the limit $d\to 0: S \to 0$
$$E_{2,\parallel} - E_{1,\parallel} = 0$$
- this is assuming that $-\partial_{t}\vec B$ is finite
- this is true for any orientation of loop with $L$ outside the plane of the boundary
- writing it as: 
$$\hat n \times (\vec E_{2} - \vec E_{1}) = 0$$
	where, $\hat n$ is the unit vector normal to the boundary
- this means that $E_\parallel$ is continuous across the boundary

- doing the same with ampere-maxwell law:
$$\begin{gather}
\iint_{S} \vec\nabla\times\vec H \cdot d\vec S  = \oint_{C}  \vec H \cdot d\vec l = \iint_{S} \left(\vec J_{f} + \frac{\partial \vec D}{\partial t}\right) \cdot d\vec S \\
\implies \hat n \times (\vec H_{2} - \vec H_{1}) = 0
\end{gather}$$
- ie. $\vec H$ is continuous across the boundary
- this is assuming that $\iint_{S} \vec J_{f} \cdot d\vec S = 0$
- if surface currents are present:
$$\hat n \times (\vec H_{2}  - \vec H_{1}) = \vec j_{f} $$
	where, $\vec j_{f}$ is the surface current density, with units A m$^{-1}$

#fig 

- when resistivity $\to 0$, ie. superconductors, $\vec j_f$ acts to expel magnetic fields, ie: $H_{2} = 0$


#fig 
$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}$
- considering a pill box on the surface
$$\oiint_{S} \vec B \cdot d\vec S = (B_{1\perp} - B_{2\perp})A + O(h) = \iiint_{V} \vec\nabla\cdot\vec B \, dV = 0$$
- $O(h) \to 0$ as $h\to0$
$$\therefore B_{1\perp} = B_{2\perp}$$
- similarly, for $\vec D:$
$$\oiint_{S} \vec D \cdot d\vec S  = (D_{1\perp} - D_{2\perp}) A + O(h) = \iiint_{V} \vec\nabla\cdot\vec  D \, dV = \iiint_{V}\rho_{f} \, dV =Q_{f}$$
	where, $Q_{f}$ is the charge enclosed
- $O(h) \to 0$ as $h\to0$
- $Q_f$ can contain contribution from surface charges
$$Q_{f} = \iiint_{V} \rho_{f} \, dV + \iint_{S} \sigma_{f}\,dS$$
	where, $\rho_{f}$ is the volume charge density, and $\sigma_{f}$ is the surface charge density

- as $h \to 0$, the volume charge $\to 0$, but the surface charge remains $\sigma_{f}A$

$$\therefore D_{1\perp} - D_{2\perp} = \sigma_{f}$$

- additionally, in conductors, the currents ($\vec J_{f}$) also need to be considered
## summarized
$$\begin{gather}
\hat n \times ((\vec E_{2} - \vec E_{1})) = 0 \\
\hat n \cdot ((\vec D_{1} - \vec D_{2})) = \sigma_{f} \\
\hat n \cdot ((\vec B_{1} - \vec B_{2})) = 0 \\
\hat n \times ((\vec H_{2} - \vec H_{1})) = \vec j{f} 
\end{gather}$$
