---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/g-fluctuations/px-284-g1-energy-deviation/","noteIcon":"1","created":"2025-08-27T13:14:32.674+01:00","updated":"2024-12-05T15:54:44.000+00:00"}
---

- in a canonical ensemble, $T$ is fixed, but $U$ (and hence $F, S, p$, etc) is calculated from an average energy, $\langle{E}\rangle$, so, in principle, could **fluctuate**
$$\langle{E}\rangle = \frac{1}{Z } \sum\limits_{i} E_{i} \exp(-\beta E_{i}) = - \frac{1}{Z} \frac{dZ}{d\beta}$$
- similarly, 
$$\langle{E^{2}}\rangle = \frac{1}{Z } \sum\limits_{i} E_{i}^{2} \exp(-\beta E_{i}) = - \frac{1}{Z} \frac{d^{2}Z}{d\beta^{2}}$$
- **note**: 
$$\frac{d\langle{E}\rangle}{d\beta} = - \frac{1}{Z } \frac{d^{2}Z}{d\beta^{2}} + \frac{1}{Z^{2}} \left(\frac{dZ}{d\beta}\right)^{2} = - (\langle{E^{2}}\rangle - \langle{E}\rangle^{2}) = - \sigma_{E}^{2}$$
	which is the **variance of energy**
- furthermore:
$$\frac{d\langle{E}\rangle}{d\beta} = \frac{dT}{d\beta} \frac{d\langle{E}\rangle}{dT} = - k_{B}T^{2} C_V$$
- thus, the **standard deviation of energy**:
$$\sigma_{E} = T \sqrt{k_{B}C_V}$$
## conclusions
- there is a finite probability for fluctuations in energy (and hence in $F, S, p,$ etc)
- the size of the fluctuations increase with increasing heat capacity