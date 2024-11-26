---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-the-solar-system/a-introduction/px-282-a8-solid-angle/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T09:33:53.325+00:00"}
---

- a solid angle gives the area of a 'spherical cap' on the surface
- it is the 3D equivalent of an angle
- units: steradians, radians
![Pasted image 20241017113641.png](/img/user/pics/Pasted%20image%2020241017113641.png)
- how many total solid angles in a sphere? ie: 
$$\int_{sphere} d\Omega =?$$
- taking a unit sphere of surface area, $dA$, for a given solid angle, $d\Omega$
- for spherical coordinates, $dA = \sin\theta\,d\theta\,d\Omega:$ 
$$\int_{0}^{2\pi} \int_{0}^{\pi} \sin\theta \,d\theta \, d\phi = 4\pi$$
- at $\theta=0$, there is not surface contribution

- the angle between two lines is always the same
- similar y, the solid angle enclosed does not change 
- eg: a beam (of $\gamma$, neutrinos) is emitted into solid angle, $\Omega$, it will diffuse with distance, but $\Omega$ does not change

- eg: a torch emits at a ring radius, $r$, at a distance, $d$. what is the solid angle?
	- the surface area of the ring of light is : $\pi r^{2}$ 
	- total area of the possible sphere is: $4\pi d^{2}$ ($d$ is the radius of the sphere containing the ring of light)
	- therefore, the solid angle is: 
	$$\Omega = \frac{\pi r^{2}}{4\pi d^{2}}\times 4\pi = \frac{\pi r^{2}}{d^{2}}$$
- more generally: 
$$\Omega = \frac{A}{d^{2}}$$
- eg in reverse: a beam of particles is released from a collider into a solid angle, $\Omega$, at a rate, $n\,s^{-1}$. how many particles hit a detector at a distance, $d$?
	- beam fills a fraction of the sphere, $\frac{\Omega}{4\pi}$, at any $d$
	- the detector also covers a fraction of the sphere, an area, $A$
	- if $A>\frac{\Omega}{4\pi}\times 4\pi d^{2}$, all particles are received
	- if $A<\frac{\Omega}{4\pi}\times 4\pi d^{2}$, the particle density is: $\frac{n}{\frac{\Omega}{4\pi}\times 4\pi d^{2}}= \frac{n}{\Omega d^{2}}$
	- rate at detector = $\frac{nA}{\Omega d^{2} }$