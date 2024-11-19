#structurefactor #ellCC #ell 
## Structure factor
This is a plot of the 1D structure factor, starting from random initial conditions.
It is represented in semi-log scale and shows
- Tails shaped like **absolute value** $\log S(q)\sim -|q|$;
- Center shaped like **a parabola** $\log S(q)\sim -q^2$

> **Olivier's guess**: The information described by $S(q)$ at the center is related to the **distribution of the kinks' positions**, while the information stored in the tails is related to the **kink's shape**. So the wavelenghts that you can extract from the two parts of the functions we expect to describe the two types of feature: the macroscopic one and the microscopic one.

This suggests the shape of $S(q)$ (in linear-linear scale) is
- An exponential $S(q)\sim e^{-|q|}$ if $|q|>>0$
- A gaussian $S(q)\sim e^{-q^2}$ if $|q|\simeq 0$
So, reasonably, $S(q)$ is a sum of the two
$$S(q)=\alpha e^{-|q|}+\beta e^{-q^2}$$
where the ratio $\beta/\alpha$ determines the value of $|q|$ where one of the two function becames more relevant than the other. So the value of $|q|$ where you see a **transition parabola to linear** in the following picture.
> **NOTICE**: The inverse **fourier transform** of both the functions **is known**! They are respectively
> - Lorentzian $$\mathcal{F}[e^{-a|x|}]=\frac{2a}{a^2+2\pi q^2}$$
> - Gaussian $$\mathcal{F}[e^{-t^2/2\sigma^2}]=\sigma\sqrt{2\pi}e^{-2(\sigma \pi q)^2}$$
> Should check
> - How to invert the transform (are they invertible?)
> - How the (inverse) Fourier transform is affected by shifts of the center (kink's position). 


| ![[time.png]] | ![[q2Sq.png]] |
| ------------- | ------------- |

### 3 wave-lenghts
You can spot three wavelenghts in the above plot
1) You can fit with a parabola the top (or with a Gaussian in linear-linear scale) and extract the value of the width (standard deviation): $\lambda = 2\pi/\sigma$
2) You can fit the tails with $e^{-\frac{|q|}{q_0}}$ and extract $q_0$: $\lambda = 2\pi/q_0$
3) You can extract the value of $|q|$ of the transition from parabola to linear: $\lambda = 2\pi/q_{transition}$

**IN GENERAL**: Think to the structure factor as a significative quantity only when you have a **concept of randomness** in the simulation (in the initial state preparation.). 
## Linear regime
### $q_{min}$
$q_{min}$ is the wave-vector related to the minimum wavelenght due to the lattice discretization $dx$. So we expect that $q_{min}\sim2\pi/dx$ and NOT $2\pi/L$.
We find that $q_{min}\simeq \pi/dx$, so it makes sense.
### Ratio $\ell/\ell_{CC}$
Compare the plot of $\ell$ and $\ell_{CC}$ both for $C>0$ constant and $C<0$ constant **in the linear regime**. Calculate the **ratio** in both cases, is that the same?
## MBC
Calculate $S(q)$ of a state with a distribution of circles.
Compare the shapes of $R(t)$ with $C>0$ oscillations.
Understand if really the initial state affects the dynamics at long times (initial width $\neq$ $\sqrt{\bar{C}}^{-1}$).