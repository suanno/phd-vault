#1D #characteristic_lenghts #ellDW #randinit #numerical 
Here we consider an initial random state and a profile of C(t) that is
- C(t) linearly increases from -1 to +1 in a time $t_{ramp}$ (ramp quench)
- Once $t>t_{ramp}$ then $C(t)=1$ constant

# Simulations

![[time_function.png]]
The **average domain size** $\frac{L}{n}$, corresponds to the lenghtscale $\ell_{DW}$ or $\ell_{CC}$, as explained [[ell DW|here]].
We do not know how this wavelenght evolves in the linear regime, but let's say that it grows as a power law (we saw that $\ell_{CC}$ grows as a power law in the linear regime).
If $\frac{L}{N}\sim t^p$ in the linear regime, as the non-linear dynamics can be considered as frozen in 1D, the asymptotic average domain size will be $\sim \tau^p$ where $\tau$ is the duration of the linear approximation.
As C(t) increases as a ramp, reasonably $\tau\sim t_{ramp}$, so we expect
$$\frac{L}{n}\sim t_{ramp}^p$$
And that is what we see here, with $p\simeq 0.36$.
![[asymp_fit.png]]