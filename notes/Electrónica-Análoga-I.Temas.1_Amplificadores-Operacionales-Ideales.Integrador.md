---
id: 1bf8q61s8m8y98lgo121rf4
title: OPAM Integrador
desc: ''
updated: 1677098851234
created: 1676926596725
---

Este amplificador operacional integra la señal de voltaje de entrada.

> La señal de entrada debe estar centrada en cero para evitar la saturación del amplificador

![](/assets/images/2023-02-20-18-43-45.png)   
_Figura 1: Diagrama de un OPAM integrador_

$$
  V_{out} = -\frac{1}{Rc}\int{V_{in}dt}+C
$$

## Análisis

Es posible realizar el análisis de este OPAM en el tiempo o en frecuencia

### Análisis en el tiempo

![](/assets/images/2023-02-20-16-35-29.png)
_Figura 2: Análisis de un OPAM integrador en el tiempo_

### Análisis en frecuencia

![](/assets/images/2023-02-20-18-41-44.png)
_Figura 3: Análisis de un OPAM integrador en frecuencia_