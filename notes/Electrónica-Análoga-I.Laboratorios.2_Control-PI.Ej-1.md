---
id: z3c6mf8tivb97o9un1lzqi1
title: Ejercicio 1
desc: ''
updated: 1678590644861
created: 1678563398044
---

## Cálculos

Se tiene la función de transferencia de un sistema de primer orden:

$$
  G(s) = \frac{M}{\tau s + 1}
$$

Para simular un sistema de primer orden, es necesario utilizar un OPAM integrador compensado acoplado con un inversor, cuya función de transferencia es:

$$
  G(s) = \frac{V_{out}}{V_{in}} = \frac{R_x/R}{1 + R_xcs}
$$

Igualando ambas funciones y operando para hallar $R_x, R$:

$$
  G(s) = \frac{R_x/R}{1 + R_xcs} = \frac{M}{\tau s + 1}
$$
$$
  \Rightarrow \Bigg\lbrace \space
  \begin{align}
  &\frac{R_x}{R} = M
  \\
  &R_xc = \tau
  \end{align}
$$
Operando y reemplazando:
$$
  \Rightarrow \colorbox{orange}{$R_x = \tau/c$}
  , \space
  \colorbox{orange}{$R = \frac{\tau/c}{M}$}
$$

Tomando los siguientes valores:
$$
  c = 4.7\mu F\\
  \tau = 0.13s\\
  M = 1.5
$$
Se obtiene:
$$
  \colorbox{orange}{$R_x = 27659.6\Omega \approx 28k\Omega$}
  , \space
  \colorbox{orange}{$R = 18439,7\Omega \approx 18k\Omega$}
$$