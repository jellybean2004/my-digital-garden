---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/q-maxwell-s-equations-in-matter/px-284-q2-magnetization/","noteIcon":"1","created":"2025-02-20T17:39:31.896+00:00","updated":"2025-02-24T17:45:19.280+00:00"}
---

- bound charges can also flow and cause currents
 
![PX284 - P5 - magnetization.png|500](/img/user/pics/PX284%20-%20P5%20-%20magnetization.png)

- the magnetic dipole moment:
$$\vec m = I \vec A$$
	where, $\vec A$ is normal to surface following the right hand rule
- units: A m$^{2}$
- magnetization magnetic dipole moment per unit volume:
$$\vec M = \frac{\sum\limits_{i\in V} \vec m_{i} }{V}$$
- considering a bar magnet
- the equivalent net cur rent will be a current around the outside of the material

![PX284 - P5 - magnetization-1.png|500](/img/user/pics/PX284%20-%20P5%20-%20magnetization-1.png)

- uniform magnetization can be modelled as a uniform grid of current loops in x-y plane

![PX284 - P5 - magnetization-2.png|500](/img/user/pics/PX284%20-%20P5%20-%20magnetization-2.png)

- considering a block of volume $\Delta x \, \Delta y \, \Delta z:$
$$m_{z} = I \Delta x \, \Delta y$$
- the current density:
$$j_{z} = \frac{I}{\Delta z}$$
	which is the current in the x-y plane

- the magnetization:
$$M_{z} = \frac{m_{z}}{\Delta x \, \Delta y \, \Delta z} = \frac{I}{\Delta z} = j_{z}$$

- generalize to all directions:
$$\vec j_{M} = \vec M \times \hat n$$


- the net current between blocks centred at $x_0$ and $x_{0}+ \delta x:$
$$\Delta \vec I = -  \frac{\partial I}{\partial x}\bigg|_{x_{0}} \Delta x \, \hat y = - \frac{\partial }{\partial x} M_{z}  \Delta x \, \Delta z \, \hat y$$
- the bulk current density (current per unit area):
$$J_{y} = - \frac{\partial }{\partial x}M_{z}$$
- generalizing in 3D:
$$\vec J = \vec\nabla \times \vec M$$
- units: A m$^{-2}$