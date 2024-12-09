It seems to be a taugh challenge to find out what are the time-scales in the system
$$\partial u = \partial_{xx}u+C(t)u-u^3$$
where $$C(t)=\bar{C}+A\sin\left( \frac{2\pi t}{T_{0}} \right)$$
We can point out those time-scales:
- $T$ **time-scale of the $C(t)$'s oscillations**
- **Coarsening's time-scale**: 
	The fact that $L\sim t^{1/2}$ is associated to a time-scale. In fact coarsening proceeds with MBC that tells $v=-\kappa$. As we have a velocity, we can define the time-scale describing how much time it takes for an interface to move over a distance of order 1:
	$$dx\sim 1, v=-\kappa \implies dt \sim \kappa^{-1}$$
	So, if we consider an "average curvature" $\bar{k}$, then we have a timescale $\bar{\kappa}^{-1}$ .
- Time-scale of the **growth of large-$\lambda$ modes in the linear regime**:
	In the linear regime, we can neglect the non-linear term in the equation and we have the dispersion relation
		$$\sigma(q)=i \omega = C(t)-q^2$$
	so $q=0$ is the fastest growing mode, that grows as
	$$u_{q=0}(t)=u_{q=0}(0)e^{\int_{0}^tdt' C(t')}$$
	if this growth is slow such that the linear approximation holds for a time $\tau_{linear}\gg T$, then we can approximate
	$$u_{q=0}(t)\sim e^{\bar{C}}t$$
	and so we recognize the time-scale
$$\tau_{linear}\sim \bar{C}^{-1}$$
	==**BUT** it is important to enhance that  $\tau_{linear}\gg T$, means that the oscillations are sufficiently fast==. If they are not, then not only the average of C(t) matters and **we have a continum set of time-scales.** $$\tau\sim C(t)^{-1}$$
	and this **diverges if C(t) gets close to zero**