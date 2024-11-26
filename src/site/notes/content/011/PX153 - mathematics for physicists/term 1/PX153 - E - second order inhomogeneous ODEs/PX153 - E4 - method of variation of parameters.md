---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-e-second-order-inhomogeneous-od-es/px-153-e4-method-of-variation-of-parameters/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:19.448+00:00"}
---

- a more general method for finding the particular integral
- consider a 2nd order inhomogeneous ODE: 
$$ay''+by'+cy = f(x)$$
- we first find the complementary function: 
$$y_{c} = C u_{1}(x) + D u_{2}(x)$$
- we assume that we can write the particular integral in the following form: 
$$y_{p}(x) = P(x)u_{1}(x) + Q(x)u_{2}(x)$$
for some arbitrary functions $P(x)$ and $Q(x)$
- we want to find $P(x)$ and $Q(x)$ in terms of $u_{1}(x), u_{2}(x), f(x)$
- first, calculate the derivative: 
$$y'_{p}(x) = P'(x)u_{1}(x) + P(x)u'_{1}(x) + Q'(x)u_{2}(x) + Q(x)u'_{2}(x)$$
- we put the following constraint: $P' u_{1}+ Q' u_{2}=0$
- the second derivative is then: 
$$y''_{p}(x) = P'(x)u'_{1}(x) + P(x)u''_{1}(x) + Q'(x)u'_{2}(x) + Q(x)u''_{2}(x)$$
- in the ODE, this gives: 
$$a(P'u'_{1} + Q'u'_{2})+ a( Pu''_{1} + Qu''_{2}) + b(Pu'_{1} + Qu'_{2}) + c(Pu_{1}+Qu_{2})=f(x)$$
$$a(P'u'_{1} + Q'u'_{2}) + P(au_{1}'' + bu_{1}' +cu_{1}) + Q(au_{2}'' + bu_{2}' +cu_{2})= f(x)$$
$$a(P'u'_{1} + Q'u'_{2}) = f(x)...[2]$$
$$P'u_{1}+Q'u_{2}= 0 ...[1]$$
- from $[1]$: 
$$Q' = - \frac{u_{1}}{u_{2}}P'$$
- subbing in $[2]$: 
$$P'\left( \frac{u'_{1}u_{2}-u_{1}u'_{2}}{u_{2}}\right) = \frac{f(x)}{a}$$
$$\implies P' = - \frac{1}{a}\frac{u_{2}f(x)}{u_{1}u'_{2}-u'_{1}u_{2}}$$
$$\implies Q' = \frac{1}{a} \frac{u_{1}f(x)}{u_{1}u'_{2}-u'_{1}u_{2}}$$
## problem class notes
- $y = u y_{1} + vy_{2}$ is a solution
- we can use two equations:
	$$u' y_{1} + v' y_{2}=0$$
	$$u' y_{1}' + v' y_{2}' = f(x)$$
- you should end up with 4 equations
