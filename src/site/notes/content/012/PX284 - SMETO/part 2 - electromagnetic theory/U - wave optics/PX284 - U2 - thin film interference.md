---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/u-wave-optics/px-284-u2-thin-film-interference/","noteIcon":"1","created":"2025-05-09T14:38:34.286+01:00","updated":"2025-05-15T14:11:22.314+01:00"}
---

![PX284 - U2 - thin film interference.png|500](/img/user/pics/PX284%20-%20U2%20-%20thin%20film%20interference.png)

- considering '**weak reflections**', ie. light is mostly transmitted
- the reflected rays need to add coherently
- therefore, considering only two reflections
- at normal incidence: 
$$\begin{gather}
r_{12} = \frac{n_{1}-n_{2}}{n_{1}+n_{2}} \\
r_{23} = \frac{n_{2}-n_{3}}{n_{2}+n_{3}}
\end{gather}$$
- total reflection coefficient (coherent sum):
$$r = r_{12} + r_{23}  \exp(i2dk_{2})$$

	where, $k_{2}$ is the wavenumber in material 2

- using a '**quarter-wave**' coating: $d = \lambda_{2}/4$, so that $\exp(2dk_{2}) = -1$
$$\therefore r = r_{12}- r_{23}$$
- typical anti-reflective coating:
$$n_{2} < n_{2}< n_{3}$$
- considering air: $n_{1}\sim 1$, glass: $n_{3}\sim 1.5$ ;  $r=0$ if $r_{12} = r_{23} \implies n_{2}^{2}= n_{1}n_{3}$
- often used material is MgF$_2$ with $n \simeq 1.38$
- this reduces reflection losses $(\propto |r|^{2})$, typically from $\sim 4\%$ to $\sim 1\%$, depending on $\lambda$

## dielectric mirror
- for dielectric mirrors $(n_{1} < n_{3} < n_{2})$ $\implies r_{12} <0 (n_{2} < n_{2})$ and $r_{23}> 0 (n_{2}> n_{3})$
$$r = r_{12} + r_{23} \exp(i2k_{2}d)$$
- for ${} d = \lambda_{2}/4: {}$ $r_{12} - r_{23}$
- ie. add constructively due to opposite signs
- eg: TiO$_2$ $n_2 \sim 2.6$ used to increase reflectance of glass from $4\%$ to $\sim40\%$ for one layer of coating or even lighter for multiple layers
## soap films
- soap (surfactant) stabilises surface, but does not affect optics
- a layer of water $n_{2} = 1.33$ between air $n_{1}=n_{3} =1$
$$\begin{gather}
r_{12} = - 0.14 \\
r_{23} = +0.14 \\
r = r_{12}  + r_{23} \exp(i2k_{2}d) = -0.14 (1+\exp(i2k_{2}d))
\end{gather}$$
- soap film under gravity:
	- top: $d$ small, $\exp(i2kd \simeq 1)$ $\implies r\simeq 0$ ie. transparent
	- middle: $\exp(i2kd) \neq 1 \forall \lambda$ $\implies$ all visible light reflected
	- bottom: $\exp(i2kd) =1$ for some wavelengths, other wavelengths reflected $\implies$ colors in bands
- basically, gravity causes $d$ to increase

## angle dependence
![PX284 - U2 - thin film interference-2.png|500](/img/user/pics/PX284%20-%20U2%20-%20thin%20film%20interference-2.png)

- phase difference between $ABC$ and $AD =$ difference in distance $\times$ wavelength:
$$\begin{gather}
ABC = \frac{2d}{\cos t} \\
AD = 2x\sin i = 3d \frac{\sin t}{\cos t} \sin i\\
\Delta \phi = \frac{2d}{\cos t} (k_{2}-k_{1}\sin t \sin i)\\
= \frac{2dk_{2}}{\cos t} ( 1-\sin ^{2}t) = 2dk_{2}\cos t	
\end{gather}$$
	where, $k_{1}\sin i = k_{2}\sin t$ (snell's law)
- destructive interference when $2dk_{2}\cos t = \pi$
$$\lambda_{2} = \frac{\lambda_{0}}{n_{2}} = 4d\cos t$$
