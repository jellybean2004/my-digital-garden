---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i1-conservation-of-mass/","noteIcon":"1","created":"2025-08-27T13:15:24.187+01:00","updated":"2025-01-31T13:44:08.000+00:00"}
---

- considering a small volume, $V$, of a fluid, bounded by a surface, $S$, with a total area, $A$
- taking a small element of the surface, with a normal vector, $\vec n$, directed outward and through, $d\vec S$
- the mass flow per second through $dS$ is $\rho \vec u \cdot d\vec S$, where $d\vec S = \vec n \, dS$
- the total mass in/outflow through $S:$
$$ \newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}
\oiint_{S} \rho \vec u \cdot d\vec S$$
- the mass of the fluid in the volume, $V$
$$M = \iiint_{V} \rho\, dV$$
- the mass is conserved, so the rate of mass change is equal to the rate of the mass in/outflow
$$\frac{\partial }{\partial t} \iiint_{V} \rho\, dV = -\oiint_{S} \rho \vec u \cdot d\vec S$$
- using the [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E2a - divergence theorem\|divergence theorem]]:
$$\oiint_{S} \vec A \cdot d\vec S = \iiint_{V} (\vec\nabla \cdot \vec A)\,dV$$

$$\begin{gather}
\iiint_{V} \frac{\partial \rho}{\partial t} \, dV + \iiint_{V} \vec\nabla\cdot (\rho\vec u)\, dV = 0 \\
\frac{\partial \rho}{\partial t} + \vec\nabla \cdot (\rho \vec u) = 0
\end{gather}$$
- this is called the **continuity equation**
- **limiting case:** if $\rho =$ constant, the fluid is *incompressible*
$$0 + \rho \vec\nabla \cdot \vec u = 0 \implies \vec\nabla\cdot\vec u = 0$$
