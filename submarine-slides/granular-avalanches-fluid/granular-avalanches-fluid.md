## Granular avalanches in fluid
> du Pont, S. C., Gondret, P., Perrin, B., & Rabaud, M. (2003). Granular avalanches in fluids. _Physical review letters_, _90_(4), 044301.

[Paper](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.90.044301)

> Keywords: #granular-flow-regimes #viscous-regime #freefall-regime #inertial-regime #submarine 

### Research questions
- Capillary actions between grains affect the stability and dynamics of submerged slopes, but the role of interstitial fluid on the runout dynamics is unknown. 
- Why does submarine slopes evolve differently from the dry slopes?
> Submarine slopes fail continuously on lee-side, while dry slopes experience a more successive avalanches.


### Future research / unanswered questions
- What is the role of permeability and initial volume?
- Compute the velocity of the grains in the simulation and compare against the different regime limit velocities. 
### Main findings
- $\theta_m$ is the maximum angle of stability and $\theta_r$ is the repose angle.
- In the granular avalanches in a rotating drum under submerged conditions, the amplitude $\Delta \theta = \theta_m - \theta_r$ of avalanches decreases and the time duration $T$, which is the time taken for an avalanche angle to change from $\theta_m$ to $\theta_r$, increases with fluid viscosity.
- Three distinct flow regimes were observed: (i) free fall regime (no fluid/dry case), (ii) viscous, and (iii) inertial regime. The interstitial fluid governs the response of the final two regimes. 
- The avalanche amplitude $\Delta \theta$ and $T$ depend a lot on the grain diameters for submerged cases and is unaffected by the effect of grain size in the dry conditions. The grain diameters between 0.1 to 1 mm has a significant effect on the duration $T\propto\frac{1}{d^2}$, while a larger diameter of 1 to 5 mm have a moderate effect of $T \propto \frac{1}{\sqrt{d}}$.
- The equation of motion for the grain of velocity $u$ down the slope, between two collisions: 
$$\frac{\pi}{6}\rho_s d^3 \frac{du}{dt} = \frac{\pi}{6}\Delta \rho g d^3 \sin\theta -F_d \quad \Delta \rho = \rho_s - \rho_f$$
The grain momentum increases under the action of its apparent weight minus a fluid drag force $F_d$. 
- **Limit velocities**:
	- At $Re << 1$, the drag force is equal to the _viscous stokes force_, the grain will reach its viscous limit velocity.
	- At $Re >> 1$, $F_d$ is the inertial force.
- The Stokes number $St$ is the relative importance of grain inertia and fluid viscosity effects:
$$St = \frac{1}{18\sqrt{2}}\sqrt{\rho_s}\sqrt{(\Delta \rho g \sin \theta)} \frac{d^{3/2}}{\eta}$$
- The density ratio $r = \sqrt{\frac{\rho_s}{\rho_f}}$
- **Regimes**
	- For $St >> 1$ and $r >> 1$ the grain does not reach any limiting regimes over $d$ (grain size).
	- For $St << 1$ and $r >> 1$ the grain reaches the __limiting Stokes velocity__: $U_{\infty v}  = \Delta \rho g d^2 \sin \theta  / {18 \eta}$
	- For $St >> 1$ and $r << 1$ the grain reaches its __limiting inertial velocity__: $U_{\infty i} = \sqrt{2 \Delta \rho g d \sin \theta / \rho_f}$, using a drag coefficient $C_d = 1/\pi \approx 0.3$.
- For $St << 1$ and $r << 1$:
	- if $Re << 1$ the flow reaches viscous regime
	- if $Re >> 1$ the flow reaches inertial regime
- A critical $Re_c$ of 2.5 marks the transition between the viscous and inertial regimes.
- $St$ is the only parameter that governs the coefficient of restitution $e$ for an immersed binary collision between solid grains. 
- At $St_c \approx 10$, $e = 0$ collision is totally inelastic as all the kinetic energy of the grain is dissipated by the fluid during the collision process.
- Above an $St_c$ of 10, $e$ increases quickly and is a function only of the Stokes number and is independent of $r$. 
- $e$ reaches its maximum value in dry condition for $St = 100$.
- A $r_c = St_c / Re_c = 4$ of separates the free-fall regime from the inertial regime.

![Granular flow regimes](https://raw.githubusercontent.com/kks32-docs/notes/main/submarine-slides/granular-avalanches-fluid/granular-fluid-regimes.png)
> Granular flow regimes