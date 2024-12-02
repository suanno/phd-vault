#mbc #2D #circular_island #ellCC #numerical #timedependingC 

Analytically, we expect that if $C(t)$ is a **strictly postitive** oscillation, in the limit where the oscillations are **slow or fast** (respect to the dynamics), then the MBC law
$$v = -\kappa$$
that for an isolated circular domain is 
$$R^2(t)=R^2_{0}-2t$$
**still holds up to first order** in $\epsilon = 2\pi (\frac{\tau_{C}}{T})$; $\tau_{C}\sim C^{-1}$ if T is large (analogous wit $T^{-1}$ if it is small)
# Resumee
Here I show some simulations carried in the two limit. An **extrapolation** at dt=0 shows that the deviation from the MBC law goes to zero if $dt\rightarrow 0$. So the effect we see in the following plot is a **numerical effect** and so there is no real influence of C(t)'s oscillations on the MBC (or at least, if there is is much smaller than the effect we see on the plots) 

# Simulations
We simulate the evolution of a circular domain. The radius is measured by measuring the perimeter of the circle as [[ell CC]]. We do not see triangular shaped variations of $R^2(t)$ when C(t) gets close to zero.

In the following plots it seems that
- An oscillation of C(t) that gets closer to zero leads to a faster anhilation of the domain.
- If C is constant and closer to zero, the domain anhilates faster.

| ![[98 - Images/circular domain/positive oscillations/Cbar=1/varyA.png]] |
| ----------------------------------------------------------------------- |
| ![[Ccost.png]]                                                          |
## But it is (at least mainly) a numerical effect!
Among the following simulations, we change only dt.

| ![[98 - Images/circular domain/positive oscillations/Cbar=1/dt.png]] |
| -------------------------------------------------------------------- |
| ![[98 - Images/circular domain/C=1/dt.png]]                          |
And if we fit, with a line, those experimental curves, we find that an extrapolation to dt=0 leads to a slope of about -2, that is the usual MBC law!

| $$\bar{C}=1; A=1; T=25$$![[98 - Images/circular domain/positive oscillations/Cbar=1/dt_slope.png]] | $$C=1$$![[98 - Images/circular domain/C=1/dt_slope.png]] |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
