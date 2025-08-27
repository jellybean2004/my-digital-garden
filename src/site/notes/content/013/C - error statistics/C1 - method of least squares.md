---
{"dg-publish":true,"permalink":"/content/013/c-error-statistics/c1-method-of-least-squares/","noteIcon":"1","created":"2025-08-27T13:15:28.392+01:00","updated":"2025-08-21T10:42:20.000+01:00"}
---

![least squares.png|500](/img/user/pics/least%20squares.png)
*image: TPA Hase, PX271 data analysis course*

- the residual of a data point is defined as:
$$R_{i} = y_{i} - y(x_{i})$$
	where, $y_{i}$ is the measured value, and $y(x_{i})$ is the theoretical value

- the method of least squares minimises the sum of the squares of the residuals by changing the slope and the intercept of the line of fit
- the 'goodness of fit' is tested by the **chi squared** statistic:
$$\chi^{2} = \sum\limits_{i} R_{i}^{2} = \sum\limits_{i} (y_{i} - y)^{2}$$
- **homoscedastic data** refers to data with the same uncertainties
- **heteroscedastic data** refers to data with different uncertainties, hence each point is weighted equally
- normalised residuals weigh the residuals by the uncertainties such that:
$$R_{norm} = \frac{R}{\alpha}$$
- the weighting is inversely proportional to its error
$$\chi^{2} = \sum\limits_{i} \frac{R_{i}^{2}}{\alpha_{i}^{2}} = \sum\limits_{i} R_{i,\,norm}^{2} $$

- for poisson data:
$$\chi^{2} = \sum\limits_{i} \frac{(O_{i}-E_{i})^{2}}{E_{i}}$$
	where, $O$ and $E$ are the obtained and the expected values
- the data are re-binned such that each interval contains expected counts more than 5

- $\chi^{2} = 1$ equates to $1\,\sigma$ confidence limit
- the ellipticity and shape of the error surface around $\chi^{2}_{min}$ indicated correlations between the errors and the fit parameters
- this needs to be incorporated into error propagation

![modified error propagation.png](/img/user/pics/modified%20error%20propagation.png)
*image: TPA Hase, PX271 data analysis course*
