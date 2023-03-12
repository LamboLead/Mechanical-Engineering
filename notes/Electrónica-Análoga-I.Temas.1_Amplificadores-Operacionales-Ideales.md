---
id: r67sz5d9f61mp3avwb1hu8w
title: 1 - Amplificadores Operacionales Ideales
desc: ''
updated: 1676317726644
created: 1676300312615
---

Un amplificador operacional (OPAM) es un componente electrónico analógico que permite, a partir de una señal de voltaje de entrada, obtener una señal de voltaje diferente de acuerdo con su configuración.

![](/assets/images/2023-02-13-11-05-05.png)
_Figura 1: Diagrama de un amplificador operacional_

![](/assets/images/2023-02-13-13-08-23.png)
_Figura 2: Esquema del circuito dentro de un OPAM_ 

## El amplificador operacional ideal

### Condiciones ideales de un OPAM

1. Su impedancia de entrada tiende a infinito. Es decir, el consumo de corriente en los pines de entrada es igual a 0.  
  $$
    z_{in} \rightarrow \infty \Rightarrow i_{in} \rightarrow 0
  $$

2. Su impedancia de salida tiende a cero. Es decir, la tensión de salida no depende de la carga conectada a la salida (fuente ideal).
  $$
    z_{out} \rightarrow 0 
  $$
3. El OPAM puede procesar un ancho de banda infinito.
4. El OPAM opera en la zona lineal, y no se encuentra saturado.
5. La ganancia del OPAM tiende a infinito, por lo que la tensión de entrada tiende a cero.
  $$
    A_{v_0} \rightarrow \infty \Rightarrow v_A \rightarrow 0
  $$
6. Existe un corto virtual entre $in_1$ y $in_2$, por lo que no hay flujo de corriente entre ellos.

> Un corto virtual entre dos pines implica que ambos pines no hay un voltaje, y por lo tanto no hay flujo de corriente entre ellos, aunque físicamente estén conectados.

> El OPAM se encuentra saturado cuando el voltaje que provee energía al OPAM es menor que el voltaje de salida.

> Cuando el pin de salida se encuentra realimentado por el pin negativo, el OPAM opera en la zona lineal.

## Tips para el análisis de circuitos con OPAM

Si se quiere realizar el análisis de un circuito que contiene un OPAM, el método más sencillo es realizar un _**análisis por superposición**_

El **análisis por superposición** consiste en simplificar el circuito al sumar los voltajes de cada una de las fuentes presentes allí, cortocircuitando las fuentes de voltaje restantes.   
Una vez se obtenga el valor de $V_{out, n}$ para cada fuente, se suman todos los voltajes resultantes.

$$
  V_{out} = V_{out,1} + V_{out,2} + ... + V_{out,n}
$$

Ver el [[análisis de un OPAM restador | Electrónica-Análoga-I.Temas.1_Amplificadores-Operacionales-Ideales.Restador#análisis]] como ejemplo.