---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-a-vectors/px-153-a4-vector-operations/","noteIcon":"1","created":"2025-08-27T13:14:08.654+01:00","updated":"2024-11-26T23:12:55.000+00:00"}
---

## addition and subtraction
$$\vec u \pm \vec v = (u_x\pm v_x,\; u_y\pm v_y,\; u_z\pm v_z)$$
- properties
	- commutative - $\vec u \pm \vec v =\vec v \pm \vec u$
	- associative - $\vec u \pm (\vec v \pm \vec w) = (\vec v \pm \vec u) \pm \vec w$
![Pasted image 20231004173735.png](/img/user/pics/Pasted%20image%2020231004173735.png)
![Pasted image 20231004173841.png](/img/user/pics/Pasted%20image%2020231004173841.png)
## vector products
### scalar/dot product
- $s =\vec u \cdot \vec v$
	- $s$ is a scalar
- geometrically, it is the magnitude of one vector projected on the other 
$$s = \vec u \cdot \vec v = |\vec u||\vec v| \cos{\theta}$$
	- $\theta =$ angle between the vectors
- if $\theta = \frac{\pi}{2}$ (orthogonal vectors), $s=0$
- for cartesian coordinate basis vectors 
$$\underline{\hat i}\cdot \underline{\hat i}=\underline{\hat j}\cdot \underline{\hat j}=\underline{\hat k}\cdot \underline{\hat k}=1$$
	and
	$$\underline{\hat i}\cdot \underline{\hat j}=\underline{\hat j}\cdot \underline{\hat k}=\underline{\hat k}\cdot \underline{\hat i}=0$$
	- this denotes that the basis vectors are orthonormal
- properties
	- commutative - $\vec u \cdot \vec v = \vec v \cdot \vec u$
	- distributive - $\vec u \cdot (\vec v + \vec w) = \vec v \cdot (\vec u + \vec w)$
- in cartesian coordinates - $s = \vec u \cdot \vec v = u_xv_x+u_yv_y+u_zv_z$
- using both definitions:
	$$\cos{\theta} = \frac{\vec u \cdot \vec v}{|u||v|}$$
	- component of $\vec u$ along $\vec v$ $= \vec u_v=(\frac{\vec u \cdot \vec v}{v^2})\vec v=(\frac{\vec u \cdot \vec v}{v})\underline{\hat v}$
- eg of scalar product in physics:
	$$W = \vec F \cdot \vec d$$
### vector/cross product

- $\vec v = \vec u \times \vec w$
	- $\vec v$ is a vector
- geometrically, $\vec u$ and $\vec w$ define a parallelepiped of area $uw\sin{\theta}$
![Pasted image 20231004203051.png](/img/user/pics/Pasted%20image%2020231004203051.png)
- $\vec v$ is a vector perpendicular to the plane of $\vec u$ and $\vec w$
	- magnitude $uw\sin{\theta}$ 
	- direction is set by the right-hand rule $$\vec v = uw\sin{\theta}\underline{\hat e}_v$$
	- $\vec v$ is the same independent of the coordinate system, its component in a given basis changes
- cases
	- if $\vec u$ and $\vec w$ are parallel, $\theta = 0$ and $\vec u \times \vec w = 0$
	- if $\vec u$ and $\vec w$ are not parallel, $\vec u \cdot(\vec u \times \vec w) = 0$
- for cartesian coordinates,
	- $\underline{\hat i}\times \underline{\hat i}=\underline{\hat j}\times \underline{\hat j}=\underline{\hat k}\times \underline{\hat k}=0$
	- $\underline{\hat i}\times \underline{\hat j}= \underline{\hat k}$    ,     $\underline{\hat j}\times \underline{\hat k}= \underline{\hat i}$    ,     $\underline{\hat k}\times \underline{\hat i}= \underline{\hat j}$
- properties:
	- vector product is NOT commutative, ie: $\underline{\hat i}\times \underline{\hat j} \neq \underline{\hat j} \times \underline{\hat i}$
	- it is anti-commutative, ie: $\underline{\hat j} \times \underline{\hat i}=-\underline{\hat k}$
- calculating cross product:$$\vec v = \vec u \times \vec w = (u_yw_z-u_zw_y)\underline{\hat i}+(\vec u_zw_x-u_xw_z)\underline{\hat j}+(\vec u_xw_y-u_yw_x)\underline{\hat k}$$
	- easy tip:
![Pasted image 20231009190120.png](/img/user/pics/Pasted%20image%2020231009190120.png)or,
![Pasted image 20231009190210.png](/img/user/pics/Pasted%20image%2020231009190210.png)
![Pasted image 20231009190249.png](/img/user/pics/Pasted%20image%2020231009190249.png)

- many physical quantities are defined by cross product
		- eg: $\vec L = \vec r \times (m \vec v)$, angular momemtum
- eg of cross product calculation
  