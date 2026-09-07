---
id: 2al1w9wojxfbxwpu2ywy52v
title: 1 - Procesos de deformación
desc: ''
updated: 1709813302113
created: 1708397296478
---

Los procesos de deformación modifican la forma de cierta materia prima haciendo uso de esfuerzos de tensión y compresión sobre la misma.

**Ventajas:**

- Los procesos de deformación (especialmente el **forjado**) aportan propiedades mecánicas superiores que otros tipos de procesos, especialmente aquellas propiedades relacionadas con la resistencia a la fatiga.
- Los procesos de deformación son favorables para la producción en masa, por lo que el costo por pieza es bajo respecto a otro tipo de procesos.

## Clasificación de los procesos de deformación

Los procesos de formado pueden clasificarse en:

### Procesos de deformación de volumen
Son aquellos procesos tales que deforman el material en su totalidad. Se caracterizan por grandes cambios de forma, y su materia prima presenta una relación área superficial/volumen relativamente pequeña.  
Entre estos se encuentran:
  - Laminado (a partir de palanquilla)
  - Forjado
  - Extrusión
  - Trefilado

### Procesos de deformación de lámina
Son aquellos procesos tales que la deformación se presenta únicamente en el contacto de la pieza con la herramienta.

**Ventajas:**
- Alta resistencia y rigidez.
- Buena precisión dimensional (del orden de décimas de milímetro).
- Muy buen acabado superficial.
- Grandes capacidades de producción a un costo bajo.

**Procesos:**
  - Embutición
  - Laminado (a partir de planchón o láminas)
  - Martillado
  - Rechazado
  - Estampado (cizallado, repujado, doblado, rebordeado, acuñado)...

> Los procesos de deformación de lámina son procesos de altísimo valor agregado para las piezas, con costos relativamente bajos.

> Es posible modificar diversas variables entre los procesos de deformación: La **temperatura del material**, la **velocidad de deformación**...

## Comportamiento del material en procesos de deformación

En los procesos de deformación se quiere llegar a la región plástica en la curva esfuerzo-deformación.

### Curva de fluencia

**Región plástica:** Es la región en la curva esfuerzo-deformación de metales en la cual el material se deforma plásticamente, es decir, permanentemente.

La **curva de fluencia** expresa el comportamiento del metal en la región plástica, es decir, se utiliza para determinar nuevos valores para el esfuerzo de fluencia después de un proceso de deformación, describe el endurecimiento por deformación del metal cuando se deforma plásticamente en términos de tensión equivalente, tasa de tensión equivalente y temperatura.

La curva de fluencia está gobernada por la siguiente ecuación:

$$
  Y_f = K\epsilon^n \space [MPa; lb/in^2]
$$

Con:
- $Y_f$: Esfuerzo real de fluencia
- $\epsilon$: Deformación real del material
- $K$: Coeficiente de resistencia $[MPa]$
- $n$: Exponente de endurecimiento por deformación

La _curva de fluencia_ también indica el _esfuerzo de fluencia_ del metal, la _resistencia_ que determina las fuerzas y la _potencia_ requerida para realizar cierta operación de formado.

#### **Esfuerzo de fluencia**

El **esfuerzo de fluencia o de flujo ($Y_f$)** es el valor instantáneo del esfuerzo requerido para continuar con la deformación del material (o mantenerlo 'fluyendo') una vez se inicia un proceso de deformación. En otras palabras, es la resistencia a la fluencia del metal en función de su deformación, expresado como:

$$
  Y_f = K\epsilon^n \space [MPa; lb/in^2]
$$

**Esfuerzo de fluencia promedio ($\bar{Y_f}$):** Es el valor promedio de los esfuerzos sobre la curva $\sigma-\epsilon$ desde el comienzo de la deformación hasta el valor máximo que ocurre durante el proceso.

$$
  \bar{Y_f} = \frac{K\epsilon^n}{1+n} \space [Mpa; lb/in^2]
$$

Con:
- $\epsilon$: Deformación máxima durante el proceso de deformación.

> Los valores de $K$ y $n$ son de vital importancia para el cálculo de la deformación final para cada proceso de deformación, y determinar el esfuerzo de fluencia promedio al que se sujeta el material durante la operación.

## Temperatura del material en procesos de deformación

Para cualquier metal, los valores de $K$ y $n$ dependen de su temperatura. Por lo tanto, se puede reducir la potencia y fuerza necesarias para cualquier operación de deformación con un incremento en la temperatura del material.

> Para cualquier metal, tanto la resistencia como el endurecimiento por deformación se ven reducidos a altas temperaturas, mientras que su ductilidad se incrementará.

Existen tres rangos de temperatura: Trabajo en frío, caliente por debajo, o caliente por encima de la temperatura de recristalización.

### Trabajo en frío

Es el formado del metal que se realiza a temperatura ambiente o ligeramente superior. Al realizarse a dicha temperatura, no se produce una capa de óxido (conocido como _calamina_) en la pieza de trabajo.

