---
id: lh3djvio5andphr6dvu1ovw
title: '3 - Pumps and valves'
desc: ''
updated: 1746408742129
created: 1746404449428
---

1. An expression relating the flow rate through an orifice to the pressure drop across it may be derived from Bernoulli's equation

  $$Q=A_0\sqrt{\frac{2}{\rho}(P_1-P_2)}$$

  This expression does not provide accurate results for fluid power applications, but a slight modification allows for increased accuracy. What is the corrected expression, what is the name of the additional term, and what purpose does the additional term serve?

  **Ans:** The additional term missing from the previous equation is the _discharge coefficient_ $C_d$. This term takes into account the geometric parameters regarding the orifice (like its aperture, its shape, etc); so, the new, more accurate expression for fluid flow should be:

  $$Q=C_dA_0\sqrt{\frac{2}{\rho}(P_1-P_2)}$$; with $0.6 \leq C_d \leq 1$.

2. The data sheet of an orifice lists the discharge coeffcient to be 1.05. Is there anything strange about this claim? Explain.

  **Ans:** The discharge coefficient is the relationship between the orifice's area and the actual area cross-section area that the flow has after the flow has passed over the orifice. The cross-section area of the fluid is never more than the area of the orifice it has passed through, so a $C_d = 1.05$ is unfeasible.

3. Hydraulic fluid ($\rho = 840 kg/m^3$) passes through a knife-edged orifice, characterized by $C_d = 0.6$, at a volumetric flow rate of 2 liters per minute. If the pressure drop across the orifice is 2 kPa, what is the cross sectional area of the orifice?

  **Ans:** 

4. Two knife-edged orifices have the same cross sectional area, $A_0$, but one orifice has a circular cross section and the other has a square cross section.
   1. Will the pressure drop be the same for these two orifices if the fluid is inviscid?
   2. Will the pressure drop be the same for these two orifices if the fluid is viscous?

5. A company uses the correlation $\Delta P=5Q^2$ to predict the pressure drop across one of their flow control valves. What is the orifice coefficient $K$ associated with the control orifice?

6. Earlier in the course we defined force and volumetric efficiencies for a cylinder. What are the analytical force and volumetric efficiencies for a pump?

7. A hydraulic motor with 85% total efficiency drives a 5 kW application. If the system power supply provides fluid at a rate of $3.155 \times 10^{-4}m^3/s$, what pressure is required to satisfy the application power requirement?

8. Empirical correlations for pump/motor efficiency are typically required for design purposes. Example correlations are presented in the Effciency and Pumping Theory lecture. Manipulate these two expressions to find the total efficiency, $\eta$, of a pump.
9.  What is flow ripple? What characteristics of a piston pump determine the frequency and amplitude of flow ripple?
10. A designer considers two mounting locations for a hydraulic filter: the first just before the reservoir on the return line, and the second between the reservoir and the pump. Which of these configurations is preferable? Explain.
11. The cracking pressure of a relief valve is the pressure drop required to unseat the main stage poppet. At the cracking pressure, the relief valve passes a negligible volumetric flow rate of hydraulic fluid. To increase the flow rate through the valve, the pressure drop must be increased. The increase in pressure drop (above that of the cracking pressure) required to achieve the valves rated flow rate is called the pressure override. Do you expect the pressure override for pilot-operated and direct-acting relief valves to be similar or different? Explain.