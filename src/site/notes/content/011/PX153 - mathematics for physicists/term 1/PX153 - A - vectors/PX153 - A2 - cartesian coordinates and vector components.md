---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-a-vectors/px-153-a2-cartesian-coordinates-and-vector-components/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:34:26.931+00:00"}
---

## basis vectors

![Pasted image 20231003190709.png](/img/user/pics/Pasted%20image%2020231003190709.png)
- 3 vectors that are linearly independent (don't lie in the same plane $\alpha \underline{e_{1}} +  \beta \underline{e_{2}} + \gamma\underline{e_{3}} \neq 0$ for non-zero $\alpha, \; \beta, \; \gamma$)
	- then $\underline{a} = a_{1}\underline{e_{1}}+  a_{2}\underline{e_{2}}+  a_{3}\underline{e_3}$
	- $\underline{e_{1}}, \underline{e_{2}}, \underline{e_{3}}$ form a basis
	- $a_1, a_2, a_3$ are the components of $\underline a$ in that basis
- normally *orthonormal* basis vectors are chosen
	- *orthonormal* = perpendicular vectors with length one
	- eg: cartesian coordiantes: $\underline{ \hat e_x},\underline{ \hat e_y},\underline{ \hat e_z}$
$$\vec v = (\underline{ \hat v_x},\underline{ \hat v_y},\underline{ \hat v_{z})}= v_{x}\underline{ \hat e_{x}}+ v_{2}\underline{ \hat e_{y}}+ v_{3}\underline{ \hat e_{z}} = \sum\limits_{i=x,y,z} v_{i} \underline{ \hat e_i}$$
$$|v|=\sqrt{{v_x}^2+{v_y}^2+{v_z}^2}$$
the direction of $\vec v$
$$\underline{\hat v} = \frac{v_{x}}{|\vec v|}\underline{ \hat e_{x}}+ \frac{v_{y}}{|\vec v|}\underline{ \hat e_{y}}+ \frac{v_{z}}{|\vec v|}\underline{ \hat e_z}$$
- the value of each component of $\underline v$, is the projection of $\underline v$ along the appropriate basis vector
## direction cosines
![Pasted image 20231003163533.png](/img/user/pics/Pasted%20image%2020231003163533.png)
- we can define the direction cosines of $\underline v$ which relate to the components of $\vec v$ to the angle of $\vec v$ relative to the cartesian basis vectors from the diagram
$$cos{\alpha} = \frac{v_x}{|\vec v|}, \; cos{\beta} = \frac{v_y}{|\vec v|}, \; cos{\gamma} = \frac{v_z}{|\vec v|}$$
- cartesian coordinates -> basis vectors are fixed in direction everywhere in space
	- this is not true for polar coordinates
![Pasted image 20231003163604.png](/img/user/pics/Pasted%20image%2020231003163604.png)
- for most of the time, right-handed cartesian coordinates will be used
![Pasted image 20231003191717.png](/img/user/pics/Pasted%20image%2020231003191717.png)
