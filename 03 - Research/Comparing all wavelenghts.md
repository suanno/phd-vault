#characteristic_lenghts #ell #ellDW #ellCC

We can measure three different characteristic wavelengths in the system [[ell]] [[ell CC]] [[ell DW]]
$$\ell, \ell_{DW}, \ell_{CC}$$
# Comparison (in the same canvas)
![[C=1.png]]
In the following plot, the thickness of the interface is estimated as the one of the stationary state associated with constant $C=\bar{C}$.
![[C0=1A=0.25T=0.1.png]]
**NOTICE**: We expect that, asymptotically, when domains are formed
$$\ell_{DW}\simeq\ell_{CC}\simeq\frac{L^2}{\mathcal L}$$
And we see that!
> **In the past,** the formula of the Cauchy-Croft theorem was wrongly implemented. Over than taking the average of the estimates (dividing by 4, that is the number of sets) also inside the formula for each estimate there was a division by a factor 4. On of the two is eccessive. The current formula has been tested on paper for estimating the perimeter of a circle, and it works.
​￼￼￼￼￼

​￼￼￼￼￼
> **Precedent plots** (with an **extra division by 4** of the total interface lenght):
> 
> ![[C=1_old.png|300]]![[C0=1A=0.25T=0.1_old.png|300]]
### Slope of $\ell_{CC}$
$l_{CC}$ s**eems to behave as $t\sim \frac12$ both in the linear and non-linear regime**, but actually a fit in the linear region and one in the non-linear show that:
- In the linear regime $t\sim t^{\frac12}$ as $\ell$ (green dashed line).
- Around $t=10$ the slope slightly changes (red dashed line). However we expect that, due to coarsening, $\ell_{CC}\sim t^{\frac12}$ asymptotically.
Fitted regions: $t = [1,10]$ (green dashed line); $t = [20,100]$ (red dashed line).
![[change_of_slope.png|300]]![[change_of_slope_zoom.png|300]]
See [[03 - Research/Linear regime#Keeping the system in the linear regime]] for more observations of $\ell_{CC}$ in the linear regime.
# Comparison (Linear regime)
Does the ratio between $\ell_C$ and $\ell_{CC}$ in the linear regime depend on the choice of $C$?
It seems **no**.
![[ratio_ell_ellCC.png]]

| ![[ratio_ell_ellCC_number.png]] | ![[ratio_ell_ellCC_number_zoom.png]] |
| ------------------------------- | ------------------------------------ |

# Comparison (Asymptotically)

Asymptotically, precisely when $\ell_{DW}$ well estimates the ratio $L^2/\mathcal{L}$ (see [[Master Report.pdf]]):

$$\ell^{-2} \simeq (2\pi)^{-2}D^{-1}I_1(C\ell_{DW}-I_2)^{-1}$$

Then, at sufficiently large times: $\ell_{DW}$ grows, so $(C\ell_{DW}-I_2)\simeq C\ell_{ÐW}$ that means

==$$\ell^{-2} = (2\pi)^{-2}(CD\ell_{DW})^{-1} I_1$$
Calculating the logarithm:

$$\log\ell = \frac12\log\ell_{DW}+ const.$$

$$const. = \log2\pi + \frac12\log (CD) - \frac12 \log I_1$$
![[asymptotically.png|300]]![[asymptotically_ellCC.png|300]]
