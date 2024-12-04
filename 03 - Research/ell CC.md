This, togheter with [[ell DW]] and [[ell]] is a wave-lenght of the system that we can measure in simulations as a function of time.
This wave-lenght estimates the average domain lenght by dividing the area of the system ($L^2$) by the **total interface lenght $\mathcal{L}$.**

We estimate the (total) length of the interfaces $\mathcal{L}$ by using the Cauchy-Crofton theorem, using 4 families of parallel lines: horizontal, vertical, $\pi/4$, $3\pi/4$. Then we calculate the estimate for each family of lines and we compute the average $\mathcal{L}$
$$\ell_{CC}=\frac{L^2}{\mathcal{L}}$$
The Cauchy-Croft formula is, **for each family of line**:
$$\mathcal{L} \simeq \frac12*n*dx*\pi$$
([[do Carmo, Manfredo. Differential geometry of curves and surfaces.pdf]] P. 48)
- n is the number of times the interface crosses the parallel lines
- dx is the spacing between the lines

### Slope of $\ell_{CC}$
$l_{CC}$ s**eems to behave as $t\sim \frac12$ both in the linear and non-linear regime**, but actually a fit in the linear region and one in the non-linear show that:
- In the linear regime $t\sim t^{\frac12}$ as $\ell$ (green dashed line).
- Around $t=10$ the slope slightly changes (red dashed line). However we expect that, due to coarsening, $\ell_{CC}\sim t^{\frac12}$ asymptotically.
Fitted regions: $t = [1,10]$ (green dashed line); $t = [20,100]$ (red dashed line).
$$C = 1\quad\text{constant}$$
![[change_of_slope.png|300]]![[change_of_slope_zoom.png|300]]
See [[03 - Research/Linear regime#Keeping the system in the linear regime]] for more observations of $\ell_{CC}$ in the linear regime.
