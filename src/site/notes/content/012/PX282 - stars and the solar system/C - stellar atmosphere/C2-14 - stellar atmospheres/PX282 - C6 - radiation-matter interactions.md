---
dg-publish: true
---

- consider light with an intensity, $I_\lambda$ passing through a material of thickness, $dz$
- the emergent light will have a new intensity, $I_{\lambda}'$
## absorption
- the change in specific intensity with respect to the depth due to absorption: 
$$\frac{dI_{\lambda}}{dz} = - \kappa_{\lambda} \,\rho \, I_{\lambda}$$
	where, $\rho=$ density, and $\kappa_\lambda=$ the absorption coefficient/opacity
## scattering
- the change in specific intensity with respect to the depth due to scattering: 
$$\frac{dI_{\lambda}}{dz} = - \sigma_{\lambda}\, \rho\, I_{\lambda}$$
	where, $\sigma_{\lambda} =$ scattering coefficient, sometimes included in $\kappa$
## emission
- the change in specific intensity with respect to the depth due to emission: 
$$\frac{dI_\lambda}{dz} = \epsilon_\lambda\,\rho$$
	where, $\epsilon_{\lambda}=$ emission coefficient
## only absoprtion
$$\frac{dI_{\lambda}}{dz} = - \kappa_{\lambda} \,\rho \, I_{\lambda}$$
- if $I_{\lambda}(z=0)= I_{\lambda,0}$, what is $I_{\lambda}(z)$?
$$\begin{align*}
	\int_{I_{\lambda0}}^{I_{\lambda}(z)} \frac{1}{I_{\lambda}} dI_{\lambda} &= \int_{0}^{z} - \kappa_{\lambda} \,\rho \, \,dz \\
	[\ln I_{\lambda}]_{I_{\lambda0}}^{I_{\lambda}(z)} &= \int_{0}^{z} - \kappa_{\lambda} \,\rho \, dz \\
	\frac{I_{\lambda}}{I_{\lambda,0}} &= \exp\left(\int_{0}^{z} - \kappa_{\lambda} \,\rho \,dz\right)	
\end{align*}$$
- if $\kappa_{\lambda}\rho$ is assumed constant: 
$$\frac{I_{\lambda}}{I_{\lambda,0}} = \exp(-\kappa_{\lambda} \,\rho \,z)$$
