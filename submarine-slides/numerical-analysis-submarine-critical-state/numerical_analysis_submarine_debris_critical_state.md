## Numerical analysis of submarine debris flow based on critical state soil mechanics
> Kobayashi, T., Soga, K., & Dimmock, P. (2015). Numerical analysis of submarine debris flows based on critical state soil mechanics. In _Frontiers in Offshore Geotechnics III: Proceedings of the 3rd International Symposium on Frontiers in Offshore Geotechnics (ISFOG 2015) (Vol. 1, pp. 975-980). Taylor & Francis Books Ltd.

[Paper](https://search.proquest.com/docview/2115978348)

> Keywords: #submarine #water_entrainment #bingham 

### Research questions

- Why do submarine slides flow longer than subaerial despite the resistance due to surrounding water?
> One hypothesis is the entrainment of water at the flow front resulting in a decrease in strength. The reduction of shear strength can explain the long run-out.

- How do fine-grained sediments (clay-rich materials) affect the run-out?

- Phase transition from solid to semifluid occurs due to shearing, mixing, and water entrainment beneath the flowing material - has this been proven?
> Several assumptions have been made on how water entrainment influences the run-out and decrease in strength. More research is needed.

- How do the mechanical properties of the sediments change at the sliding plane?

- What is the proportion of water entrainment at the bottom vs. the rest of the sediments?


## Questions to consider

- How can the critical state be modified to accommodate higher water contents? 
> Can we use similarities with liquefaction to study this behavior?

- Does the mechanical properties vary with the duration and the flow?
 
- What range of liquidity index should be considered?

- The assumptions of how water entrainment (occurs after reaching CSL, follows the path of CSL) affects the run-out behavior is not established.

- What is the occurrence and magnitude of water entrainment in real debris flows?

- How does the volume of sediment expand with run-out due to water entrainment? What is the impact of the specific volume on this behavior? 

- Can we relate the distance traveled with the amount of water entrainment, or is there a critical threshold?

- Shear strength and viscosity change with water entrainment and run-out. What is the relationship?

## Main findings

- Non-newtonian fluid models do not accommodate for the transition in material properties by assuming constant rheological parameters throughout the flow.
- Rheological flow models approximate the regime changes (solid to fluid-like) over the spatial and temporal domains and do not capture the real mechanics. 
- The undrained strength from critical state soil mechanics is found to change with liquidity index ($I_L$) as $S_u = 1.7 \times 100^{(1- I_L)}$
- The original critical state assumption does not deal with high water content (where the water content is larger than the liquid limit).
- A new power-law relationship is proposed between the liquidity index and undrained strength: $S_u = 1.07 I_L^{-0.258}$
- Locat (1997) defined the Bingham viscosity as: $\mu = \left(\frac{9.27}{I_L}\right)^{3.3}$
- Because of the proposed powerlaw relationship for critical state line, the algorithm of specific volume rather than the specific volume is used, as proposed by (Butterfield., 1979).
- The modified Cam-Clay Bingham shear strength is proposed as
$$ \tau = \tau_{cam}(I_L, \varepsilon_v^p, \varepsilon_d^p) + \mu(I_L)\dot{\gamma}$$
where $\tau$ is the shear strength, $\varepsilon_v^p$, and $\varepsilon_d^p$ are the plastic volume and deviatoric strains, $\mu$ is the viscosity, and $I_L$ is the liquidity index. The first term represents the shear resistance of the sediment and becomes less dominant on large shear strains. The second term represents the strain-rate-dependent resistance due to viscosity.
- If the two terms $\tau_{cam}$ and $\mu(I_L)$ are constant, then the conventional Bingham fluid model is recovered. 
- Sensitivity of clay is considered by including a hardening parameter $p_d$ to the modified cam clay yield surface. Including sensitivity allows to model the measured peak strength and softening behavior. 
- To model the phase transition behavior due to water entrainment, the following assumptions are made:
	- water entrainment occurs after soil reaches the critical state
	- volume expansion happens along the critical state line
	- mean stress $p^\prime$ and $q$ decreases along CSL
- The occurrence and magnitude of water entrainment in real debris flows are not well understood.
- Instead, (2004) observed water entrainment mainly occurring at the bottom of the flow front.
- Effect of water entrainment (strength reduction) is modeled as a function of the distance traveled by the material points.
	- The rate of volume expansion ($R_v$)  against the travel distance and the maximum specific volume $V_{max}$ control the effect of water entrainment, but the factors and their relationships are unknown.
- Numerical simulations matching the run-out observed showed the material parameters to be ($\mu$ of 600 pa.s and $\tau_y$ of 150 kPa) based on trial and error to match the run-out. Rheological measurements showed ($\mu$ of 1.5 pa.s and $\tau_y$ of 461 kPa at $I_L=1.16$).
	- There is an order of magnitude difference in viscosity
	- The equivalent fluid approximation using constant parameters does not capture the run-out response accurately.


![Relation between $I_L$ and Su](https://raw.githubusercontent.com/kks32-docs/notes/main/submarine-slides/numerical-analysis-submarine-critical-state/liquidity-index-su.png)
> Relation between $I_L$ and Su


![Modeling of phase transition due to water entrainment](https://raw.githubusercontent.com/kks32-docs/notes/main/submarine-slides/numerical-analysis-submarine-critical-state/submarine-phase-transition-critical-state.png)
> Modeling of phase transition due to water entrainment

