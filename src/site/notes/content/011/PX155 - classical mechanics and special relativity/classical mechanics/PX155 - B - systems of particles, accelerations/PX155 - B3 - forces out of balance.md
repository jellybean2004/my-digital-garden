---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-b-systems-of-particles-accelerations/px-155-b3-forces-out-of-balance/","created":"2024-10-01T18:27:09.495+01:00","updated":"2024-11-26T19:55:13.252+00:00"}
---

- [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A6 - block on a slope\|PX155 - A6 - block on a slope]]
	- but now, the block is sliding $\to$ friction is kinetic ![Pasted image 20231016160749.png](/img/user/pics/Pasted%20image%2020231016160749.png)
		- $a$ is not a force, so indicated by a double header arrow
	- by [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]]
		- parallel to the slope: $W\sin{\theta}-F_k=ma$
		- perpendicular the the slope: $W\cos{\theta}=0$
			where, $W=mg$ ; $N=mg\cos{\theta}$
				$F_{k}=\mu_kN=\mu_kmg\cos{\theta}$
			$ma=mg\sin{\theta}-\mu_kmg\cos{\theta}$
			$a=g\sin{\theta}-\mu_kg\cos{\theta}=g(\sin{\theta}-\mu_k\cos{\theta})$
				 $a$ is constant
- eg:  reconsider the block on a slope, but now, the slope is to the upper surface of a wedge and the wedge is resting on a table and there is no friction. to find: accelerations of the block and the wedge
	- draw two diagrams, one for each body![Pasted image 20231016160802.png](/img/user/pics/Pasted%20image%2020231016160802.png)
	- $\vec a_1$ is not the actual acceleration of the block (relative to the table), it is the acceleration relative to the wedge, which doesn't define the initial reference frame
	- we need to apply [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]] in the frame defined by the fixed reference
$$\vec a_{B}=\vec a_1 +\vec a_2$$
	- for wedge, horizontally:
$$N\sin\theta = m_{W}a_2$$
	- for block, perpendicular to the slope:
$$N-m_{B}g\cos\theta = -m_{B}a_{2}\sin\theta$$
	- combining above equations:
$$\begin{align*}
			m(g\cos\theta-a_{2}\sin\theta) \sin\theta = m_{W}a_{2} \\
			a_{2} = \frac{m_{B}g\cos\theta\sin\theta}{m_{W}+m_{B}\sin^{2}\theta}
		\end{align*}$$
	- for block, parallel to the slope:
$$mg\sin\theta = m(a_{1}-a_{2}\cos\theta)$$
	- combining equations above:
$$a_{1}= g\sin\theta + \frac{m_{B}g\cos^{2}\theta\sin\theta}{m_{W}+m_{B}\sin^{2}\theta}$$
