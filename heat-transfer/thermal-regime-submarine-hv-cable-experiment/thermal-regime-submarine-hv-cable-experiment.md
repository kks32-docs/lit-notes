## The thermal regime around buried submarine high-voltage cables
> Emeana, C. J., Hughes, T. J., Dix, J. K., Gernon, T. M., Henstock, T. J., Thompson, C. E. L., & Pilgrim, J. A. (2016). The thermal regime around buried submarine high-voltage cables. _Geophysical Journal International_, _206_(2), 1051-1064.

[Paper](https://academic.oup.com/gji/article/206/2/1051/2606019)

> Keywords: #hv-cables #experiments #1g #conduction-convection

### Research questions

-  What is the relation between grain size and permeability?
    
-  What is the condition for switching from conduction to convection?
    
-  What are the factors affecting the thermal regime change?
> Permeability, temperature gradient 

-   What are the thermal regimes and heat transfer mechanisms?
> Conduction and convection

### Future research / unanswered questions
-   Plot dT/dt evolution with time to show the evolution towards steady-state
    
-   Turn-off convection in the process and compare the profiles between conduction and convection - numerically.

-   Normalize the temperature to maximum temperature and plot against the radial distribution. Can we find a characteristic curve such that the deviation from this would mean convection?

-   Find the transition line between conduction and convection. 

-   How does burial depth influence the transition between conduction and convection?


### Main findings
-   Lower temperature in the pipe requires a longer time to reach steady-state
 
-   Low permeability (1E-13 $m^2$) soil only showed conduction for temp up to 60C above ambient
    
-   Med permeability (5E-11 $m^2$):
    -   Conduction < 10$^\circ$ C
    -   Convection > 19$^\circ$ C

-   Conduction shows a symmetric distribution of heat around source
    
-   High permeability (1E-10 $m^2$)
	-   Even at low temp of 7C asymmetric heat distribution is observed.
    
-   At high permeability, convective drive results in a reduction in heat compared to what would be expected from a purely conductive flow. This behavior is only observed in high permeability conditions.
      

Submarine High Voltage (HV) cables used in renewable power transmission are typically buried at a depth of 1-2m.

The maximum operating temperature is 90$^\circ$C and leads to a surface cable temperature of 70$^\circ$C. This kind of high temperature is only observed at a depth of 2.8 km under normal conditions in subsea. There is little knowledge between the thermal properties of marine sediments and the current that may be reliably carried - A balance between resistive heating within the cable and how efficiently heat is lost to the environment.  

Hughes (2005) observed both conduction and convection behavior in fully saturated sediments. Hughes also observed that permeability is the controlling factor in the transition from conduction to convection as permeability increases to the range of $10^{-11}$ to $10^{-12} m^2$. 

If conductive heat transfer occurs then the greater efficiency may allow significantly higher currents to be carried by the cable - is this good? **How can we carry more current when it is lost due to heat by convection?**

Permeability is evaluated using the Carman-Kozeny equation.

Plotting $dT/dt$ evolution shows a steady state is reached after 5 days and 1.7 days for 7$^\circ$ C and 18$^\circ$ C, lower temperature requires a longer time to reach steady state.

The difference in temperature distribution is normalized to a distribution at an arbitrary temperature of 60$^\circ$ C. **Why this value is chosen is unclear.**

Carslaw & Jaeger (1959) defined steady-state conduction to have an approximately radial distribution of heat with negligible heat generation. However, at the onset of convective flow the points on the radial plots begin to scatter.  

Emeena et al plotted a histogram of std deviation of temp radially and uses an arbitrary critical value of 0.06 to identify convective boundary and this is the average std dev at 19$^\circ$ C.

![conduction-convection regime](https://raw.githubusercontent.com/kks32-docs/notes/main/heat-transfer/thermal-properties-seabed-subsea-flowlines/conduction-convection.png)