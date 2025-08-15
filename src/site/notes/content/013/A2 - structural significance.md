---
{"dg-publish":true,"permalink":"/content/013/a2-structural-significance/","noteIcon":"1","created":"2025-08-15T07:29:02.509+01:00","updated":"2025-08-15T09:12:30.661+01:00"}
---

- intensities are plotted against the scattering wavevector, $q:$
$$q = \frac{4\pi}{\lambda} \sin\left(\frac{\theta}{2}\right)$$
	where, $\lambda$ is the wavelength of x-rays/neutrons, and $\theta$ is the scattering angle
- physically, $\Delta p = \hbar q$ is the momentum transfer after the scattering
- plotting patterns against $q$ makes it $\lambda$-independent, which would not be the case for plot against $\theta$

![A2 - structural significance.png](/img/user/pics/A2%20-%20structural%20significance.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*

- scattering peaks can be interpreted in terms of diffraction by the periodic pore structure in the nm scale
- many materials do not exhibit periodicity, hence their SAS patterns do not exhibit any sharp peaks

- linear sales have featureless plots
- logarithmic scales reveal a plateau at small $q$ followed by an oscillatory decrease 

- bragg's law is concerned with diffraction very specific to scattering from periodic structures
$$2d\sin\left(\frac{\theta_{d}}{2}\right) = n\lambda $$
	where, $d$ is the periodicity of structure, $\theta_d$ is the diffraction angle, and $n\in\mathbb{Z}>0$
- this is not a general law, but a consequence of the general principles particularised to spatially periodic structures

- assumptions:
	- the emission of secondary waves are isotropic
	- they reach the detector without being scattered twice

- only the unperturbed incoming waves are responsible for secondary waves
- the phase, $\phi$, of a secondary wave reaching the detector is solely the function of the position of the scattering centre, $(x,y,z)$
- for any given angle, a characteristic phase map can be calculated, $\phi_\theta(x,y,z)$
- the intensity can be obtained by comparing $\phi_\theta$ with the actual spatial distribution of electrons/nuclei in the sample

![A2 - structural significance-1.png](/img/user/pics/A2%20-%20structural%20significance-1.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*

- the phase map is obtained by:
$$\phi_{\theta}= \frac{2\pi L}{\lambda}$$
- it takes constant values on geometric planes oriented at an angle of $\theta/2$ wrt the incident beam
$$\phi_{\theta}(x,y,z) = \phi_{0} + qy$$
- it increases by $2\pi$ over $\lambda^{*} = 2\pi/q$
- for SAS< $\sin(\theta/2) \simeq \theta/2$, so $\lambda^{*} \simeq \lambda/\theta$
