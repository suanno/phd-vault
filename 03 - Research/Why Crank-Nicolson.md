#Crank-Nicolson #numerical

We integrate the TDGL equation
$$\partial_t u = \partial_{xx}u +C(t)u-u^3\quad\text{(1D)}$$
$$\partial_t u = \Delta u +C(t)u-u^3\quad\text{(2D)}$$
with the Crank-Nicolson scheme (in Fourier space [see here](#Crank-Nicolson-In-Fourier-Space)).
The reason is that Implicit and Explicit Euler algorithm do not integrate correctly the dynamics of an initially flat profile $u(x)=u_0$ (0D case).


### Explicit and implicit Euler for an initially flat profile
Here we integrate the 1D TDGL equation with Implicit or Explicit Euler's algorithm (in Fourier space) starting from a state $u(x,t=0)=1$. During the dynamics $C(t)$ oscillates as
$$C(t)=\sin(2\pi t)$$
So the average value of the oscillation is zero, this means that we should see
$$u(t)\sim t^{-\frac12}$$
Instead we see an exponential time dependance!
![[ExplicitImplicitCbar0.png]]

### Crank-Nicolson for an initially flat profile
Instead, integrating the same system with Crank-Nicolson scheme (in Fourier space), leads to the correct power-law decay!
![[Crank-Nicolson no saturation.png]]
# Crank-Nicolson-In-Fourier-Space 