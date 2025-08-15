---
{"dg-publish":true,"permalink":"/content/013/a-small-angle-scattering/a4-structure-factor/","noteIcon":"1","created":"2025-08-15T08:50:20.552+01:00","updated":"2025-08-15T09:12:51.102+01:00"}
---

![A4 - structure factor.png](/img/user/pics/A4%20-%20structure%20factor.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*

- structure factor captures the collective contribution by a large number of particles
$$|a| = \rho V [P(q)]^{1/2}$$
- the phase depends on particle position
- for identical particles:
$$I(q) = \rho^{2} V^{2} P(q) \left| \sum\limits_{i} \exp(i \phi_{i}) \right|^{2} $$
	where, $\phi_{i} =\phi_{\theta}(x,y,z)$ at say its centre of mass
## randomly positioned particles
- considering randomly positioned particles, so the vector orientations are also random, forming a random walk
- $N$ successive steps are made with the same length, $a$ and random directions
- consequently, average walk length is not proportional to $N$, but the average squared length is
$$\langle{|A|^{2}}\rangle = N|a|^{2}$$
$$\therefore I(q) = c \rho^{2} V^{2} P(q)$$
	where, $c$ is the concentration

- $I\propto N$ is typical of incoherent scattering
## aggregated particles
- in most cases, particles aggregate with $n_{a}= 3$
- the trajectories end up being more elongated, and hence larger intensities are obtained
- considering $q \to 0$, $\lambda^{*} \gg$ aggregates
- all particles in an aggregate scatter coherently, so the length of a step is $n_{a}a$
- aggregates scatter incoherently, so a random walk with $N/n_{a}$ steps
$$\langle{|A|^{2}}\rangle \simeq n_{a} N |a|^{2}$$
$$\therefore I(q) = c \rho^{2} V^{2} P(q)\, S(q)$$
	where, $S(q)$ is the structure factor

![A4 - structure factor-1.png](/img/user/pics/A4%20-%20structure%20factor-1.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*
