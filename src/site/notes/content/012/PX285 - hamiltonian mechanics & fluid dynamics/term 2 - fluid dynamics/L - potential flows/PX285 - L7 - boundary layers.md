---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l7-boundary-layers/","noteIcon":"1","created":"2025-08-27T13:15:28.575+01:00","updated":"2025-03-07T14:37:40.000+00:00"}
---

- when reynold's number, $Re$, is large, the boundary layers are thin:
$$\frac{\delta}{d} = \left(\frac{\mu}{\rho u_{0}d}\right)^{1/2} = \frac{1}{\sqrt{Re}}$$
- typically, $Re \gg 1$, and the boundary layers are thin compared to the object size

- considering the flow around a cylinder, where the flow outside the boundary layer can be taken to be potential

![PX285 - L7 - boundary layers.png|500](/img/user/pics/PX285%20-%20L7%20-%20boundary%20layers.png)

- the pressure on the surface:
$$\begin{gather}
P_{s} (\theta) = P_{0} + \frac{1}{2} \rho u^{2} (1 - 4\sin^{2} \theta) \\
P_{C'} > P_{B'} > P_{A} \\
P_{C} > P_{B} > P_{A}   
\end{gather}$$
- in fluids: 
$$F \propto - \frac{\partial P}{\partial x}$$
- in the upstream region, the pressure gradient accelerates the flow, ie. favourable pressure gradient
- in the downstream region, the pressure gradient decelerates the flow, ie. adverse pressure gradient

![PX285 - L7 - boundary layers-1.png](/img/user/pics/PX285%20-%20L7%20-%20boundary%20layers-1.png)

- considering the flow near the surface, ie. in the boundary layer, using the navier stoke equation:
$$(\vec u \cdot \vec\nabla) \vec u = - \frac{1}{\rho} \vec\nabla P + \frac{\mu}{\rho} \nabla^{2} u$$
- let the density be constant
- using the symmetry of the model:
$$u_{x} \frac{\partial u_{x}}{\partial x} = - \frac{1}{\rho} \frac{\partial P}{\partial x} + \frac{\mu}{\rho} \frac{\partial^{2} {u_x}}{\partial {y}^{2}}$$
- within the boundary layer: $Re$ is small, so the viscous term $\gg$ inertial term
$$\frac{\partial^{2} {u_x}}{\partial {y}^{2}} = \frac{1}{\mu} \frac{\partial P}{\partial x} = A(x)$$
	since there is no acceleration in $x$

- integrating twice:
$$\implies u_{x} = A(x) \frac{y^{2}}{2} + By  + C$$
- the boundary conditions:
$$\begin{gather}
\text{no slip: } u_{x}(y = 0 ) = 0 \\
\text{potential flow: } u_{x}(y = \delta) = u_{0} \\\\
\implies C = 0
\end{gather}$$
- using the second condition:
$$A \frac{\delta^{2}}{2} + B \delta  = u_{0} \implies B =\frac{u_{0}}{\delta} -A \frac{\delta}{2}$$
$$u_{x}(y) = - \frac{A}{2} (y \delta - y^{2}) + \frac{u_{0}}{\delta} y$$
- this works only for $y < \delta$, therefore, $(y \delta - y^{2})$ and $y / \delta>0$ 

- if $A<0: u_{x}> 0$ (flow from left to right)
- if $A>0$ and sufficiently large: $u_{x} < 0$ (flow from right to left, only in the boundary layer)

![PX285 - L7 - boundary layers-2.png|500](/img/user/pics/PX285%20-%20L7%20-%20boundary%20layers-2.png)

- the location along the plate where the flow reverses, ie. $\partial_{y} u_{x} = 0:$
$$\begin{gather}
\frac{\partial u_{x}}{\partial y} = - \frac{A}{2} (\delta - 2y) + \frac{u_{0}}{\delta} = 0 \\
- \frac{A\delta}{2} + \frac{u_{0}}{\delta} = 0 \\
\therefore A = \frac{2u_{0}}{\delta^{2}}
\end{gather}$$
- this is called the **'separation point'**

![PX285 - L7 - boundary layers-3.png|500](/img/user/pics/PX285%20-%20L7%20-%20boundary%20layers-3.png)

- this splitting of the flow due to the flow reversal effect affects the flow outside the boundary layer
- this is called **boundary separation**

- a similar example:

![PX285 - L7 - boundary layers-4.png|500](/img/user/pics/PX285%20-%20L7%20-%20boundary%20layers-4.png)

- incorporating this for the flow around the cylinder:

![PX285 - L7 - boundary layers-5.png|500](/img/user/pics/PX285%20-%20L7%20-%20boundary%20layers-5.png)