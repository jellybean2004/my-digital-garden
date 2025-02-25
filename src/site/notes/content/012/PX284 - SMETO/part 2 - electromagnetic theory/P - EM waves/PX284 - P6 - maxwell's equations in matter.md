---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/p-em-waves/px-284-p6-maxwell-s-equations-in-matter/","noteIcon":"1","created":"2025-02-24T10:20:07.508+00:00","updated":"2025-02-24T11:11:55.132+00:00"}
---

- the charge density can be separated into two components: free and bound
$$\begin{gather}
\rho = \rho_{f} + \rho_{b} \\
\rho_{b} = \rho_{P} = - \vec\nabla \cdot \vec P
\end{gather}$$

- also, the current density has two components:
$$\begin{gather}
\vec J = \vec J_{f} + \vec J_{b} \\
\vec J _{b} = \vec J_{P} + \vec J_{M} \\
\vec J_{P} = \frac{\partial  \vec P}{\partial t} \\
\vec J_{M} = \vec\nabla \times \vec M
\end{gather}$$

- the solenoidal condition remains unchanged:
$$\vec\nabla \cdot \vec B = 0$$

- faraday's law does not involve $\rho$ or $\vec J$, so it remains unchanged as well:
$$\vec\nabla \times \vec E = - \frac{\partial \vec B}{\partial t}$$

- gauss' law:
$$\begin{align*}
\vec\nabla\cdot\vec E &= \frac{\rho}{\varepsilon_{0}} \\
&= \frac{\rho_{f} + \rho_{b}}{\varepsilon_{0}} \\
&= \frac{\rho_{f}-\rho_{P}}{\varepsilon_{0}} \\
&= \frac{\rho_{f}-\vec\nabla\cdot\vec{P}}{\varepsilon_{0}}
\end{align*}$$
$$\begin{gather}
\ \vec\nabla\cdot(\varepsilon_{0}\vec E +\vec P) = \rho_{f} \\
\vec D = \varepsilon_{0} \vec E + \vec P
\end{gather}$$
- $\vec D$ is called the **'displacement'**, and gauss' law can be rewritten as:
$$\vec\nabla\cdot\vec D = \rho_{f}$$

- ampere-maxwell law:
$$\begin{align*}
\vec\nabla \times \vec B &= \mu_{0} \left(\vec J + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right) \\
&= \mu_{0} \left(\vec J_{f} + \vec J_{P} + \vec J_{M} + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right) \\
&= \mu_{0} \left(\vec J_{f} + \frac{\partial \vec P}{\partial t} + \vec\nabla \times \vec M + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right) \\
\implies \vec\nabla \times \left(\frac{\vec B}{\mu_{0}} - \vec M \right) &= \vec J_{f} + \frac{\partial }{\partial t} (\varepsilon_{0} \vec E + \vec P) \\
\vec H &= \frac{\vec{B}}{\mu_{0}} - \vec M 
\end{align*}$$
- $\vec H$ is called the **'magnetic field strength'**
- $\vec B$ is called the **'magnetic flux density'**
$$\vec\nabla \times \vec H = \vec J_{f} + \frac{\partial \vec D}{\partial t}$$

- the complete set of maxwell's equations in matter:
$$\begin{gather}
\vec\nabla\cdot\vec D = \rho_{f} \\
\vec\nabla \cdot \vec B = 0 \\
\vec\nabla \times \vec E = - \frac{\partial \vec B}{\partial t} \\
\vec\nabla \times \vec H = \vec J_{f} + \frac{\partial \vec D}{\partial t}
\end{gather}$$
- for the electric case: 
$$\vec P = \varepsilon_{0} \chi \vec E$$
- isotropic: ${} \vec P \parallel \vec E {}$
- linear: ${} \chi \neq \chi(\vec E) {}$
$$\vec D = \varepsilon_{0} \vec E  + \vec P = \varepsilon_{0} (1 + \chi) \vec E = \varepsilon_{0}\varepsilon_{r} \vec E$$

- for the magnetic case:  
$$\vec M = \chi_{M} \vec H$$
	where, $\chi_{M}$ is the magnetic susceptibility
- isotropic: $\vec M \parallel \vec H$
- linear: $\chi \neq \chi(\vec H)$
$$\vec B = \mu_{0}(\vec H + \vec M) = \mu_{0}(1 + \chi_{M})\vec M = \mu_{0}\mu_{r} \vec M$$

- $\chi$ and $\chi_M$ may be freqency dependent
- eg: water molecules (H$_2$O)
- the atoms are aligned at an angle, so there is a dipole
#fig
- in the absence of an electric field, the dipole moments have random orientations due to thermal motion, giving a net zero dipole moment
- when an external field is applied, $\vec E$, the diploes align with the field, giving a net polarization along the direction of $\vec E$
#fig 
- if $\vec E$ is oscillating, molecules/ions need time to reorient themselves, which is les possible at high $\omega$
- therefore, $\chi = \chi(\omega)$ and $\varepsilon_{r} = \varepsilon_{r}(\omega)$, and $\chi_{M} = \chi_{M}(\omega)$ and $\mu_{r} = \mu_{r}(\omega)$

