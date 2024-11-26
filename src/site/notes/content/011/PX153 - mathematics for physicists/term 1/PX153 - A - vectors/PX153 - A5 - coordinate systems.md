---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-a-vectors/px-153-a5-coordinate-systems/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:36:19.270+00:00"}
---

- recall [basis vectors]([[content/011/PX153 - mathematics for physicists/term 1/PX153 - A - vectors/PX153 - A1 - notation and geometrical representation\|PX153 - A1 - notation and geometrical representation]])
	- in 3D, a coordinate system can be defined by specifying 3 linearly independent basis vectors at every point in space
	- usually defined to be orthonormal ![Pasted image 20231009145446.png](/img/user/pics/Pasted%20image%2020231009145446.png)
- to find $\underline{\hat e_i}$, several ways
	- eg: tangent to the curve marking the change in coordinate
## cartesian coordinates
[[content/011/PX153 - mathematics for physicists/term 1/PX153 - A - vectors/PX153 - A2 - cartesian coordinates and vector components\|cartesian coordinates]]
## circular polar coordinates
- 2D![Pasted image 20231009145159.png](/img/user/pics/Pasted%20image%2020231009145159.png)
	- here, $r$ is the magnitude of the vector and $\theta$ is the angle made by the vector with the x-axis in counter-clockwise direction such that $0 \leq \theta < 2\pi$ or $\theta \in [0,2\pi)$
- transforming between polar and cartesian coordinates:
	 $x = r \cos{\theta}$
	 $y = r \sin{\theta}$
		 $r=\sqrt{x^2+y^2}$
		 $\theta = \arctan{(\frac{y}{x})}$
- the basis vectors for polar coordinates vary in space, but are always orthonormal
		$\underline{\hat e_{r}}= \cos{\theta}\underline{\hat e_x}+\sin{\theta}\underline{\hat e_y}$
		$\underline{\hat e_{\theta}}= -\sin{\theta}\underline{\hat e_x}+\cos{\theta}\underline{\hat e_y}$
			![Pasted image 20231010181800.png](/img/user/pics/Pasted%20image%2020231010181800.png)
- to check: these are orthonormal
	$\vec e_r \cdot \vec e_\theta=\cos{\theta}(-\sin{\theta})+\sin{\theta}\cos{\theta}=0\implies orthormal$
## cylindrical polar coordinates
{ #04f786}


- 3D
- polar coordinates in x-y plane, extend by keeping the z-axis
	- defined by $(r,\theta,z)$
![Pasted image 20231010182022.png](/img/user/pics/Pasted%20image%2020231010182022.png)
- transformations to/from cartesian:
		$x=r\cos{\theta}$
		$y=r\sin{\theta}$
		$z=z$
			$r=\sqrt{x^2+y^2}$
			$\theta=\arctan{\frac{y}{x}}$
			$z=z$
## spherical polar coordinates
- 3D
	- defined by $(\theta, \phi, r)$
- for problems with spherical symmetry
- ![Pasted image 20231010182043.png](/img/user/pics/Pasted%20image%2020231010182043.png)
		$0\leq r$
		$0\leq \theta \leq \pi$
		$0\leq \phi \leq 2\pi$
- transformations to/from cartesian:
		$x = r\sin{\theta}\cos{\phi}$
		$y=r\sin{\theta}\sin{\phi}$
		$z=r\cos{\theta}$
			$r=\sqrt{x^2+y^2+z^2}$
			$\phi=\arctan{\frac{y}{x}}$
			$\theta=\arccos{(\frac{z}{\sqrt{x^2+y^2+z^2}})}$
		again, $\underline{\hat e_r}$, $\underline{\hat e_\theta}$, $\underline{\hat e_\phi}$ vary in space		