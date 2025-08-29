---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-2-solar-system/i-planetary-motion/px-282-i6a-three-body-problem-i/","noteIcon":"1","created":"2025-08-27T13:15:22.840+01:00","updated":"2025-01-24T11:28:16.000+00:00"}
---

- considering the motion of three bodies
- generally, there is no analytical solution, and it is chaotic

![PX282 - I6 - three body problem.png|500](/img/user/pics/PX282%20-%20I6%20-%20three%20body%20problem.png)
*image: Wolfram Alpha*

- there are exceptions, such as the **restricted three body problem**, where the mass of third object is negligible

![PX282 - I6 - three body problem-1.png|500](/img/user/pics/PX282%20-%20I6%20-%20three%20body%20problem-1.png)
*image: Murray & McDermott, Solar System Dynamics (1999)*

![PX282 - I6 - three body problem-2.png|500](/img/user/pics/PX282%20-%20I6%20-%20three%20body%20problem-2.png)
*image: Carroll & Ostile, An Introduction to Modern Astrophysics (2007)*

- stable orbits in ***roche potential*** at ***lagrangian points*** where the gravitational potential is locally flat (in rotating frame)
- eg: $L_1$ and $L_{2}$ in earth-sun system is often used for space telescopes

![PX282 - I6 - three body problem-3.png|500](/img/user/pics/PX282%20-%20I6%20-%20three%20body%20problem-3.png)
*image: Murray & McDermott, Solar System Dynamics (1999)*

- **tadpole** and **horseshoe** orbits vibrate around the  $L_{4}$ and $L_5$ points
- eg: trojan asteroids in jupiter-sun system

- approximate sphere of influence around the second body where orbits can be stable, called the **hill sphere***
- moons must be well within the hill sphere 

- considering a test particle at $L1$ point, so the distance between $M_{2}$ and the particle is the radius of the hill sphere, $R_H$, and the distance between ${} M_{1}$ and $M_{2}$ is $a$

$$\begin{gather}
\underbrace{\frac{GM_{2}}{R_{H}^{2}} - \frac{GM_{1}}{(a-R_{H})^{2}}}_\text{gravitational acceleration} + \underbrace{\Omega^{2} (a-R_{H})}_\text{centrifugal acceleration} = 0
\end{gather}$$
- using [[content/012/PX282 - stars and solar system/term 2 - solar system/I - planetary motion/PX282 - I2 - kepler's laws\|kepler's third law]], with $M_{1} \gg M_{2}:$
$$\Omega^{2} = \left(\frac{2\pi}{P}\right)^{2} = \frac{Gm_{1}}{a^{3}}$$
- since $R_{H} \ll a$, using binomial expansion:
$$(a - R_{H})^{-2} = a^{-2} \left(1- \frac{R_{H}}{a}\right)^{-2} \approx a^{-2} \left(1+ 2 \frac{R_{H}}{a}\right)$$
$$\begin{gather}
\frac{GM_{2}}{R_{H}^{2}} - \frac{GM_{1}}{a^{2}} \left(1 + 2 \frac{R_{H}}{a}\right) + \frac{GM_{1}}{a^{2}}\left(1- \frac{R_{H}}{a}\right) \approx 0 \\
\frac{M_{2}}{R_{H}^{2}} - \frac{M_{1}}{a^{2}} \left(3 \frac{R_{H}}{a}\right) \approx 0 \\
\therefore R_{H }\approx \left(\frac{M_{2}}{3M_{1}}\right)^{1/3}a
\end{gather}$$

