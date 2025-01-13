---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/h-gases/px-284-h4-ideal-gas/","noteIcon":"1","created":"2025-01-13T10:30:42.838+00:00","updated":"2025-01-13T10:41:59.098+00:00"}
---

- ideal gases are classical and indistinguishable
- therefore, the partition function:
$$Z_{N} = \frac{Z_{1}^{N }}{N!} = \frac{1}{N!} \left(\frac{V}{\lambda_{th}^{3}}\right)^{N}$$
	where, $\lambda_{th} = \cfrac{h}{\sqrt{2\pi m k_{B} T}}$

- using **stirling's approximation**:
$$\ln Z_{N} = N \ln V  - 2N \ln \lambda_{th} - N \ln N + N$$
- previously:
$$p = - \left( \frac{\partial F}{\partial V}\right)_{T}$$
	where, $F = -k_{B}T\ln Z$
$$p = k_{B}T \left(\frac{\partial \ln Z_{N}}{\partial V}\right)_{T} = N k_{B} T \frac{\partial \ln V}{\partial V} = N k_{B}T$$
- therefore, the [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state\|ideal gas law]] is obtained:
$$pV = N k_{B} T$$

- it can also be found that:
$$U = \frac{3}{2}N k_{B}T \implies C_{V} = \frac{3}{2} N k_{B} T$$
- this agrees with [[content/012/PX284 - statistical mechanics/D - equipartition theorem/PX284 - D1 - equipartition theorem\|equipartition]]

- also:
$$F = N k_{B} T \left[ \ln \left(\frac{N\lambda_{th}^{3}}{V}\right) - 1 \right]$$
hence, the **sackur-tetrode equation**:
$$S = \frac{U-F}{T} = F = N k_{B} \left[ \frac{5}{2} - \ln \left(\frac{N\lambda_{th}^{3}}{V}\right) \right]$$
