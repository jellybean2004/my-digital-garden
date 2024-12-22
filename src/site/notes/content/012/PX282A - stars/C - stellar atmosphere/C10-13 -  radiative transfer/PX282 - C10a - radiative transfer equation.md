---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/c-stellar-atmosphere/c10-13-radiative-transfer/px-282-c10a-radiative-transfer-equation/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-22T15:32:21.574+00:00"}
---

- combining all the sources of opacity:
$$dI_{\lambda} = - \kappa_{\lambda}\rho I_{\lambda}\,dz + \epsilon_{\lambda}\rho \,dz$$
	where, $\kappa_{\lambda}= \kappa_{b-b} + \kappa_{b-f} + \kappa_{f-f} + \kappa_{H^{-}} + \kappa_{e-s}$ factors in all the absorptions
$$\frac{dI_{\lambda}}{\rho\kappa_{\lambda}\,dz} = -I_{\lambda} + \frac{\epsilon_{\lambda}}{\kappa_{\lambda}} $$
defining **the source function**: 
$$S_{\lambda} = \frac{\epsilon_\lambda}{\kappa_{\lambda}}$$
- therefore, the radiative transfer equation is:
$$- \frac{1}{\rho\kappa_{\lambda}} \frac{dI_{\lambda}}{dz} = I_{\lambda}-S_{\lambda}$$

- considering the balance between $I_{\lambda}$ and $S_{\lambda}$
	- if $I_{\lambda} > S_{\lambda}: \frac{dI_{\lambda}}{dz}<0$ , so, $I_{\lambda}$ decreases with $z$
	- if $I_{\lambda} < S_{\lambda}: \frac{dI_{\lambda}}{dz}>0$ , so, $I_{\lambda}$ increases with $z$
- thus, $I_\lambda$ converges to the source function
- the beam intensity approaches the local value of the source function ($S_{\lambda}$ may vary too quickly to reach)

- in $\tau$-space, the classic form of radiative transfer equation is obtained: 
$$\frac{dI_{\lambda}}{d\tau_{\lambda}} = I_{\lambda}- S_{\lambda}$$
