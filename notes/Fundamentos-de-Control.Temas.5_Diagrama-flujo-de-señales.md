---
id: 1oj1i945phpro2ooon602mq
title: 5 - Diagrama de flujo de señales
desc: ''
updated: 1681507043847
created: 1681422705202
---

Los _SFG_ son una versión simplificada de los diagramas de bloques.
Consiste en una red en la que los nodos se encuentran conectados por rama con **dirección** y **sentido**.

Cada nodo representa una variable del sistema, y cada rama conectada entre dos nodos actúa como multiplicador.

_(meter un diagrama de flujo de señales de ejemplo)_

**Nudo:** Punto que representa una variable o señal.
- Nodo de entrada fuerte: Nodo que solamente tiene ramas de salida. Corresponde a una variable independiente.
- Nodo de salida (pozo/sumidero): Nodo que tiene solamente ramas de entrada. Corresponde a una variable dependiente.
- Nodo mixto: Nodo que tiene tanto entradas como salidas.

**Ganancia:** Relación entre dos variables unidas por una rama. Es el cociente entre la salida y la entrada.
**Rama:** Segmento de línea con dirección y sentido que une dos nodos.
**Trayectoria:** Recorrido de ramas conectadas en el sentido de la flecha.
- Trayectoria abierta: Trayectoria que no se cruza con ningún nodo más de una vez.
- Trayectoria cerrada: Trayectoria que finaliza en el mismo nodo del cual partió, sin cruzar más de una vez por un nodo.
- Otra trayectoria: Trayectoria que cruza un nodo más de una vez, y finaliza en un nudo distinto del que se partió.
- Trayectoria directa: Trayectoria que empieza en un nodo de entrada y termina en uno de salida, sin atravesar un nodo más de una vez.  

**Lazo:** Trayectoria que se origina y termina en el mismo nodo, y donde ningún nodo se encuentra más de una vez (trayectoria cerrada).
- **Lazos disjuntos:** Son lazos que no tienen ningún nodo en común.
**Ganancia de trayectoria:** Es el producto de las ganancias de las ramas que atraviesa dicha trayectoria.
**Ganancia de lazo:** Es el producto de las transmitancias de las ramas del lazo.   

## Fórmula de ganancia de Mason

Esta fórmula se utiliza para determinar la relación entre una variable de entrada y una variable de salida.
$$
  Ganancia: \sum{P_K\Delta_K}
$$
Con:  
  $M$: Número de trayectorias directas que hay entre un nodo de salida y el nodo de entrada   
  $P_K$:Ganancia K-ésima de trayecto directo  
  $\Delta$:Determinante del gráfico.  
  $\Delta_K$:Se obtiene a partir de $\Delta$, quitando los lazos que tocan la trayectoria $\Delta_K$

## Ejercicio

Halle la función de transferencia del sistema descrito por el siguiente diagrama de flujo de señales:

