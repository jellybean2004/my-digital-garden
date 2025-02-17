---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/o-introduction-to-emt/px-284-o3-charge/","noteIcon":"1","created":"2025-02-13T15:26:44.312+00:00","updated":"2025-02-13T15:30:13.124+00:00"}
---

## current density
- considering a cylindrical conductor, with a cross-section, A, and charge density, $\rho$
- the charges are travelling at a speed, $v$
- so, the charge through $A$ in time, $\delta t:$
$$Q = \rho  A v \, \delta t$$
- the charge density:
$$\vec J = \rho \vec v$$
## conservation of charge
$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}$
$$\oiint \vec J \cdot d\vec S =- \frac{d}{dt} Q_{\text{encl.}} = - \frac{d}{dt} \iiint_{V} \rho \, dV$$
- using the [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E2a - divergence theorem\|divergence theorem]]:
$$\begin{gather}
\oint_{S} \vec J \cdot d\vec S  = \iiint_{V} \vec\nabla\cdot\vec J \, dV = - \frac{d}{dt} \iiint_{V}\rho \,dV \\ 
\iiint_{V} \left(\frac{\partial \rho}{\partial t} + \vec\nabla\cdot\vec J\right) \, dV = 0 \\
\frac{\partial \rho}{\partial t} + \vec\nabla\cdot\vec J  = 0
\end{gather}$$
- this is the **continuity equation** for the conservation of charge
