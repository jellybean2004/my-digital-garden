---
dg-publish: true
---

## scalar triple product
- defined by $[\vec u, \;\vec v, \;\vec w]\equiv\vec u\cdot(\vec v \times \vec w)$
	- the result is a scalar
![Pasted image 20231010174719.png](/img/user/pics/Pasted%20image%2020231010174719.png)
	- scalar triple product is the volume of the parallelepiped defined by $\vec u$, $\vec v$ and $\vec w$
- can be used to determine whether three vectors are linearly independent (lie in the same plane)
	- if $[\vec u, \;\vec v, \;\vec w]=0$, they are linearly independent
- $\vec u \cdot \vec v = \vec v \cdot \vec u$ but $\vec u \times \vec v = -\vec c \times \vec u$
	- so, $\vec u(\vec v \times \vec w) = -(\vec w \times \vec v)\cdot \vec u$
- to check: $\vec u(\vec v \times \vec w) = (\vec u \times \vec v)\cdot \vec w$ 
		- in cartesian coordinates,
		$RHS=(\vec u \times \vec v)\cdot \vec w=(u_yv_z-u_zv_y)w_x+(u_zv_x-u_xv_z)w_y+(u_xv_y-u_yv_x)w_z$
			$=w_xu_yv_z-w_xv_yu_z+v_xw_yv_z-u_xw_yv_z+u_xv_yw_z-v_xu_yw_z$
		$LHS=\vec u \cdot(\vec v \times \vec w)=(v_yw_z-v_zw_y)u_x+(v_zw_x-v_xw_z)u_y+(v_xw_y-v_yw_x)u_z$
			$=w_xu_yv_z-w_xv_yu_z+v_xw_yv_z-u_xw_yv_z+u_xv_yw_z-v_xu_yw_z$
		$\therefore LHS=RHS$
- alt method for computing: 
$$ [u, v, w] = \det
\begin{vmatrix}
u_{x} & u_{y} & u_{z} \\ 
v_{x} & v_{y} & v_{z} \\ 
w_{x} & w_{y} & w_{z} \\
\end{vmatrix}
$$

- to find: volume for the parallelepiped with vertices:
	$A = (1,3,0)$
	$B = (2,1,6)$
	$C = (1,1,3)$
	$D = (0,1,4)$
- find $\vec {AB}, \vec {AC}, \vec {AD}$
- volume = $[\vec {AD}, \vec {AC}, \vec {AB}]$
	- order of vectors doesn't matter, just take the absolute value of the scalar triple product
## vector triple product
- defined as $\vec u \times (\vec v \times \vec w)$ :
$$\vec u \times (\vec v \times \vec w)\neq (\vec u \times \vec v) \times \vec w)$$
$$\vec u \times (\vec v \times \vec w) = (\vec u\cdot \vec w)\vec v - (\vec u .\vec v)\vec w$$
- $\vec v \times \vec w$ gives a vector perpendicular to the plane $\vec v$, $\vec w$ 
	- if you work through the components, the above result can be proved. 
	- eg: if angular velocity $\vec \omega$
		- centripetal acceleration: $\vec a =\vec{\omega}\times (\vec \omega \times \vec r)$