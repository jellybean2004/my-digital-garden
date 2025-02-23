---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/p-em-waves/px-284-p2-energy-in-em-fields/","noteIcon":"1","created":"2025-02-17T10:36:15.302+00:00","updated":"2025-02-23T13:25:29.515+00:00"}
---

- for a conservation law, there must be a continuity equation:
$$\frac{\partial u}{\partial t} + \underbrace{\vec\nabla \cdot \vec P}_\text{energy flux} = - W$$
	where, $u$ is the energy density,  $W$ is the work done per unit volume per unit time

- the lorentz force:
$$\vec F = Q \vec E = \rho \Delta V \vec E$$
	where, $\rho$ is the charge density, and $\Delta V$ is the volume element

- the rate of doing work on $\Delta V:$
$$\begin{gather}
W \Delta V = \rho \Delta V \vec E \cdot \vec v = \Delta V \vec E \cdot (\rho \vec v) \\\\
\vec J = \rho \vec v \\
\implies - W = - \vec E \cdot \vec J = - \vec E \cdot \left(\frac{\vec\nabla\times\vec{B}}{\mu_{0}} - \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right)
\end{gather}$$

- using the vector identity:
$$\vec\nabla \cdot ( \vec E \times \vec B) = \vec B \cdot (\vec\nabla \times \vec E) - \vec E \cdot (\vec\nabla \times \vec B)$$
$$\begin{align*}
\implies - W &= \frac{\vec\nabla\cdot (\vec E \times\vec B)-\vec B \cdot (\vec\nabla \times\vec E)}{\mu_{0}} + \varepsilon_{0} \vec E \cdot \frac{\partial \vec E}{\partial t} \\
&= \vec\nabla \cdot \frac{\vec E \times \vec B}{\mu_{0}} + \frac{1}{\mu_{0}}\vec B \cdot \frac{\partial \vec B}{\partial t} + \varepsilon_{0}\vec E \frac{\partial \vec E}{\partial t} \\
&= \vec\nabla \cdot \underbrace{\frac{\vec E \times \vec B}{\mu_{0}}}_{P} + \frac{\partial }{\partial t} \underbrace{\left(\frac{B^{2}}{2\mu_{0}} + \varepsilon_{0} \frac{E^{2}}{2}\right)}_{u} \\
\therefore - W &= \frac{\partial u}{\partial t} + \vec\nabla \vec P
\end{align*}$$
