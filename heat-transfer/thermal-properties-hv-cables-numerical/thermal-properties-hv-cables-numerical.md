## Effect of Sediment Properties on the Thermal Performance of Submarine HV Cables

> Hughes, T. J., Henstock, T. J., Pilgrim, J. A., Dix, J. K., Gernon, T. M., & Thompson, C. E. (2015). Effect of sediment properties on the thermal performance of submarine HV cables. _IEEE Transactions on Power Delivery_, _30_(6), 2443-2450.

[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7029130)

> Keywords: #conduction-convection #numerical #finite-difference


### Research questions
-   How different properties of sediments affect heat transfer properties.

-   What is the difference between terrestrial and marine buried cables and their heat transfer?
>  On land where high windspeeds facilitate the transfer of heat from the soil to the air, a higher wind speed results in a better correlation to a convective condition.
    
### Future research / unanswered questions

-   What type of soil predominates the top few meters in Gulf of Mexico and around the US?
      
-   Plot the profile of temperature and velocity variations with depth
    
-   Permeability and porosity influence the thermal regimes how do we correlate these two properties correctly?
    
-   Plot temperature changes against permeability incrementing permeability $K_{i+1} = K_i \times 10^{0.2}$
    
-   Plot conduction vs convective flux boundary for different permeability
    
-   Compare the conduction-convection regime with the Re

-   How do we estimate if conduction has transformed to convection?
> A regime change can be identified based on the difference in temperature between radial directions and at the top. If it exceed a critical percentage (say 20%), we estimate this to be convective behavior.

### Assumptions and methods
-   Waterbody acts as a heat sink taking heat away from the surface - this acts like an isothermal boundary
-   The PDE is a time-independent coupled fluid & heat transfer equation.

-   Bulk thermal conductivity is a weighted summation of thermal conductivity and porosity
-   Boundary Condition:
	-   Sides & bottom: No fluid and heat flux $n \cdot u = 0$ and $n \cdot (-\lambda \Delta T) = 0$.
    -   Top: constant pressure common on buoyancy flow problem. **What pressure should we apply?**
    -   Top: Similar to water-cooled interface use $n \cdot (-\lambda \Delta T) = h (T - T_0)$. $T_0$ temp of the water and $h$ is the heat transfer coefficient.

### Main findings
-   Permeability, thermal conductivity and burial depth affect the heat transfer regime. 
-   Permeability controls the velocity of the fluid flow which dictates the convective flux
-   At low permeability $K < 10E-14 m^2$
    -   Temp field is isotropic
    -   Some anisotropy near the water surface as it acts as a heat sink
    
-   At high permeability $K > 10E-10 m^2$
    -   Buoyancy force drive fluid circulation
    -   Heat transfer is asymmetric and transferred up through convection. 
    
-   Burial depth:
    -   Affects distance to seawater (heat sink)
    -   Cable temperature can be increased by deeper burial depth
    -   Depth of burial due to currents and migration produce a 5m difference in a year.
    -   When convection happens burial depth has no effect on temp vs permeability
    
-   IEC60287 standards for terrestrial burials and depend on backfill soil properties and only use conduction mode for heat transfer.

![Effect of burial depth](https://raw.githubusercontent.com/kks32-docs/notes/main/heat-transfer/thermal-properties-hv-cables-numerical/conduction-convection-burial.png)

> Dependence of the conductor temperature on cable burial depth. In each case, the solid phase thermal conductivity is 1 $\frac{W}{m\cdot K }$

![Conduction vs. Convection](https://raw.githubusercontent.com/kks32-docs/notes/main/heat-transfer/thermal-properties-hv-cables-numerical/conduction-convection.png)
