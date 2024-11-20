#Crank-Nicolson #numerical

We integrate the TDGL equation
$$\partial_t u = \partial_{xx}u +C(t)u-u^3\quad\text{(1D)}$$
$$\partial_t u = \Delta u +C(t)u-u^3\quad\text{(2D)}$$
with the Crank-Nicolson scheme (in Fourier space [see here](#Crank-Nicolson-In-Fourier-Space)).
The reason is that Implicit and Explicit Euler algorithm do not integrate correctly the dynamics of an initially flat profile $u(x)=u_0$ (0D case).





# Crank-Nicolson-In-Fourier-Space 