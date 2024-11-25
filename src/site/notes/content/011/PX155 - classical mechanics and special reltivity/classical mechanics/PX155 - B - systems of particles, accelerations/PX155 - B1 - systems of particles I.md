---
dg-publish: true
---
- consider an object/body as $N$ particles at positions $\vec r_i$ relative to some origin $O$
![Pasted image 20231010183545.png](/img/user/pics/Pasted%20image%2020231010183545.png)
- force on particle $j$ due to particle $i$ is $\vec F_{ij}$
- external force on particle $i$ is $\vec F_i$
- total force on one of the particles $i:$
$$\vec F_{i} + \sum\limits_{j\neq i}^{N}{\vec F_{ji}} = m_{i} \vec a_{i}$$
- sum over all particles:$$\sum_i^N{\vec F_i}+\sum_i^N{\sum\limits_{j\neq i}^{N}{\vec F_{ji}}}=\sum\limits_i^N{m_i \vec a_i}$$
- 2nd term = 0 : for every $\vec F_{ji}$ there is an equal and opposite $\vec F_{ij}$ 
	$\vec F_{ji}=-\vec F_{ij}$ by [[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A3 - newton's third law\|PX155 - A3 - newton's third law]]
	$\vec F = \sum\limits_i^Nm_i \vec a_i$
	$\vec F = (\sum\limits_i^N m_i)\frac{\sum\limits_i^Nm_i \vec a_i}{\sum\limits_i^N m_i}=(M)\frac{\sum\limits_i^Nm_i \vec a_i}{M}$
	$\vec F =M(\frac{\sum\limits_i^Nm_i \frac{d^2\vec r_i}{dt^2}}{M})$
	$\vec F =M(\frac{\frac{d^2}{dt^2}\sum\limits_i^Nm_i \vec r_i}{M})$
	$\vec F =M\frac{d^2}{dt^2}\vec r_{cm}$
		where, $\vec r_{cm}=$ centre of mass
	$$\vec F =M\vec a_{cm}$$
- [[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]] holds provided all points on the body accelerate at $\vec a_{cm}$ or if we only care about $\vec a_{cm}$