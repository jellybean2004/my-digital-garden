---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/c-stellar-atmosphere/c5-8-stellar-atmospheres/px-282-c6b-intensity-after-absorption/","noteIcon":"1","created":"2024-12-22T10:26:10.909+00:00","updated":"2024-12-22T10:27:12.617+00:00"}
---

the [[content/012/PX282A - stars/C - stellar atmosphere/C5-8 - stellar atmospheres/PX282 - C6a - radiation-matter interactions#absorption\|absorption equation]]: 
$$\frac{dI_{\lambda}}{dz} = - \kappa_{\lambda} \,\rho \, I_{\lambda}$$
- supposing $I_{\lambda}(z=0)= I_{\lambda,0}:$
$$\begin{align*}
	\int_{I_{\lambda0}}^{I_{\lambda}(z)} \frac{1}{I_{\lambda}} dI_{\lambda} &= \int_{0}^{z} - \kappa_{\lambda} \,\rho \, \,dz \\
	\big[\ln I_{\lambda}\big]_{I_{\lambda,0}}^{I_{\lambda}(z)} &= \int_{0}^{z} - \kappa_{\lambda} \,\rho \, dz \\
	\frac{I_{\lambda}}{I_{\lambda,0}} &= \exp\left(\int_{0}^{z} - \kappa_{\lambda} \,\rho \,dz\right)	
\end{align*}$$
- if $\kappa_{\lambda}\rho$ is assumed constant: 
$$\therefore I_{\lambda}(z) = I_{\lambda,0}\exp(-\kappa_{\lambda} \,\rho \,z)$$
