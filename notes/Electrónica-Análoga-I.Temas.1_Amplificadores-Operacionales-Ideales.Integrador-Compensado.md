---
id: nxwo08aiasu3ifmq2i58qhh
title: OPAM Integrador Compensado
desc: ''
updated: 1677099563271
created: 1677098780831
---

Este amplificador operacional integra la señal de voltaje de entrada, sin importar si ésta está centrada en cero o no.

![](/assets/images/2023-02-22-15-53-15.png)   
_Figura 1: Diagrama de un OPAM integrador compensado_

$$
  V_{out} = -\frac{1}{Rc}\int{V_{in}dt}
$$

Con $R_xcs >> 1$, siendo $s$ la frecuencia de la señal de entrada

> $R_x$ debe ser grande, pero no lo suficiente como para que el OPAM se sature con la señal de DC.
>
> Una alta capacitancia $c$ o una alta frecuencia $s$ ayudarán a que el OPAM se comporte como un integrador puro.

## Análisis

![](/assets/images/2023-02-22-15-56-06.png)
_Figura 2: Análisis de un OPAM integrador compensado en frecuencia_