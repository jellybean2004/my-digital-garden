---
dg-publish: true
---
## the law
![Pasted image 20240218165600.png](/img/user/pics/Pasted%20image%2020240218165600.png)
$$
\vec B(\vec r, t) = \frac{\mu_{0}}{4\pi}q \frac{\vec v(t) \times (\vec r-\vec r'(t))}{|\vec r-\vec r'(t)|^{3}}
$$
	where,
		$\vec r =$ position where $\vec B$ is measured
		$\vec r'(t)=$ position of the source, charge that is moving
		$\mu_{0}=$ *permeability of vacuum* $=4\pi \times10^{-7}\,H\,m^{-1}$ ($H=henry=kg\,m^{2}\,c^{-2}$)
- law is valid for *magnetostatics*: particle acceleration would give rise to extra terms and radiation
## forces from two moving charges
![Pasted image 20240218165614.png](/img/user/pics/Pasted%20image%2020240218165614.png)
- two charges, $q$, moving along parallel paths separated by a distance, $\vec r = r\,\hat y$, at velocities, $\vec v_{1}$ and $\vec v_{2}$, such that $\vec v_{1}=\vec v_{2} = v\,\hat x$
- from [[content/011/PX157 - electricity and magnetism/PX157 - A - coulomb's law/PX157 - A2 - coulomb's law\|coulomb's law]]:
	- electrostatic force felt by charge 1 due to charge 2:
$$
\vec F_{E,\,21} = \frac{q^{2}}{4\pi\epsilon_{0}r^{2}} \hat y
$$
	- electrostatic force felt by charge 2 due to charge 1:
$$
\vec F_{E,\,12} = -\frac{q^{2}}{4\pi\epsilon_{0}r^{2}} \hat y
$$
- from [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C3a - the biot-savart law\|the biot-savart law]] :
	- magnetic field felt by charge 1 due to charge 2:
$$
\vec B_{2}(at\;1) = \frac{\mu_{0}}{4\pi} q \frac{\vec v_{2}\times \vec r}{r^{3}}  = \frac{\mu_{0}\,q\,v}{4\pi\epsilon_{0}r^{2}}\hat z
$$
	- magnetic field felt by charge 1 due to charge 2:
$$
\vec B_{1}(at\;2) = \frac{\mu_{0}}{4\pi} q \frac{\vec v_{2}\times (-\hat r)}{r^{3}}  = -\frac{\mu_{0}\,q\,v}{4\pi r^{2}}\hat z
$$
- [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C1a - the lorentz force\|the lorentz force]]:
	- force felt by charge 1 moving in the magnetic field of charge 2:
$$
\vec F_{B,\,21} = q\,\vec v_{1}\times \vec B_{2}(at\;1) = - \frac{\mu_{0}q^{2}v^{2}}{4\pi r^{2}}\hat y
$$
	- force felt by charge 2 moving in the magnetic field of charge 1:
$$
\vec F_{B,\,12} = q\,\vec v_{2}\times \vec B_{1}(at\;2) =  \frac{\mu_{0}q^{2}v^{2}}{4\pi r^{2}}\hat y
$$
- comparing the magnitudes of the two forces:
$$
\frac{|\vec F_{B}|}{|\vec F_{E}|} = \mu_{0}\epsilon_{0}v^{2}
$$
- the speed of light can be defined as:
$$
c = \frac{1}{\sqrt{\mu_{0}\epsilon_{0}}}
$$
$$
\frac{|\vec F_{B}|}{|\vec F_{E}|} = \left(\frac{v}{c}\right)^{2}
$$
- for charges with $v<<c: \vec F_{E}>>\vec F_{B}$ 