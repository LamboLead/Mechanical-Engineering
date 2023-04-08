---
id: i6rb18otpy9nt9ptdzbol8w
title: Ejercicio 2
desc: ''
updated: 1678850161572
created: 1678848827876
---

## Cálculos

Tomando la expresión que describe el comportamiento de la ganancia de un controlador PI, se tiene:

$$
  G(s) = K_P + \frac{K_i}{s} = \frac{R_2}{R_1} + \frac{1}{s}\bigg(\frac{1}{R_1c}\bigg)
$$

Igualando las constantes $K_I$, $K_P$ para hallar $R_2$, $R_1$, $c$ de acuerdo con la función de trasnferencia de un sistema de segundo orden con la planta del ejercicio anterior:

$$
  \begin{align}
  &K_P = \bigg(\frac{-2\tau ln(\epsilon)}{t_s} - 1\bigg) = \frac{R_2}{R_1}
  \\
  &K_I = \frac{\tau}{M}\bigg(\frac{ln(\epsilon)}{\rho t_s}\bigg)^2 = \frac{1}{R_1c}
  \end{align}
$$

Además, $t_s = 4\tau$

**Sistema amortiguado:**

Reemplazando los valores $t_s=0.15s \Rightarrow \tau=0.0375s, \epsilon=0.02, M=1.5, \rho=0.6$:

$$
  \Rightarrow \Bigg\lbrace \space
  \begin{align}
  &K_P = 0.637 = \frac{R_2}{R_1}
  \\
  &K_I = 47.2 = \frac{1}{R_1c}
  \end{align}
$$

Tomando $c = 4.7\mu F$:
$$
  \colorbox{yellow}{$R_1 = 4507.7\Omega \approx 4.5k\Omega$}
  , \space
  \colorbox{yellow}{$R_2 = 2871.44\Omega \approx 2.9k\Omega$}
$$

**Sistema sobreamortiguado:**

Reemplazando los valores $t_s=1.5s \Rightarrow \tau=0.375s, \epsilon=0.02, M=1.5, \rho=1.5$:

$$
  \Rightarrow \Bigg\lbrace \space
  \begin{align}
  &K_P = 0.637 = \frac{R_2}{R_1}
  \\
  &K_I = 0.756 = \frac{1}{R_1c}
  \end{align}
$$

Tomando $c = 4.7\mu F$:
$$
  \colorbox{yellow}{$R_1 = 179334.5\Omega \approx 180k\Omega$}
  , \space
  \colorbox{yellow}{$R_2 = 281529.8\Omega \approx 280k\Omega$}
$$