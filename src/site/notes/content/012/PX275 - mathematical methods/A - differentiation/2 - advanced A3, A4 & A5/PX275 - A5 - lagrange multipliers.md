---
dg-publish: true
---

-  typically, given a function, $f(x,y)$, a maxima or a minima can be found via the partial derivatives, ie: 
$$\frac{\partial f}{\partial x}=0\,;\, \frac{\partial f}{\partial y}=0$$
- or, it can be found in terms of the total derivative, ie: 
$$df = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy$$
- if the maximum or minimum of the function, $f(x,y)$, with respect to a constraint, $y=1-x$, is to be found, the constraint needs to be rewritten as a function, $g(x,y)=x+y=1$ 
- **note:** the constraint being exactly equal to a constant is critical for this method

- at the max of $f(x,y)$ subject to the constraint, $\frac{\partial f}{\partial x}\neq0;\, \frac{\partial f}{\partial y}\neq0$, but because $g(x,y)=constant$, it can be said that $dg = \frac{\partial g}{\partial x}dx+ \frac{\partial g}{\partial y}dy=0$
- without a formal proof, a statement for the minimum/maximum condition is: $$d(f+\lambda g)=0$$
	where, $\lambda$ is an undetermined constant, called the *lagrange multiplier*
- the total differential will be: 
$$\begin{gather} 
	d(f+\lambda g) = \left(\frac{\partial f}{\partial x} + \lambda \frac{\partial g}{\partial x}\right)\,dx + \left(\frac{\partial f}{\partial y} + \lambda \frac{\partial g}{\partial y}\right)\,dy = 0 \\
	\implies \left(\frac{\partial f}{\partial x} + \lambda \frac{\partial g}{\partial x}\right) =0 \\
	\text{and,}\,\left(\frac{\partial f}{\partial y} + \lambda \frac{\partial g}{\partial y}\right)\,dx =0 \\
	g(x,y) = \text{constant}
\end{gather}$$
- this system of simultaneous equations can be solved to find $x,\;y\;\text{and } \lambda$ 

![Pasted image 20241027162609.png](/img/user/pics/Pasted%20image%2020241027162609.png)
