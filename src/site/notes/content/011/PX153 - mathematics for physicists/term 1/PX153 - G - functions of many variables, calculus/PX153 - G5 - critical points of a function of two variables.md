---
dg-publish: true
---

## for a function of one variable
$$\frac{df}{dx}|_{x_{c}} = 0$$
-  expanding $f(x)$ around this point using a taylor series: 
$$f(x) = f(x_{c}) + f'(x-x_{c})|_{x_{c}}+ \frac{1}{2}f''(x-x_{c})^{2}+...$$
$$f(x)-f(x_{c}) \approx \frac{1}{2} f''(x-x_{c})^{2}$$
	- $(x-x_{c})^{2}$ is always positive
	- for local maxima, $f(x)<f(x_{c}) \implies f''<0$
	- for local minima, $f(x)>f(x_{c}) \implies f''>0$
	- if  $f''=0$, might be point of inflection
## for a function of two variables
- there are three types of critical points:
	- local maxima
	- local minima
	- *saddle point*: approached along some directions, they look like maxima, and along other directions, they look like minima
- at all critical points, both $\frac{\partial f}{\partial x}=0$ and $\frac{\partial f}{\partial y} =0$
- for all maxima, all nearby points are lower in value; for all minima, all higher; and for saddle, some higher, some lower
- apply taylor series to second order, with the first order derivatives equal to zero
- we have, $(x-x_{c} = \Delta x$ , $y-y_{c}=\Delta y)$ : 
$$f(x,y) - f(x_{c},y_{c}) \approxeq \frac{1}{2!}f_{xx}\Delta x^{2} + \frac{1}{2!} f_{yy} \Delta y^{2} + f_{xy} \Delta x \Delta y$$
	- whose $f_{xx}... , etc$ are evaluated at $(x_{c},y_{c})$
- rearrange to be similar to the expression for a function of one variable, ie: square on $RHS$: 
$$f(x,y) - f(x_{c},y_{c}) \approx \frac{1}{2f_{xx}} (f_{xx}^{2} \Delta x^{2} + f_{xx}f_{yy} \Delta y^{2} + 2f_{xx}f_{xy} \Delta x \Delta y)$$
- completing the square: 
$$f(x,y) - f(x_{c},y_{c}) \approxeq \frac{f_{xx}}{2} (f_{xx}^{2} \Delta x^{2} + 2f_{xx}f_{xy} \Delta x \Delta y + f_{xy}^{2} \Delta y^{2} - f_{xy}^{2} \Delta y^{2} + f_{xx}f_{yy} \Delta y^{2})$$
$$f(x,y) - f(x_{c},y_{c}) \approx \frac{f_{xx}}{2} [(f_{xx}\Delta x + f_{xy}\Delta y)^{2} + ( f_{xx}f_{yy} - f_{xy}^{2}) \Delta y^{2}]$$
- $(f_{xx}\Delta x + f_{xy}\Delta y)^{2}>0$ and $\Delta y^{2}>0$ : always
- taking $\Delta = f_{xx}f_{yy} - f_{xy}^{2}$ :
	- if $\Delta >0$ and $\Delta t > 0$ :
		- if $f_{xx}>0 \implies f(x,y)-f(x_{c},y_{c})>0$, then $(x_{c},y_{c})$ is a *local minimum*
		- if $f_{xx}<0 \implies f(x,y)-f(x_{c},y_{c})<0$, then $(x_{c},y_{c})$ is a *local maximum*
	- if $\Delta <0$, then the sign of $f(x,y)-f(x_{c},y_{c})$ can change depending on the direction, ie: *saddle point*
	- if $\Delta = f_{xx}f_{yy} - f_{xy}^{2} = 0$, then the test is inconclusive

- eg: ![Pasted image 20240102113206.png](/img/user/pics/Pasted%20image%2020240102113206.png)

- eg: ![Pasted image 20240102113943.png](/img/user/pics/Pasted%20image%2020240102113943.png) ![Pasted image 20240102114004.png](/img/user/pics/Pasted%20image%2020240102114004.png)
- eg: ![Pasted image 20240102115518.png](/img/user/pics/Pasted%20image%2020240102115518.png) ![Pasted image 20240102115533.png](/img/user/pics/Pasted%20image%2020240102115533.png)
- eg: ![Pasted image 20240102121244.png](/img/user/pics/Pasted%20image%2020240102121244.png) ![Pasted image 20240102121308.png](/img/user/pics/Pasted%20image%2020240102121308.png)
	