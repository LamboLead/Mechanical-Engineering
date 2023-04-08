---
id: jfw23a7w2pb50l7135as2u3
title: Ejercicio 1
desc: ''
updated: 1680825567202
created: 1680815148350
---
## Cálculos

Hallando las expresiones de $V_x$ y $V_C$:
$$
  \begin{align}
  &V_x = 10\Big(\frac{R_2}{R_2 + R_1}\Big)
  \\
  &V_C = 10(1-e^{-t/R_CC}); \space R_C = 10^3 + P_1
  \end{align}
$$

Hallando el valor de $V_C$ en el que el temporizador empieza a actuar, con $R_1 = R_2$:
$$
  \begin{align}
  V_x = V_C &\Rightarrow 10\Big(\frac{R_1}{R_1 + R_1}\Big) = 10(1-e^{-t/R_CC})
  \\
  &\Rightarrow \frac{-t}{R_CC} = ln(1/2)
  \\
  &\Rightarrow t = ln(2)R_CC
  \end{align}
$$

Despejando $C$ y reemplazando $R_C = 40k\Omega$, $t = 24s$:
$$
  C = \frac{t}{ln(2)R_C}
  \Rightarrow
  \colorbox{orange}{$C \approx 8.45E-04F = 845\mu F$}
$$
Para esta configuración, se tomará:
$$
  \colorbox{orange}{$ C = 1000\mu F$}, \colorbox{orange}{$P_1 = 40k\Omega$}, \colorbox{orange}{$R_1 = R_2 = 1k\Omega$}
$$