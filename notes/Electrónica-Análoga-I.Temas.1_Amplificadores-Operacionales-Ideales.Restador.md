---
id: ka68prlgl3p6gnjpfocgx82
title: OPAM Restador
desc: ''
updated: 1677085434660
created: 1676311521843
---

El amplificador operacional restador permite restar dos señales de voltaje.

![](/assets/images/![](/assets/images/2023-02-13-14-09-02.png)%20%20.png)   
_Figura 1: Esquema de un amplificador operacional restador_

Si $R_1 \not= R_A \land R_2 \not= R_B$:
$$
  V_{out} = -\frac{R_2}{R_1}V_1 + \Big(\frac{R_B}{R_A + R_B} \Big)\Big(1 + \frac{R_2}{R_1}\Big)V_2
$$

Si $R_1 = R_A \land R_2 = R_B$:
$$
  V_{out} = \frac{R_2}{R_1}(V_2 - V_1)
$$

## Análisis

![](/assets/images/2023-02-13-14-19-27.png)
![](/assets/images/2023-02-13-14-19-38.png)
_Figura 2: Análisis de un OPAM restador_