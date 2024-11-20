#Crank-Nicolson #numerical

We integrate the **TDGL** (or Cahn-Allen) equation
$$\partial_t u = \partial_{xx}u +C(t)u-u^3\quad\text{(1D)}$$
$$\partial_t u = \Delta u +C(t)u-u^3\quad\text{(2D)}$$
with the Crank-Nicolson scheme (in Fourier space [see here](#Crank-Nicolson-In-Fourier-Space)).
The reason is that Implicit and Explicit Euler algorithm do not integrate correctly the dynamics of an initially flat profile $u(x)=u_0$ (0D case).


### Explicit and implicit Euler for an initially flat profile
Here we integrate the **1D** TDGL equation with Implicit or Explicit Euler's algorithm (in Fourier space) starting from a state $u(x,t=0)=1$. During the dynamics $C(t)$ oscillates as
$$C(t)=\sin(2\pi t)$$
So the average value of the oscillation is zero, this means that we should see
$$u(t)\sim t^{-\frac12}$$
Instead we see an exponential time dependance!
![[ExplicitImplicitCbar0.png]]

### Crank-Nicolson for an initially flat profile
Instead, integrating the same system with Crank-Nicolson scheme (in Fourier space), leads to the correct power-law decay!
![[Crank-Nicolson no saturation.png]]

# Linear dynamics
You can see better why the Euler schemes are not good, by integrating **only the linear part** of the equation. This time there is no need of Fourier transform as the equation to integrate is
$$\partial_t u = C(t)u$$

| ![[Explicit Euler explosion.png]] | ![[Implicit Euler explosion.png]] | ![[Crank-Nicolson-Linear.png]] |
| --------------------------------- | --------------------------------- | ------------------------------ |
You can see that $u(t)$ grows or decays exponentially fast also when the average value $\braket{C}=0$ if you use Implicit or Explicit Euler schemes. While Cranck Nicholson works fine.
# Crank-Nicolson-In-Fourier-Space 
To integrate the TDGL equation, we apply a Fourier transfrom in x, so
$$\partial_t u = \partial_{xx}u +C(t)u-u^3$$
becomes ($u(x,t)\rightarrow U_q(t)$)
$$\partial_t U_q = -q^2U_q+C(t)U_q-\mathcal{F}[u^3]_q\quad U_q\equiv\mathcal{F}[u(x)]_q$$