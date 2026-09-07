---
id: ej6m3o02ovzdxch235gt2tr
title: Foro 
desc: ''
updated: 1733839719569
created: 1733779867046
---

**Título:** _Contact of nominally flat surfaces_

---

## Introducción

Se tiene la suposición de que el área de contacto depende de la deformación plástica de las impurezas más grandes. Una teoría más avanzada fue propuesta por Archard, y dice que el área de contacto puede ser proporcional a la carga aplicada

¿Que describe el paper?

- Una nueva teoría de contacto elástico, más relacionada con las superficies reales de los objetos. Dicha teoría demestra que _la deformación en contacto depende de la topografía de la superficie_.
- Se define una propiedad de _dureza de contacto elastico_, que depende de de las propiedades elásticas y la topografía de la superficie.
- Se muestra un nuevo instrumento para la medición de la topografía de la superficie, y se muestran los resultados de las mediciones de los radios de curvatura de las asperezas.

## Modelo matemático

Considere un plano en contacto con una superficie nominalmente plana con varias asperezas que cuya punta puede asumirse como esférica.

Suposiciones:
- Todas las asperezas tienen el mismo radio $\beta$ en la punta
- Las alturas de las asperezas varían aleatoriamente.

![](/assets/images/2024-12-09-18-03-16.png)

Se tienen las siguientes variables:
- **Radio de contacto:**
- **Acomodamiento ($w$):** Distancia que los puntos por fuera de la zona de deformación se mueven durante la deformación

### Distribución exponencial de la altura de las asperezas

En este caso, las alturas siguen una distribución exponencial $\phi^*(s) = e^{-s}$. Entonces:

- $n = \eta Ae^{-h}$.
- $G = \pi^{1/2}\mu\rho^-1(\beta\sigma)^{1/2}Ae^{-h}$.
- ...

Eliminando la separación $h$ entre las superficies se descubre que _existe una proporcionalidad exacta entre la carga y el número de puntos de contacto, la conductancia y el área de contacto_. Esto quiere decir que el tamaño promedio de los puntos de contacto y la presión de contacto son independientes de la carga.

**Precisión:** La distribución exponencial es una aproximación aceptable para el 25% mayor del total de las asperezas de la mayoría de superficies. 

> En la distribución exponencial el tamaño promedio de contacto se mantiene constante ya que, a medida que la carga aumenta, por supuesto que el tamaño de los puntos que ya se encuentran en contacto aumenta, pero a su vez nuevos puntos se forman, lo que lleva a mantener el promedio en dicho tamaño.

### Distribución gaussiana de la altura de las asperezas

Para la gran mayoría de superficies, la distribución de las alturas de las asperezas es Gaussiana, por lo tanto:

$$
\phi^*(s) = \frac{1}{\sqrt{2\pi}}e^{-s^2/2}
$$

## Conceptos relevantes

- Dureza de contacto elástica
- Índice de plasticidad ($\phi$): Define cómo será la deformación de la superficie. A mayor índice de plasticidad, menor comportamiento elástico.
- 

## Conclusiones

- La teoría desarrollada lleva a varias relaciones que determinan el área total de contacto real, el número de microcontactos, la carga, y la conductancia entre dos superficies de acuerdo con la separación de sus planos.
- **Dureza plástica** El área de contacto y la carga dependen de la separación, por lo que la razón entre ellas es casi constante. De aquí nace el concepto de _dureza elástica_, por el que el área de contacto puede predecirse a partir de la carga (como la dureza en deformación plástica).
- **Radio máximo:** 