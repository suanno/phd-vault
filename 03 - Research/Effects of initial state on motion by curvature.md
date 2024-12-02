#mbc #early_dynamics 

Here we consider the initial state to be an isolated circular domain
$$u(r,t=0)=-u_0\tanh((r-R_0)W^{-1})$$
where $u_0$ and $W$ represent the height and the width of the kink/interface.

> Do different values of $u_0$ and $W$ lead to a different evolution of the radius $R(t)$?
> **Do the initial conditions influence $R(t)$** in the early dynamics or in the late one?

Here I show some simulations, where it appears that the measure of $R(t)$ **seems to NOT be affected** by the choices of $u_0$ or $W$.

### C constant
In the following simulations, $C=0.1$ constant
![[C=0.1const.png]]
Here I show also the profile of the initial states considered above, obtained by evaluating $u(x,y)$ at time t=0 along $x=L/2$. You can see that the **blue and the green curves have the same kink's slope** (the first derivative is the same), this means that the width $W$ is the same.
![[C=0.1.png]]
### C oscillating
![[98 - Images/circular domain/initial conditions/C0=1A=1T=50.png]]
![[98 - Images/circular domain/initial conditions/saves/C0=1A=1T=50.png]]
### But remember that
Motion by curvature is a first (leading) order effects, so if C changes the curve $R(t)$ will change. See [[Motion by curvature CORRECTIONS]].