**Ventajas:**
- Proporciona tolerancias más estrechas en la pieza.
- Brinda un buen acabado en la superficie de la pieza.
- Aumenta la resistencia y dureza de la pieza, gracias al endurecimiento por deformación.
- Proporciona propiedades direccionales convenientes en el producto resultante.
- Se ahorran costos energéticos y de herramienta relacionada al calentamiento de la pieza.

**Desventajas:**
- Se requiere una mayor potencia o fuerza para realizar la operación.
- La pieza debe estar libre de suciedades e incrustaciones para un formado óptimo.
- La ductilidad y el endurecimiento de la pieza limitan la cantidad de formado que puede realizarse sobre la pieza (incluso requiriendo de un recocido para realizar formados posteriores).

### Trabajo en caliente (por debajo de temp. de recristalización)

Implica la deformación a temperaturas en el rango de $T = 0.3T_m$, donde $T_m$ es el punto de fusión del metal en cuestión. En este rango, la pieza presenta menores resistencia y endurecimiento por deformación, así como mayor ductilidad.

**Ventajas:**
- Se requieren fuerzas más bajas y menores requerimientos de potencia respecto al formado en frío.
- Son posibles deformaciones más complejas e intrincadas.
- Es posible eliminar o reducir la necesidad del recocido para futuros trabajos.

### Trabajo en caliente (por encima de temp. de recristalización)

Implica la deformación a temperaturas mayores a la temperatura de recristalización del material, pero no tan cercanas a su temperatura de fusión, ya que se quiere evitar la fusión en algunas partes de la misma. Entonces, la temperatura se ubica en el rango $0.5T_m > T > 0.75T_m$.

Ya que a dichas temperaturas el metal posee un coeficiente de resistencia $K$ mucho menor que a temperatura ambiente, $n$ es prácticamente cero (en teoría) y la ductilidad del material se incrementa de manera significativa, se producen deformaciones plásticas sustanciales del material.

**Ventajas:**
- Es posible alterar la forma de la pieza de forma significativa.
- Se requiere menor fuerza y potencia para deformar el material.
- Un incremento en la ductilidad del material permite una deformación que, en frío, provocaría su fractura.
- Las propiedades de resistencia son generalmente isotrópicas, gracias a una ausencia de una estructura orientada de granos.

Además, este trabajo no produce un fortalecimiento de la pieza; característica deseable para subsecuentes procesos de formado.

**Desventajas:**
- Menor precisión dimensional y peor acabado superficial.
- Mayores requerimientos de energía (para calentar la pieza).
- Oxidación de la superficie de trabajo.
- Menor duración de las herramientas.

### Formado isotérmico

Consiste en los procesos de formación que precalientan el herramental a la misma temperatura de trabajo de los materiales a trabajar, para evitar que se endurezcan. Estos procesos se utiliza para materiales que poseen una dureza considerable, incluso por encima de la temperatura de recristalización (usualmente forjado).

## Velocidad de deformación

En los trabajos en caliente por encima de la temperatura de recristalización, los metales presentan una sensibilidad a la **velocidad de deformación**. Dicha propiedad está definida por:

$$
  \dot{\epsilon} = \frac{v}{h} \space \bigg[\frac{m}{s\cdot m} = \frac{1}{s}; \space \frac{in}{s\cdot in}\bigg]
$$

Con:
- $\dot{\epsilon}$: Velocidad de deformación real.
- $v$: Rapidez de deformación.
- $h$: Altura instantánea de la pieza de0 trabajo que se deforma $[m; in]$

**Sensibilidad a la velocidad de deformación:** Es el efecto que posee la velocidad de deformación sobre las propiedades de resistencia en la pieza a trabajar. Es decir, _al aumentar la velocidad de deformación, se incrementa la resistencia a la deformación_.

Dicha sensibilidad se representa usualmente como una línea recta en una gráfica log-log, definida por la siguiente expresión:

$$
  Y_f = C\dot{\epsilon}^m
$$

Con:
- $C$: Constante de resistencia (similar al coeficiente de resistencia en la ecuación de la curva de fluencia).
- $m$: Exponente de sensibilidad a la velocidad de deformación.

> Al incrementar la temperatura, decrece el valor de $C$ (consistente con su efecto sobre $K$ en la ecuación de curva de fluencia) y aumenta el valor de $m$.

**Esfuerzo de flujo (en función de deformación y velocidad de deformación):**

Por lo anterior, _una expresión más completa para el esfuerzo de fluencia_ sería la siguiente:

$$
  Y_f = A\epsilon^n\dot{\epsilon}^m
$$

Con:
- $A$: Coeficiente de resistencia que combina los efectos de $K$ y $C$

### Rangos de deformación y velocidad de deformación

En **procesos de deformación de volumen** se consiguen:
- Deformación: $\bar{\epsilon} \lesssim 3.0 - 4.0$
- Velocidad de deformación: $\bar{\dot{\epsilon}} \lesssim 10^2 \space s^{-1}$

En **procesos de deformación de lámina** se consiguen:
- Deformación: $\bar{\epsilon} \lesssim 1.0$
- Velocidad de deformación: $\bar{\dot{\epsilon}} \lesssim 10^{-1} \space s^{-1}$

## Ejemplos: Curvas de flujo

