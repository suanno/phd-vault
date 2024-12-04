#characteristic_lenghts #ell #ellDW #ellCC

We can measure three different characteristic wavelengths in the system [[ell]] [[ell CC]] [[ell DW]]
$$\ell, \ell_{DW}, \ell_{CC}$$
Here we will discuss how them are related. We will show experimental images where **$C$ is constant (C=1), but the relations we discuss hold generally unless specified.**
# Comparison (in the same canvas)
![[C=1.png]]
**Analytically**, we expect that
- $\ell \sim t^{1/2}$ in the linear regime (see [[03 - Research/Linear regime|Linear regime]])
- $\ell_{DW}\simeq\ell_{CC}\simeq\frac{L^2}{\mathcal L}$ asymptotically, as they both estimate the average domain lenght, once domains are formed.
- $\ell_{DW}, \ell_{CC} \sim t^{1/2}$ asymptotically for **coarsening**.
and we see that. Then we also see **numerically** that
- $\ell_{CC}\sim t^{1/2}$ in the linear regime (see [[ell CC]] for more)
- $\ell_{DW}$ makes no sense in the linear regime
# Comparison (Linear regime)
Does the ratio between $\ell_C$ and $\ell_{CC}$ in the linear regime depend on the choice of $C$?
It seems **no**. This ratio is **around 0.8**.
![[ratio_ell_ellCC.png]]

| ![[ratio_ell_ellCC_number.png]] | ![[ratio_ell_ellCC_number_zoom.png]] |
| ------------------------------- | ------------------------------------ |

# Comparison (Asymptotically)

Asymptotically, precisely when $\ell_{DW}$ well estimates the ratio $L^2/\mathcal{L}$ (see [[Master Report.pdf]]):

$$\ell^{-2} \simeq (2\pi)^{-2}D^{-1}I_1(C\ell_{DW}-I_2)^{-1}$$

Then, at sufficiently large times: $\ell_{DW}$ grows, so $(C\ell_{DW}-I_2)\simeq C\ell_{ÐW}$ that means

==$$\ell^{-2} = (2\pi)^{-2}(CD\ell_{DW})^{-1} I_1$$
$$\log\ell = \frac12\log\ell_{DW}+ const.$$

$$const. = \log2\pi + \frac12\log (CD) - \frac12 \log I_1$$
As we said before, asymptotically $\ell_{DW}=\ell_{CC}$ so the same is expected for $\ell_{CC}$:

![[asymptotically.png|300]]![[asymptotically_ellCC.png|300]]
