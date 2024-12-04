#twokinks #1D #costantC

If C(t) is 
- **Strictly positive** $C(t)>0 \forall t$
- And its **oscillations are slow** $(T\gg \tau_{c})$
following the idea presented in [[Kink effective dynamics.pdf]] (and generalized for $C$ constant $\rightarrow$ slow oscillations limit in [[Kink effective dynamics under slow POSITIVE oscillations (theory)]]) it is possible to describe the evolution dictated by the TDGL with an **effective law** for the velocity of each kink. If $x_n$ is the position of the n-th kink  (the n-th zero of $u(x)$) and $l_n\equiv x_{n+1}-x_n$ is the lenght of the n-th domain:
$$\dot{x_n}(t)=16 C^{\frac12}(t)\frac{[e^{-2^{\frac12}C(t)^{\frac12}l_n}-e^{-2^{\frac12}C(t)^{\frac12}l_{n+1}}]}{\int_{\chi_{n-0.5}}^{\chi_{n+0.5}}d \chi \partial_{\chi} u_{p}(\chi)}$$
where $u_{p}(\chi)$ is the periodic stationary state with period $(\chi_{n+1}-\chi_{n_+1})$ and $\chi_{n}=C(t)^{\frac{1}{2}x_{n}}$.
If there are only two kinks and PBC boundaries are adopted (so if the distance from the right is $d$ then the distance from the left is $L-d$) the distance $d(t)$ will decrease in this way (L>d)
$$\dot{d}(t)=-2 * 16 C^{\frac12}(t)\frac{[e^{-2^{\frac12}C(t)^{\frac12}d}-e^{-2^{\frac12}C(t)^{\frac12}(L-d)}]}{\int_{\chi_{n-0.5}}^{\chi_{n+0.5}}d \chi \partial_{\chi} u_{p}(\chi)}$$
Where the integral at the denominator can be approximated by the integral of the single-kink stationary state and the integration is carried on the whole real axis: $\int_{\chi_{n-0.5}}^{\chi_{n+0.5}}d \chi \partial_{\chi} u_{p}(\chi)\simeq \int_{-\infty}^{+\infty}d \chi u_{k}(\chi)=I_{1}$
where $I_1$ has been calculated in the [[Master Report.pdf]] and $I_1 = \frac{2\sqrt{2}}{3}$.

If also the smaller exponential is neglected, in the limit $L\gg d$
$$\dot{d}(t)\simeq-24\sqrt{2} C^{\frac12}(t)e^{-2^{\frac12}C(t)^{\frac12}d}$$
# Annihilation time
To estimate the time-scale of the annhilation process, we consider the case where C is constant. The solution to the differential equation for $\dot{d}$ is
$$d(t)=A+\log(\alpha(t_{c}-t))$$
$A=(2C)^{-0.5}$; $\alpha = 48C$  and the annhilation time is
$$t_{c}=\frac{e^{d_{0}/A}}{\alpha}=\frac{{e^{d_{0}(2C)^{0.5}}}}{48C}$$

# Simulations
#### C is constant
In this case, we can verify the predicted result that prefactor of the logarithm, is $(2C)^{-\frac12}$.
![[decay.png]] ![[prefactor_slope.png]]
#### C(t) is a slow and positive oscillation
Here we can compare the expected law for $\dot{d}$ with a numerical simulation. Here the equation for $\dot{d}$ is integrated with Explicit Euler.
$$C(t)=1+1\sin\left( \frac{2\pi t}{500} \right)$$
![[C0=1A=1T=500.png]]
There isn't a good match, probably because the distance decays when C is very close to zero and there **the intrinsic timescale of the problem $\tau_{C}\sim C^{-1}$ diverges**, so we are no more in the limit of slow oscillations.