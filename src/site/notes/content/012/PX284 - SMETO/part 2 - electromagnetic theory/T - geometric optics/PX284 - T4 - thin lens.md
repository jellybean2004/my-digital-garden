---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/t-geometric-optics/px-284-t4-thin-lens/","noteIcon":"1","created":"2025-05-03T12:24:15.897+01:00","updated":"2025-05-22T07:49:37.837+01:00"}
---


![PX284 - T3d - spherical lens.png|500](/img/user/pics/PX284%20-%20T3d%20-%20spherical%20lens.png)

- for light travelling left-to-right:
	- $u>0 \implies$ object to the left of the surface
	- $v>0 \implies$ image to the right of the surface

- now combining the two sides of a spherical lens, such that the image of the first (left) lens becomes the object for the second (right) lens

![PX284 - T3d - thin lens.png|500](/img/user/pics/PX284%20-%20T3d%20-%20thin%20lens.png)

- left lens:
	- object distance: $u$
	- image distance: $v'$
- right lens:
	- object distance: $u' = -v'$
	- image distance: $v$

- let the outside medium be air ($n_1=1$) and lens be glass ${} n_{2}= n {}$
$$\begin{gather}
\frac{1}{u} + \frac{n}{v'} = \frac{n-1}{R_{1}} \\
\frac{n}{-v'} + \frac{1}{v} = -\frac{n-1}{R_{2}} \\
\implies \frac{1}{u}+ \frac{1}{v} = (n-1) \left(\frac{1}{R_{1}} - \frac{1}{R_{2}}\right)
\end{gather}$$
- for light from infinity, $u \to \infty$, the light converges at the focus of the lens, at focal length $v = f$
$$\frac{1}{f} = (n-1) \left(\frac{1}{R_{1}} - \frac{1}{R_{2}}\right)$$
- this is called the **lens maker's equation**
- if the focal length is known, the **thin lens equation**, which neglects the offset between the two surfaces:
$$\frac{1}{u} + \frac{1}{v} = \frac{1}{f}$$
- $1/f$ is called the '**power**' of the lens, measured in units of 'dioptres' $[\text{m}^{-1}]$
