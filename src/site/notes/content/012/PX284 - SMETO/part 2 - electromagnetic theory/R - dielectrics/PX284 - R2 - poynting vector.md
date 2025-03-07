---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/r-dielectrics/px-284-r2-poynting-vector/","noteIcon":"1","created":"2025-03-06T15:40:16.206+00:00","updated":"2025-03-06T17:36:28.933+00:00"}
---

- the continuity equation:
$$- W = \frac{\partial u}{\partial t} + \vec\nabla\cdot\vec  S $$
	where, $u$ is the energy density, and $\vec S$ is the energy flux, $W$ is the rate of doing work per unit volume on free charges

- from newton's third law:
$$-W =  - \vec E \cdot \rho_{f} \vec v = - \vec E \cdot \vec J_{f} = - \vec E \cdot \left(\vec\nabla\times\vec H - \frac{\partial \vec D}{\partial t}\right)$$
$$\vec\nabla \cdot (\vec E \times \vec H ) = \vec H \cdot (\vec\nabla \times \vec E) - \vec E \cdot (\vec\nabla\times\vec H)$$

$$\begin{align*}
- W &= \vec\nabla\cdot (\vec E \times \vec H) - \vec H \cdot (\vec\nabla \times \vec E) -\vec E \cdot \frac{\partial \vec D}{\partial t} \\
&= \vec\nabla \cdot (\vec E \times \vec H) + \frac{\partial  }{\partial t} \left(\frac{\vec H\cdot \vec B + \vec D \cdot \vec E}{2}\right)
\end{align*}$$
- the poynting vector:
$$\vec S = \vec E \times \vec H$$
- the energy density:
$$u = \frac{\vec H\cdot \vec B + \vec D \cdot \vec E}{2}$$
- $\vec S \perp \vec E , \vec H$ and therefore $\vec S \parallel \vec k$
- the magnitude:
$$S = EH = \frac{E^{2}}{Z }= ZH^{2} $$
- $Z$ is frequency dependent, therefore, so is $S$
$$\begin{gather}
\vec S = \vec E \times \vec H \implies Re(\vec E) \times Re(\vec H) \\
|\vec S | = E_{0} \cos \omega t \, H_{0} \cos\omega t = \frac{E_{0}^{2}}{Z} \cos^{2}\omega t
\end{gather}$$
- average over time:
$$\bar S = \frac{E_{0}^{2}}{Z} \frac{1}{2} = \frac{E_{RMS}^{2}}{Z}$$
- this is useful when considering waves of different frequencies, eg: sunlight: $\bar S_{earth} = 1300\,\text{Wm}^{-2}$
- the impedance of air $\simeq Z_{0} = 377\, \Omega$
- so, $E_{RMS} = \sqrt{Z_{0} \bar S_{earth}} \simeq 700\, \text{Vm}^{-1}$
- energy flux implies a momentum flux / radiation pressure: $E = pc$
- the momentum flux, ie. a pressure:
$$\frac{\vec S}{c} = \frac{\vec E \times \vec H}{c}$$
- eg: sunlight on earth: $|p_{rad}| \simeq 4.3\times10^{-6}$ Nm$^{-2}$
- radiation pressure can be significant
	- large area, eg: solar sails
	- more luminous radiation, eg: in very massive stars, the effect of $p_{rad}$ can balance gravity, limiting the size and power of star

## in a current carrying conductor
- consider a cylindrical with a cross-sectional area, $A$, carrying a current in the same direction as $\vec E$
- from the right hand rule, $\vec H$ loops around the wire
- $\vec S = \vec E \times \vec E$, the pointing vector always points into the wire
- $|\vec E| = V/L$, $|\vec H| = I/2\pi r$, so, the energy that enters the wire: 
$$|\vec S| A = \frac{VIL2\pi r}{L2\pi r} = VI =E$$
- this is equal to the energy dissipated in the wire
- 