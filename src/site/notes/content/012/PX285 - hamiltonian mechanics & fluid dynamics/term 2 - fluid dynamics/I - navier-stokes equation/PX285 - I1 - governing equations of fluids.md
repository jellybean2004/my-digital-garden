---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i1-governing-equations-of-fluids/","noteIcon":"1","created":"2025-01-23T14:07:52.564+00:00","updated":"2025-01-23T15:09:33.627+00:00"}
---

## the conservation of mass
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
\frac{\partial \rho}{\partial t} = \vec\nabla \cdot (\rho \vec u) = 0
\end{gather}$$
- this is called the **continuity equation**
- **limiting case:** if $\rho =$ constant, the fluid is *incompressible*
$$0 + \rho \vec\nabla \cdot \vec u = 0 \implies \vec\nabla\cdot\vec u = 0$$

## conservation of momentum
- considering a *lagrangian* fluid element of volume, $V$, that moves at the fluid velocity, ${} \vec u {}$
	- *lagrangian*: its mass is constant, ie: $\rho\,dV =$ constant
- the rate of change of momentum:
$$\frac{d}{dt} (\rho\, dV\, \vec u) = \rho \, dV \frac{d\vec{u}}{dt}$$
	where, $\cfrac{d\vec{u}}{dt} = \cfrac{\partial \vec u}{\partial t} + (\vec u \cdot \nabla) \vec u$
- momentum conservation is newton's second law:
$$\begin{gather*}
\vec F = m \vec a  = \rho\, dV \, \frac{d\vec u}{dt} \\
\implies \rho \frac{d \vec u}{dt} = \sum\limits \frac{\vec F}{dV} = - \vec\nabla P + \vec F_{v} + \rho \vec g + \dots
\end{gather*}$$
- this is the **navier-stokes equation**

- the viscous force:
$$\vec F = \mu \nabla^{2}\vec u + \lambda \nabla (\vec\nabla \cdot \vec u)$$
	where, $\mu$ and $\lambda$ arise from the shear and volume viscosities, respectively
- often, $\lambda = \mu/3$
- in incompressible fluid, $\vec\nabla\cdot\vec u = 0$

- need for additional equation for $P$, which comes from the conservation of energy
- only adiabatic processed will be covered
- if the state equation of the fluid is the [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state\|ideal gas law]]
- for the adiabatic condition:
$$PV^{\gamma} = \text{constant}$$
	where, $\gamma = \frac{C_{P}}{C_{V}}$ is the adiabatic index $\approx 5/3$

$$\frac{d}{dt}(P V^{\gamma)}= 0$$

$$\begin{gather}
m^{\gamma}  \frac{d}{dt} \left(\frac{P}{\rho^{\gamma}}\right)= 0 \\ \implies \frac{d}{dt} \left(\frac{P}{\rho^{\gamma}}\right)= 0
\end{gather}$$
