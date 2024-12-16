---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-c-magnetic-fields/px-157-c2-force-of-current-loops/","noteIcon":"1","created":"2024-10-01T18:27:10.180+01:00","updated":"2024-11-26T20:09:23.952+00:00"}
---

## force on a wire
![Pasted image 20240218165423.png](/img/user/pics/Pasted%20image%2020240218165423.png)
- the force on one moving charge:
$$
\vec F = q\,\vec v_{d}\times \vec B
$$
$$
\vec v_{d} \parallel d\vec l \implies \vec v_{d}\cdot d\vec l = v_{d}d\vec l
$$
- number density of charges (current carriers): $n$
- volume of section of wire: $A\,dl$
- [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/III - properties/PX157 - B13a - current#drift velocity\|drift velocity]]: $I=n\,q\,v_{d}\,A$
- total force on section, $dl:$
$$\begin{align*}
	d\vec F &= n\,A\,dl\,q\,\vec v_{d}\times \vec B \\
	&= n\,A\,q\,v_{d}\,d\vec l \times \vec B \\
	\therefore d\vec F &= I\,d\vec l \times \vec B
\end{align*}$$
- for the whole wire:
$$
\vec F = \int I\,d\vec l\times\vec B
$$
## force on a moveable bar
![Pasted image 20240218165455.png](/img/user/pics/Pasted%20image%2020240218165455.png)
- extended magnetic field: $\vec B = B\,\hat z$
- crossbar section: $d\vec l = dl\,\hat y$
- force on section:
$$\begin{align*}
		d\vec F &= I\,d\vec l \times \vec B \\
		&= I\,dl\,B\,\hat y \times \hat z \\
		&= I\,dl\,B\,\hat x
	\end{align*}$$
- total force:
$$
\vec F = \int I\,dl\,B\, \hat x = I\,L\,B\,\hat x
$$
## force and torque on a current loop
![Pasted image 20240218165508.png](/img/user/pics/Pasted%20image%2020240218165508.png)
- forces on each of the sides:
	$\vec F_{12} \sim \hat z$
	
	$\vec F_{34} \sim -\hat z$, $\vec F_{34} = -\vec F_{12}$
	
	$d\vec F_{23} = -I\,d\vec l \times \vec B = -I\,dl\, B\, \hat y$, with $d\vec l = dl\,\hat z$
		$\vec F_{23} = \int -I\,B\,dl\,\hat y = -I\,B\,a\,\hat y$
	
	$d\vec F_{41} = +I\,d\vec l \times \vec B = I\,dl\, B\, \hat y$, with $d\vec l = dl\,\hat z$
		$\vec F_{41} = \int I\,B\,dl\,\hat y = I\,B\,a\,\hat y$
- total force:
$$
\vec F = \sum\limits\vec F_{mn} =  0
$$
![Pasted image 20240218165530.png](/img/user/pics/Pasted%20image%2020240218165530.png)
- torque on each section:
$$
d\vec\tau = \vec r \times d\vec F_{41}+(-\vec r)\times d\vec F_{23}
$$
- also, $|\vec r| = \frac{b}{2}$, $d\vec d_{41}= -d\vec F_{23}:$
$$\begin{align*}
	d\vec\tau &= \vec r \times d\vec F_{41} - \vec r \times (-d\vec F_{41}) \\
	&= 2\vec r\times d\vec F_{41} \\
	&= 2 \frac{b}{2}d\hat r\times I\,B\,dl\,\hat y \\
	&= dl\,b\,I\,B\,\hat r\times\hat y \\
	d\vec\tau &= dl\,b\,I\,B\,\hat n\times\hat x
\end{align*}$$
- **total torque**:
$$
\vec\tau = \int dl\,b\,I\,B\,\hat n\times\hat x = a\,b\,I\,B\,\hat n\times\hat x
$$
$$
\vec\tau = \vec\mu \times\vec B\;;\; \vec\mu = I\,A\,\hat n\;;\; A=a\,b
$$
	where, $\vec\mu=$ magnetic dipole moment, units: $C\,m^{2}\,s^{-1}$
- for $N$ windings, $\vec\mu = N\,I\,A\,\hat n$
- **potential energy**:
$$
U = -\vec\mu \cdot\vec B
$$
