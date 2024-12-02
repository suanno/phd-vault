### MBC correction
Also if there are no oscillations of C(t) (**C is constant**), MBC 
$$v=-\kappa$$
is a leading order effect. This means there are higher order corrections that we are neglecting. As MBC is the leading contribution in the limit $\kappa\rightarrow 0$, then the **next-to-leading order contribution** would be **quadratic in $\kappa$**
$$v = -\kappa + \alpha \kappa^2$$
that, for an isolated circular domain is
$$\dot{R} = R^{-1}+\alpha R^{-2}$$
- **Numerically** we can fit the experimental curve with the **analytical solution** of the above equation, instead of the solution of $\dot{R}=-R^{-1}$. And we can see how $\alpha$ depends on C.
### What is a big/small correction to leading order dynamics?
- In **1D**, the oscillations of $C$ do not change how fast is the coarsening: it is still logarithmic as if C was constant. Although the **oscillations change the pre-factor of the logarithm**.
- In **2D**, the oscillations introduce a correction to MBC, but this correction **does NOT consist in changing the pre-factor** of the power-law coarsening $\sim t^{\frac12}$ (or of the linear decay of $R^2(t)$ for a circular domain). A correction exists, but it has a time dependence that is weaker than MBC's time dependence. 
Referring to the above considerations, we say that oscillations introduce a relevant change in the dynamics in 1D, but a non-relevant change in 2D.

### Ratio $\ell/\ell_{CC}$ in the linear regime
$\ell(t)$ is expected to evolve, during the linear regime, independently on C(t). Just the linear regime lasts for a time $\tau_C\sim C^{-1}$. So $\ell(t)$, during the linear regime, is the **same curve** for any choice of C(t). The fact that we see this also for $\ell_{CC}(t)$ is not trivial.
The experimental ratio $\ell(t)/\ell_{CC}(t)$ during the linear regime is $\simeq 0.8$.

# Dynamics of kinks under C(t)'s oscillations
Including the first order correction to the kink's shape when $C(t)$ is **slowly oscillating and strictly positive** in the calculations of [[Effective dynamics of kinks under slow POSITIVE oscillations]], we find that
$\dot{x}_n(t)$ evolves in the same way it evolves if $C$ is constant, but you substitute $C=C(t)$.
This holds in the limit when $\epsilon\rightarrow 0$, where $\epsilon\sim T^{-1}$ describes how slowly $C(t)$ varies in time.
We **expected** this result, because in the limit $\epsilon\rightarrow 0$ we expect **adiabatic dynamics**. Although what is surprising is that the correction to the formula of $\dot{x}_n$ that is of order $\sim \epsilon^1$ is zero, so the first order correction is of order $\sim \epsilon^2$.
This result is found assuming that the value of $u(x)$ at the midpoint of two kinks differs from the plateau value of an isolated kink by a value $\delta u_{p0}$ that **is at most of order** $\epsilon\sim T^{-1}$.
- Measure $\delta x, that is how much $x = d/2$ changes for two isolated kinks **in one period T**. Then plot $\delta_x$ as a function of $T^{-1}$ and expect the behavior at $T^{-1}\rightarrow 0$ to be **at least quadratic.**