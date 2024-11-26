---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-i-integration/px-153-i3-domain-of-integration/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:38:05.046+00:00"}
---

![Pasted image 20240110183917.png](/img/user/pics/Pasted%20image%2020240110183917.png) 
- the region, $R$, is divided into $m\times n$ rectangles by dividing the interval $a \leq x \leq b$ into $m$ stripes, and $c \leq y \leq d$ into $n$ stripes
- each of the rectangles has area, $\Delta A_{rs} = (x_{r}-x_{r-1})(y_{s}-y_{s-1}) = \Delta x_{r} \Delta y_{s}$
- the volume of the column above $\Delta A_{rs}$ is: 
$$f(\bar x_{r} , \bar y_{s})\Delta x_{r} \Delta y_{r}$$
		where, $(\bar x_{r} , \bar y_{r})$ is some point in the range $x_{r-1} \leq \bar x_{r} \leq x_{r}$ and $y_{s-1} \leq \bar y_{s} \leq y_{s}$
- the total volume is then: 
$$I = \sum\limits_{s=1}^{m}\sum\limits_{r=1}^{n} f(\bar x_{r} , \bar y_{s})\Delta x_{r} \Delta y_{r}$$
- taking the limit $n\to \infty$: 
$$I = \sum\limits_{s=1}^{m} \left( \int_{a}^{b} f(x , \bar y_{s}) .dx \right) \Delta y_{r} \simeq \sum\limits_{s=1}^{m} g(\bar y_{s})\Delta y$$
- taking the limit $m\to \infty$: 
$$I = \int_{c}^{d} \left(\int_{a}^{b} f(x, y) .dx \right) .dy$$
- eg: evaluate $I = \int\int_{R} xy.dx.dy$, where $R$ is the rectangle with vertices $(0,0)$, $(0,2)$, $(1,0)$, $(1,2)$
	![Pasted image 20240110183946.png](/img/user/pics/Pasted%20image%2020240110183946.png) 
	$$I = \int_{0}^{2} \int_{0}^{1} xy.dx.dy = \int_{0}^{2} \left[ \frac{x^{2}}{2}y \right]_{0}^{1}.dy = \int_{0}^{2} \frac{y}{2}.dy = \left[ \frac{y^{2}}{4} \right]_{0}^{2} =1$$