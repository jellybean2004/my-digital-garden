---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-c-thermal-physics-2/px-154-c6-kinetic-molecular-model-of-the-ideal-gas/","noteIcon":"1","created":"2025-08-27T13:14:08.623+01:00","updated":"2024-11-26T23:14:08.000+00:00"}
---

- links the *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state#^b45b14\|ideal gas equation]]* to the motion of the gas molecules
## derivation
- how collisions of the molecule lead to pressure
- consider a volume of $V$ filled with an ideal gas of $N$ molecules, each of mass $m$ 
 ![Pasted image 20231031185107.png](/img/user/pics/Pasted%20image%2020231031185107.png)
- firstly, consider just one molecule of gas moving in 3D with a velocity of $\vec v$ 
- consider an *elastic* collision with the shaded wall
- in the collision,  *$x$ component is reversed* but *$y$ and  $z$ components are unchanged*
- the change in momentum is then $2mv_x$
- we need to know the rate at which collisions occur with the wall for the gas 
- how many molecules hit the wall in a time $dt$?
- molecules have an x-component of velocity  $v_x$
- in time $dt$, they can move a direction of $v_xdt$, so, only molecules less than $v_xdt$ can hit the wall
![Pasted image 20231018165339.png](/img/user/pics/Pasted%20image%2020231018165339.png)
$$n_{col}= \frac{1}{2}\frac{N}{V}Av_xdt$$
	- where, $V=$ number density
- only half the molecules are likely to be moving towards the wall at given time $\therefore \frac{1}{2}$
- so, change in momentum $dQ$ in time $dt$:
$$dQ=n_{col}2mv_{x}=\frac{N}{V}Amv_x^2dt$$
- this causes a force [YF eqn 18.10] : 
$$F= \frac{dQ}{dt}=\frac{N}{V}Amv_x^2$$
- so, the pressure exerted on the wall is: 
$$p=\frac{F}{A}=\frac{N}{V}mv_x^2$$
- we apply the same argument for $v_{y}$ and $v_z$
- in an isotropic system, $v_x=v_y=v_z$, ie: $v^2=v_x^2+v_y^2+v_z^2$: 
$$p=\frac{1}{3}\frac{N}{V}mv^2$$
- we have assumed that all $m$ molecules have the same speed $v$, however, we will see that the molecules have a distribution of speeds *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C7 - maxwell-boltzmann distribution\|here]]*
- here, we are using $v^2$, so, we will use the average value of $v^{2\implies}\bar{v}^2$ 
$$p= \frac{N}{3V}m \bar{v}^2$$
- multiplying both sides by $V$: 
$$pV=\frac{1}{3}Nm\bar{v}^2=Nk_BT$$
## alternative method
$\Delta p = 2mv_x$
[[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]]: $F= \frac{2mv_{x}}{dt}$
- if length of the cube is $L$, time for a molecule to get from one wall to the other and back:
	$v_{x} = \frac{2L}{dt} \implies dt = \frac{2L}{v_{x}}$
	$\implies F= \frac{m v_{x}^{2}}{L}$
- for $N$ molecules: $\frac{F}{N}= \frac{m \bar v_{x}^{2}}{L}$
$$p=\frac{F}{A} = \frac{\frac{Nm \bar v_{x}^{2}}{L}}{A} = \frac{m\bar v_{x}^{2}}{V}$$
- statistically, $\bar v^{2} = \bar v_{x}^{2} + \bar v_{y}^{2} + \bar v_{z}^{2} = 3 \bar v_{x}^{2}$
$$\implies pV = \frac{1}{3}Nm\bar v^{2}$$
$$\frac{3}{2}pV = N \frac{1}{2}m\bar v^{2} = Nk_{B}T$$
## some consequences
[YF p619]
- we can define temperature:
$$T= \frac{m\bar{v}^{2}}{3k_{B}}$$
	- microscopic definition of temperature
- we can consider kinetic energy:
$$m\bar{v}^{2}=3k_{B}T$$
$$\bar{E}_{K}=\frac{3}{2}k_{B}T$$
	- we have related the average KE of the gas to its temperature