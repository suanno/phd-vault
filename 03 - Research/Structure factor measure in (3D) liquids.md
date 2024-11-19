#structurefactor #liquids 

In (3D) liquid the is no preferential direction, as in the present case. There, it is possible to measure experimentally the structure factor $S(\mathbf{q})$ with a **neutron scattering experiment** (the neutrons can have a wave-lenght of the order of the Amstrong, that can probe "patterns" with which molecules are arranged in space).

Assuming elastic scattering, if the incident wave vector $\mathbf{k_i}$ is fixed, then there is only one (due to energy conservation) scattered wave vector $\mathbf{k_o}$ for each **direction** $\Omega$. 
As a consequence, there is a bijective relation $\mathbf{k}\iff \Omega$ , where $\mathbf{k}=\mathbf{k_0}-\mathbf{k_i}$ is the momentum transferred to the sample. So the differential cross section $\frac{d\sigma}{d\Omega}(\Omega)$ is a function of $\mathbf{k}$
as we can say that $\Omega = \Omega (\mathbf{k})$. In particular, using the **Fermi Golden rule**:
$$\frac{d\sigma}{d\Omega}\propto S(\mathbf{k})$$
Experimentally, it is possible to measure the differential cross section: a detector, is placed at an angle $\Omega$. It will absorb all radiation scattered in the directions $[\Omega, \Omega+d\Omega]$, where $d\Omega$ is the same for every direction $\Omega$ if the detector is moved along an hemispherical guide. Then the number of detections, in a fixed amount of time equal for any direction $\Omega$, is counted. Dividing this measure by the cone of the detector $d\Omega$, will give a value that is proportional to the differential cross section, with a proportionality factor equal for any direction.
So we can measure $S(\mathbf{k})$ by putting a detector at a specific angle $\Omega(\mathbf{k},\mathbf{k_i})$.

**How do people actually measure the differential cross section in (3D) liquids?**
As there is isotropy, and so we expect $S(\mathbf{k})$ to be the same for values of $\mathbf{k}$ with the same magnitude, it is **reasonable that people move the detector only along $\theta$ and not $\varphi$** (as moving along $\varphi$ will not change the magnitude of $\mathbf{k_o}$ and so of $\mathbf{k}$).
NOTICE: the coordinate system is respect to the point where the scattering happens (the whole sample is a point if the detector is far).

So **I suppose** that when people plot $\hat{S}(q)$ they sample it by sampling the differential cross section at many angles $\theta$ , with a fixed $\varphi$. Then you can **label** each measure of the differential cross section at an angle $\theta$ as the value of $S(\mathbf{q})$ at the (it's unique once $\varphi$ is fixed) vector $\mathbf{q}$ associated with $\theta$.
Now, what is this vector $\mathbf{q}$? Its direction will change by changing $\theta$ **but we do not care about its direction**, but only about its magnitude, that (as the scattering is elastic) is given by
$$|\mathbf{q}| = 2|\mathbf{q_i}|\sin(\theta/2)$$
So, for any value of $|\mathbf{q}|$, you measure $S(\mathbf{q})$ for **one vector** $\mathbf{q}$ with that norm. And that is what you plot. 

So, experimentally, you **do not** sample $S(\mathbf{q})$ for many values of $\mathbf{q}$ with the same direction but different norm, **although** you expect to find the same result, due to isotropy.
And, experimentally, to get a point of the spectrum $\hat{S}(q)$ you do not measure $S(\mathbf{q})$ for many values with the same $|\mathbf{q}|$, but just for one; as if you evaluate $S(\mathbf{q})$ along one line in the q-space.