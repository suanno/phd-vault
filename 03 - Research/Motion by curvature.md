#2D #circular_island #mbc

In the limits of
- Slow oscillations and $C(t)>0$ strictly
- Fast oscillations and $\bar{C}>0$
We prove that, up to firs order in $\epsilon$, the dynamics is dictated by motion by curvature (**MBC**), that means the velocity of an interface between domains is proportional to the local curvature $\kappa$
$$v=-\kappa$$
## Circular domain
![[R0=50L=4096.png]]
If the MBC law is applied to the case of an (isolated) circular domain with initial radius $R_0$, then the curvature is $R^{-1}$, while the interface velocity is $\partial_t R$, so
$$R^2(t)-R_0^2=-2t$$
This means that $R^2$ decays linearly with time and the island eventually disappears at a time $t_c = R_0^2/2$. However, in the proof of MBC we assume that the curvature $\kappa$ is small everywhere, but when the island becomes very small, then $R$ is small and so $\kappa=R^{-1}$ is very large. So, close to $t_c$, we do not expect the MBC law to hold, so the actual $t_c$ will be different than the predicted one (in particular, simulations show that $t_c < R_0^2/2$).
### How to measure $R$
It is possible to use the **Cauchy-Crofton (CC) formula** to estimate the lenght of the interface $\mathcal{L}$ (that is the perimeter of the circle) and then estimate 
$$R(t)=\mathcal L/(2\pi)$$