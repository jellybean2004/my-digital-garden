---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/o-introduction-to-emt/px-284-ox-maxwell-s-equations-in-free-space/","noteIcon":"1","created":"2025-02-11T10:05:30.774+00:00","updated":"2025-02-11T10:14:24.310+00:00"}
---

- **gauss'** law:
$$\vec\nabla\cdot\vec E = \frac{\rho}{\varepsilon_{0}}$$
- **'the law with no name'** AKA the **solenoidal condition**:
$$\vec\nabla\cdot\vec B = 0$$
- **faraday-lenz** law:
$$\vec\nabla \times \vec E = - \frac{\partial \vec B}{\partial t}$$
- **ampere-maxwell** law:
$$\vec\nabla \times \vec B = \mu_{0}\left( \vec J + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right)$$

- additionally, **conservation of charge**: 
$$\frac{\partial \rho}{\partial t} + \vec\nabla\cdot\vec J = 0$$
	- this is the continuity equation

- with **no sources**, the equations become:
$$\begin{gather}
\vec\nabla\cdot\vec E = 0 \\
\vec\nabla\cdot\vec B = 0 \\
\vec\nabla \times \vec E = - \frac{\partial \vec B}{\partial  t} \\
\vec\nabla \times \vec B = \mu_{0}\varepsilon_{0} \frac{\partial \vec E}{\partial t}
\end{gather}$$