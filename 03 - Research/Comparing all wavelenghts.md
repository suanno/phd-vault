#characteristic_lenghts #ell #ellDW #ellCC

We can measure three characteristic wavelengths in the system:
## $\ell$
$$\braket{q^2}\equiv \frac{\int q^2 |u_q|^2dq}{\int |u_q|^2dq}$$
$$\ell \equiv \frac{2\pi}{\sqrt{\braket{q^2}}}$$
We know from [[Linear regime]] that, during the **linear regime**
$$\ell\sim t^{\frac12}$$
Then, in appendix G of the [[Master Report.pdf]] we show that, asymptotically this wavelength is related to $\ell_{ÐW}$ that asymptotically shows the coarsening exponent $\frac12$: $\ell_{DW}\sim t^{\frac12}$  so
$$\ell\sim t^{\frac14}$$
## $\ell_{DW}$
$$\ell_{DW} = \frac{L^2}{\int |\nabla u|^2 dxdy}*W$$
Where $W$ is the width of the interface, defined as the integral of the derivative of the field $u(x,y)$ along a direction perpendicular to the interface. We estimate this integral by considering the stationary state with $C=\bar{C}$:
$$u_k(\xi) = \sqrt{C}\tanh(\sqrt{\frac{C}{2}}\xi)$$
$$W=\int_{-\infty}^{\infty}(\partial_{\xi}u_k(\xi))^2 d\xi = \frac23 \sqrt2 C^{\frac32}$$
(the last integral is calculated in Appendix G of the [[Master Report.pdf]]).
As the gradient is peaked in the regions close to the interfaces, $\ell_{DW}$ should estimate the ratio between the size of the system $L^2$ and the (total) length of the interfaces $\mathcal{L}$.
## $\ell_{CC}$
We estimate the (total) length of the interfaces $\mathcal{L}$ by using the Cauchy-Crofton theorem, using 4 families of parallel lines: horizontal, vertical, $\pi/4$, $3\pi/4$. Then we calculate the estimate for each family of lines and we compute the average $\mathcal{L}$
$$\ell_{CC}=\frac{L^2}{\mathcal{L}}$$
The Cauchy-Croft formula is, **for each family of line**:
$$\mathcal{L} \simeq \frac12*n*dx*\pi$$
([[do Carmo, Manfredo. Differential geometry of curves and surfaces.pdf]] P. 48)
- n is the number of times the interface crosses the parallel lines
- dx is the spacing between the lines
# Comparison (in the same canvas)
![[C=1.png]]
In the following plot, the thickness of the interface is estimated as the one of the stationary state associated with constant $C=\bar{C}$.
![[C0=1A=0.25T=0.1.png]]
**NOTICE**: We expect that, asymptotically, when domains are formed
$$\ell_{DW}\simeq\ell_{CC}\simeq\frac{L^2}{\mathcal L}$$
And we see that!
> **In the past,** the formula of the Cauchy-Croft theorem was wrongly implemented. Over than taking the average of the estimates (dividing by 4, that is the number of sets) also inside the formula for each estimate there was a division by a factor 4. On of the two is eccessive. The current formula has been tested on paper for estimating the perimeter of a circle, and it works.
> **Precedent plots** (with an **extra division by 4** of the total interface lenght):
> 
> ![[C=1_old.png|300]]![[C0=1A=0.25T=0.1_old.png|300]]
### Slope of $\ell_{CC}$
$l_{CC}$ s**eems to behave as $t\sim \frac12$ both in the linear and non-linear regime**, but actually a fit in the linear region and one in the non-linear show that:
- In the linear regime $t\sim t^{\frac12}$ as $\ell$ (green dashed line).
- Around $t=10$ the slope slightly changes (red dashed line). However we expect that, due to coarsening, $\ell_{CC}\sim t^{\frac12}$ asymptotically.
Fitted regions: $t = [1,10]$ (green dashed line); $t = [20,100]$ (red dashed line).
![[change_of_slope.png|300]]![[change_of_slope_zoom.png|300]]
See [[Linear regime#Keeping the system in the linear regime]] for more observations of $\ell_{CC}$ in the linear regime.
# Comparison (Linear regime)
Does the ratio between $\ell_C$ and $\ell_{CC}$ in the linear regime depend on the choice of $C$?
It seems **no**.
![[ratio_ell_ellCC.png]]

| ![[ratio_ell_ellCC_number.png]] | ![[ratio_ell_ellCC_number_zoom.png]] |
| ------------------------------- | ------------------------------------ |

# Comparison (Asymptotically)

Asymptotically, precisely when $\ell_{DW}$ well estimates the ratio $L^2/\mathcal{L}$:

$$\ell^{-2} \simeq (2\pi)^{-2}D^{-1}I_1(C\ell_{DW}-I_2)^{-1}$$

Then, at sufficiently large times: $\ell_{DW}$ grows, so $(C\ell_{DW}-I_2)\simeq C\ell_{ÐW}$ that means

==$$\ell^{-2} = (2\pi)^{-2}(CD\ell_{DW})^{-1} I_1$$
Calculating the logarithm:

$$\log\ell = \frac12\log\ell_{DW}+ const.$$

$$const. = \log2\pi + \frac12\log (CD) - \frac12 \log I_1$$
![[asymptotically.png|300]]![[asymptotically_ellCC.png|300]]
