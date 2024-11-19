In the **appendix G** of the [[Master Report.pdf]] we show that, asymptotically, $\ell$ and $\ell_{DW}$ can be expressed one as a function of the other.
Although, there when we use the Parceval's theorem, we state that
$$(2\pi)^{-\frac12}\int q^2 |u_q|^2dq = \int |\nabla u(x)|^2dx$$
So that the fourier transform of $|\nabla u|^2$ is $q^2 |u_q|^2$ . But this is not clear to me. I know that
$$\mathcal{F}[\partial_{xx} u] = -q^2 \mathcal{F}[u]$$
$$\mathcal{F}[\partial_x u] = -iq \mathcal{F}[u]$$
while now we are stating that
$$\mathcal{F}[(\partial_x u)^2]=+q^2 |\mathcal{F}[u]|^2$$
That is like substituting $\nabla u$ in the integral with its fourier transform, but I don't know if it is fair as the integrand is not $\nabla u$ but $|\nabla u|^2$. And additionally, even if you do this trick, there is a sign minus missing.