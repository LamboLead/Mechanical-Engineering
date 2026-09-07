---
id: s6tlrnz1grsqyf4cj2fq40o
title: Cizallado
desc: ''
updated: 1709588495559
created: 1709502038101
---

Es un **proceso de deformación de lámina** que consiste en el corte de un trozo (de cierta forma geométrica) de lámina sometiéndola a esfuerzos de corte utilizando un punzón y una matriz.

## Descripción del proceso

Este proceso utiliza una prensa para ejercer una fuerza sobre el punzón.

1. El proceso inicia con la formación de grietas en las orillas superior e inferior de la pieza de trabajo. Finalmente, estas grietas se encuentran una con otra y ocurre la separación completa.

   ![](/assets/images/2024-03-03-20-42-43.png)

## Parámetros del proceso de cizallado

En el proceso de cizallado es definido a partir de los siguientes parámetros:
- La forma del punzón y de la matriz.
- Velocidad de punzonado.
- Fuerza de punzonado.
- Lubricación.
- Holgura ($c$) entre el punzón y la matriz.

A continuación se profundiza en algunos de ellos:

### Fuerza de punzonado

Es la fuerza requerida para punzonar, y es producto de la resistencia al cortante de la hoja metálica y el área total cizallada a lo largo de la periferia. Es posible estimar la **fuerza máxima de punzonado ($F$)** con:

(revisar de la página 459 de fundamentos de Manufactura Moderna)

$$
  F = 0.77TL\sigma_{max}
$$

Con:
- $T$: Espesor de la hoja.
- $L$: Longitud o perímetro de cizallado.
- $\sigma_{max}$: Resistencia última a la tensión del material.

> Además de la fueza de punzonado, existe una segunda fuerza en el proceso requerida para retirar el punzón de la hoja durante su carrera de retorno. Esta fuerza es difícil de estimar por los muchos factores involucrados en la operación.

### Holgura

(esto se encuentra en la página 459 de Fundamentos de Manufactura Moderna)

> Al aumentar la holgura, disminuyen la fuerza de punzonado y el desgaste de punzones y matrices.

El proceso 

(ver página 397 del libro de 'Procesos de Manufactura Moderna')