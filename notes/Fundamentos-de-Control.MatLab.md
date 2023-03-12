---
id: fjm2p0girmpfm0ka7sv01pu
title: MatLab
desc: ''
updated: 1677857455310
created: 1676729412896
---

Este es el conocimiento y la sintaxis básica necesaria para trabajar con MatLab en Fundamentos de Control.

---

## Funciones importantes

- tf: Defines the transfer function of a system
- pzmap: Pole-zero map of dynamic systems
- rlocus: Finds the roots of the system

**Ejercicio:** Definir la siguiente función de transferencia en MatLab:
$$
  \frac{y(s)}{U(s)} = \frac{x+7}{x^3 + 7x^2 + x}
$$

```matlab
  y = [1 7] % x + 7
  u = [1 7 1 0] % x^3 + 7x^2 + x + 0
  transferFunction = tf(num, den) % Defines the transfer function for 'y' and 'u'
  pzmap(syst) % Creates the s-plane for the transfer function
```