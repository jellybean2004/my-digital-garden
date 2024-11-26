---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-e-ac-circuits/px-157-e4d-solving-as-an-ode/","created":"2024-10-01T18:27:10.291+01:00","updated":"2024-11-26T20:11:28.722+00:00"}
---

- $V(t)$ is a general time-dependant input:
$$\begin{gather*}
	V_{in}(t) = RI + L \frac{dI}{dt} + \frac{Q}{C} \\
	L \frac{d^{2}I}{dt} + R \frac{dI}{dt} + \frac{1}{C}I = \frac{dV_{in}}{dt}
\end{gather*}$$
- homogeneous part:
$$\begin{align*}
	I(t) &\sim e^{\lambda t} \\
	 L\lambda^{2}+R\lambda+ \frac{1}{C} &= 0 \\
		 \lambda_{\frac{1}{2}} &= -\frac{R}{2L} \pm \frac{1}{2L} \sqrt{R^{2}- \frac{4L}{C}}
\end{align*}$$
