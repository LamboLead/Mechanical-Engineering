---
id: qi4g0ofg326hbekeha0v8yg
title: 3 - Inflación e IPC
desc: ''
updated: 1691544222794
created: 1690845499699
---

## Inflación

La inflación es una métrica que describe el cambio general del precio de los bienes y servicios en un periodo determinado. Mide el nivel general de los precios en la economía.

La inflación sirve para:
- Calcular cambios en el valor de una canasta típica de consumo y **evaluar cambios en el costo de vida**.
- Ajustar el **salario mínimo** y mantener el poder adquisitivo de los hogares.
- Comparar valores en pesos a lo largo de diferentes periodos.

> La inflación es la **variación porcentual** en el nivel general de precios.

> El **Banco de la República** es la entidad que, entre otras, mide el nivel de calidad de vida de las personas. Una de sus tareas es la de someter la inflación en niveles no mayores al 3%.

### Deflactor

Es posible tener una noción de la inflación a partir del [[PIB nominal y real|macroeconomía.1_Datos-Macroeconómicos.1_PIB#3-pib-nominal-y-real]].

$$
  Deflactor = \frac{PIB_{nominal}}{PIB_{real}} * 100
$$

> El deflactor del PIB mide el precio de la producción en relación con el precio que tenía en el año base.

## IPC (Índice de Precios al Consumidor)

Es una métrica que **mide el nivel general de precios** de una canasta base y evaluar cambios en el coste de vida.

Es calculado por el DANE a partir de grandes categorías de productos y servicios contratados en Colombia, dándole una ponderación fija a cada bien presente en la canasta base definida.

> El IPC para cada año requiere de una canasta base correspondiente a dicho año.

**Cálculo de la canasta base:** Considere que un país consume los productos $x$, $y$, $z$. Tomando los costos como los de un año base, la canasta base se calcula de la siguiente manera:

$$
  Canasta = P_xC_{x,base} + P_yC_{y,base} + P_zC_{z,base}
$$

> Las cantidades para la canasta base se dejan fijas en el año base. **Esta canasta solamente tiene en cuenta los productos consumidos nacionalmente**.

**Cálculo del IPC:** Teniendo los valores de la canasta en el periodo de interés y la canasta del periodo base, el IPC se calcula así:

$$
  IPC = \frac{C_P}{C_{base}} * 100
$$

Con:
- $C_P$: Costo de la canasta en el periodo a calcular   
- $C_{base}$: Costo de la canasta en el año base

> El IPC puede sobreestimar la inflación en los siguientes casos:
> - **Sesgo de sustitución:** Si un bien eleva mucho su precio, el consumidor final puede sustituirlo por un bien con un precio más reducido. Esto puede reflejarse en el IPC con que el costo de vida no aumenta tanto, ya que el bien con mayor valor no fue consumido en gran medida.
> **Introducción de bienes nuevos:** Si se introducen más bienes en el mercado, aumenta el bienestar de las personas; pero esto no traduce en un mayor IPC.

## Deflactor vs. IPC para el cálculo de la inflación

El deflactor del PIB mide los precios de los bienes y servicios _nacionales producidos_, mientras que el IPC mide los precios de bienes y servicios _nacionales e importados consumidos_.

Además el IPC asigna una ponderación fija, mientras que el deflactor asigna una ponderación variable.

**Inflación básica:** Es la inflación calculada sin tener en cuenta el valor del precio de elementos no regulados.

## Cálculo de la inflación

La inflación $\pi$ puede calcularse a partir de los siguientes métodos:

### 1. Deflactor

Si $n$ es el año sobre el cual se quiere calcular la inflación, entonces:

$$
  \pi = \frac{Deflactor_n - Deflactor_{n-1}}{Deflactor_{n-1}} * 100 \space[\%]
$$

### 2. IPC

Si $n$ es el año sobre el cual se quiere calcular la inflación, entonces:

$$
  \pi = \frac{IPC_n - IPC_{n-1}}{IPC_{n-1}} *100 \space[\%]
$$

> Si bien el resultado de la inflación es similar siendo calculado con el deflactor o el IPC, tenga en cuenta que:
>
> **El deflactor es calculado a partir del PIB real y nominal, es decir, a partir de la cantidad de bienes producidos en un año.**
> 
> **El IPC es calculado a partir de los bienes consumidos producidos nacional e internacionalmente.**