#twokinks #1D #costantC 

If C(t)'s oscillations are fast respect to the intrinsic time-scale of the system, we know from [[Fast oscillations 1D]] that the zeroth-order shape of an isolated kink is 
$$m_0(x,t) = \sqrt{\bar{C}}\tanh(x\sqrt{\frac{\bar{C}}{2}})$$
As a consequence, we expect that (==but I didn't check this on paper==) the kink's dynamics, to leading order, is the same that you have if $C$ was constant, but with $C\rightarrow \bar{C}$ (see [[Kink effective dynamics under slow POSITIVE oscillations (theory)|here]] for a proof)
$$\dot{x_n}(t)=16 \bar{C}^{\frac12}\frac{[e^{-2^{\frac12}\bar{C}^{\frac12}l_n}-e^{-2^{\frac12}\bar{C}^{\frac12}l_{n+1}}]}{\int_{\chi_{n-0.5}}^{\chi_{n+0.5}}d \chi \partial_{\chi} u_{p}(\chi)}$$
For two isolated kinks, at a distance $d\ll L$
$$\dot{d}(t)\simeq-24\sqrt{2} \bar{C}^{\frac12}(t)e^{-2^{\frac12}\bar{C}^{\frac12}d}$$
# Simulations
![[C0=1A=0.5T=0.1.png]]
![[C0=1A=2T=0.1.png]]
