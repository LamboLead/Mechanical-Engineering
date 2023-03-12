---
id: 0ffzv1uj0as46i7l1dh6qg6
title: Ejercicio 1
desc: ''
updated: 1677811398061
created: 1677091751606
---

## Cálculos

<!-- ![](/assets/images/2023-02-22-13-55-16.png) -->

Tomando la fórmula general del OPAM restador:
$$
  V_o = -\frac{R_2}{R_1}V_1 + \Big(\frac{R_B}{R_A + R_B} \Big)\Big(1 + \frac{R_2}{R_1}\Big)V_2
$$
Analizando el circuito $V_{o,2} = 3V_i - 2$ y tomando $R_1 = R_A$, $R_2 = R_B$:
$$
  V_{o,2} = \frac{R_2}{R_1}(V_2-V_1) = \frac{R_2}{R_1}(V_2) - \frac{R_2}{R_1}(V_1)
$$
$$
  \Rightarrow
  \colorbox{orange}{$R_2 = 3R_1$}
  ,\space
  \colorbox{orange}{$V_1 = 0.67V$}
$$

Analizando el circuito $V_{o,1} = 2V_i - 3$, con $R_1 \not= R_A$, $R_2 \not= R_B, V_1 = 0.67V$:
$$
  V_o = -\frac{R_2}{R_1}V_1 + \Big(\frac{R_B}{R_A + R_B} \Big)\Big(1 + \frac{R_2}{R_1}\Big)V_2
  \\
  \Rightarrow \Big(\frac{R_B}{R_A+R_B}\Big)\Big(1+\frac{R_2}{R_1}\Big) = 2
$$
$$
  \Rightarrow
  \colorbox{orange}{$R_2 = (9/2)R_1$}
  ,\space
  \colorbox{orange}{$R_B = (4/7)R_A$}
$$
Entonces, se toman los siguientes valores:  
- Para $V_{o,1} = 2V_i - 3$:
  $$
    R_1 = 1k\Omega\\
    R_2 = 4.5k\Omega\\
    R_A = 3.5k\Omega\\
    R_B = 2k\Omega\\
    V_1 = 0.67V
  $$
- Para $V_{o,2} = 3V_i - 2$:
$$
  R_1 = R_A = 1k\Omega\\
  R_2 = R_B = 3k\Omega\\
  V_1 = 0.67V
$$

## Simulación

Ver diagrama [[aquí | D:\Documentos\Ingeniería mecánica\Semestre VIII\Electrónica Análoga I\Laboratorio\2_Amplificadores-operacionales-básicos\Ej-1.psimsch]]   
Ver simulación [[aquí | D:\Documentos\Ingeniería mecánica\Semestre VIII\Electrónica Análoga I\Laboratorio\2_Amplificadores-operacionales-básicos\Ej-1.smv]]

![](/assets/images/2023-02-22-13-50-15.png)
