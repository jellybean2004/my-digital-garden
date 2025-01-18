---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/h-introduction-to-fluids/px-285-h6c-example-in-a-cylinder/","noteIcon":"1","created":"2025-01-16T14:53:08.375+00:00","updated":"2025-01-17T12:34:26.456+00:00"}
---

![PX285 - H6c - example in a cylinder.png|500](/img/user/pics/PX285%20-%20H6c%20-%20example%20in%20a%20cylinder.png)
- assuming a laminar, steady and viscous flow:
$$\vec u = u_{z}(r)\hat z$$
- considering a fluid element in cylindrical geometry

![PX285 - H6c - example in a cylinder-1.png|500](/img/user/pics/PX285%20-%20H6c%20-%20example%20in%20a%20cylinder-1.png)
![PX285 - H6c - example in a cylinder-2.png|500](/img/user/pics/PX285%20-%20H6c%20-%20example%20in%20a%20cylinder-2.png)
- area of the outer surface:
$$A_{O} = \Delta z (r + \Delta r) \Delta \phi$$
- area of the inner surface:
$$A_{I} = \Delta z \,r\, \Delta \phi$$
$$F_{v} = (r + \Delta r) \Delta z \,\Delta \phi \, \mu \frac{\partial u_{z}}{\partial r} \bigg|_{r+\Delta r} - r\, \Delta\phi \,\Delta z \,\mu \frac{\partial u_{z}}{\partial r}\bigg|_{r}$$
- **note:** areas of the inner and outer surfaces of the chosen fluid element are different (in contrast with the plane case)
- using [[content/011/PX153 - mathematics for physicists/term 1/PX153 - G - functions of many variables, calculus/PX153 - G4 - taylor expansion of a function of two variables\|tayor expansion]]:
$$\frac{\partial u_{z}}{\partial r} \bigg|_{r+\Delta r} \approx  \frac{\partial u_{z}}{\partial r} \bigg|_{r} + \frac{\partial^{2} {u_{z}}}{\partial {r}^{2}}\bigg|_{r}\Delta r +\dots$$
- ignoring all terms in $(\Delta r)^{2}$ or smaller:
$$F_{v}= \mu \, \Delta z \,\Delta\phi \, \Delta r \left(\frac{\partial u_{z}}{\partial r}\bigg|_{r} + r \frac{\partial^{2} {u_{z}}}{\partial {r}^{2}}\bigg|_{r}\right) = \mu \, \Delta z \,\Delta\phi \, \Delta r  \frac{\partial }{\partial r} \left(r \frac{\partial u_{z}}{\partial r}\right)$$

- the pressure force:
$$F_{P} = r \, \Delta \phi \, \Delta r (P(z) - P(z+\Delta z)) = - r\, \Delta\phi \, \Delta r \, \Delta z \frac{\partial P}{\partial z}$$

- since it is a steady motion, there is no acceleration, so the net force must be zero:

$$\begin{gather}
\mu   \frac{\partial }{\partial r} \left(r \frac{\partial u_{z}}{\partial r}\right) = r \frac{\partial P}{\partial z} \\
\mu \frac{1}{r} \frac{\partial }{\partial r} \left(r \frac{\partial u_{z}}{\partial r}\right) = \frac{\partial P}{\partial z} = -Q
\end{gather}$$

- integrating twice and applying boundary conditions: $u_{z}(r= a) = 0$ and $\cfrac{\partial u_{z}}{\partial r} (r=0) = 0$
$$u_{z}(r) = \frac{Q}{4\mu} (a^{2}-r^{2}) = \frac{P_{1}-P_{2}}{4\mu L}(a^{2}-r^{2})$$
- this is again,the **poisseuille flow**