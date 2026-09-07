---
id: miw8818o2omogqfaua1rfzj
title: 5 - Selección por tenacidad
desc: ''
updated: 1725591567234
created: 1724441372871
---

**Tenacidad:** Es una medida general que describe la capacidad de un material de absorber energía y deformarse plásticamente antes de fracturarse.

**Resiliencia:** Es la energía almacenada en el material sin deformación plástica.

**Tenacidad a la fractura:** Específicamente, se refiere a la capacidad de un material de resistir la propagación de una grieta, cuantificada por medio del parámetro $K_{nC}$, siendo $n$ el modo por el cual se evalúa dicha propiedad.

## Mecánica de la fractura

### Concentradores de esfuerzos

Son secciones de una pieza tales que los esfuerzos aplicados allí son amplificados localmente.

![](/assets/images/2024-09-05-16-44-17.png)

Un concentrador de esfuerzos, microscópicamente, puede ser una grieta interna o externa; o macroscópicamente, puede ser también esquinas afiladas, indentaciones o rayaduras.

**Factor de concentrador de esfuerzos ($K_t$):** Es una medida que indica cuál es el efecto de un concentrador de esfuerzos sobre un esfuerzo externo aplicado sobre la pieza.

$$
K_t = \frac{\sigma_m}{\sigma_0} = 2\Big(\frac{a}{\rho_t}\Big)^{1/2}
$$

Con:
- $\sigma_m$: Esfuerzo local amplificado por el concentrador.
- $\sigma_0$: Esfuerzo original aplicado a la pieza.
- $a$: Longitud de la grieta.
- $\rho_t$: Radio de punta de la grieta.

### Tenacidad a la fractura

El esfuerzo crítico $\sigma_c$ tal que una grieta se propague en un material frágil es:

$$
\sigma_c = \Big(\frac{2E\gamma_s}{\pi a}\Big)^{1/2}
$$

Con:
- $E$: Módulo de elasticidad.
- $\gamma_s$: Energía de superficie específica.
- $a$: 1/2 de la longitud de la grieta.

> Todos los materiale frágiles poseen numerosas grietas con diferentes tamaños, geometrías y orientaciones. Cuando la magnitud de un esfuerzo de tensión excede el valor de $\sigma_c$, una grieta aparece y se propaga rápidamente, llevando a una falla.

**Tenacidad a la fractura ($K_c$):** Es una propiedad que mide la capacidad de un material de fallar de forma frágil (con una grieta propagándose incontroladamente) cuando una grieta está presente.

$$
K_c = Y\sigma_c\sqrt{\pi a} \space \space [MPa\sqrt{m}; psi\sqrt{in}]
$$

Con:
- $Y$: Factor adimensional que depende de la longitud, geometría y orientación de la grieta y la pieza, así como la forma en la que la carga está aplicada.

**Tenacidad a la fractura en modo I ($K_{1c}$):** Es la tenacidad a la fractura que corresponde a la situación específica de una placa gruesa de material sometida a tracción, implicando que no existe una deformación significativa en las caras frontal y posterior de la placa.

$$
K_{1c} = Y\sigma\sqrt{\pi a}
$$

![](/assets/images/2024-09-05-21-36-37.png)

### Diseño basado en mecánica de la fractura

Es necesario considerar las siguientes situaciones teniendo en cuenta fracturas:

1. **Cuando el material y la longitud de la grieta son definidas:** Definiendo el material (y por lo tanto, $K_1c$) y el tamaño de grieta, el esfuerzo crítico tal que la grieta se salga de control se determina como:
$$
\sigma_c = \frac{K_{1c}}{Y\sqrt{\pi a}}
$$

2. **Cuando el esfuerzo y el material son definidos:** El tamaño de grieta crítico se determina como:
$$
a_c = \frac{1}{\pi}\Big(\frac{K_{1c}}{\sigma Y}\Big)^2
$$

---

_(ver ejemplo de diseño de un tanque a presión en la página 240 del Callister)_

---

## Selección de materiales por tenacidad

**¿Cómo saber si es necesario diseñar basándose en tenacidad?**

Un diseño por tenacidad generalmente se aplica en situaciones en las que se quiere evitar una fractura catastrófica e incontrolada. Esto es evidente en el diseño de contenedores a presión.

**_Yield before break:_** Es un método de diseño tal que se pueda detectar una deformación en el material del contenedor y su presión pueda ser liberada de forma controlada.

**_Leak before break:_** Utilizado en contenedores grandes, es un método de diseño tal que asegure que la grieta más pequeña que pueda propagarse descontroladamente tenga una longitud mayor que el espesor de la pared del material (tamaño crítico de grieta), y el contenido pueda escapar controladamente.

---
_(ver ejemplo de selección de materiales para tanque a presión en página 218 del Ashby)_

---

**Estructura**
- Definición de tenacidad
- (opc) Mecanismos de fractura
- ¿Qué hace que un material sea tenaz? ¿Qué propiedades del material se relacionan con la tenacidad? (desde el punto de vista de C. de materiales) (ver Callister)
- Macroscópicamente, ¿Cómo la microestructura de un material afecta su tenaicidad? (tamaño de grano, fases, etc)
- (opc) ¿Cuáles son los mecanismos de endurecimiento para metales? (por solución, por precipitación, por deformación)
- Definición de fractura, pasos para formación de grietas, modos de fractura (dúctil y frágil)
- Diseño para la fractura: ¿Cómo afecta la tenacidad a la fractura los concentradores de esfuerzos?
- ¿Qué es la tenacidad a la fractura? ¿Cómo se mide? ¿Qué modos hay?
- ¿Qué es el tamaño crítico de grieta?
- ¿Cómo diseñar y seleccionar materiales por tenacidad y tenacidad a la fractura? (ver caso de estudio)


Considere un elemento 

**Tenacidad a la fractura:** $K_{1c} = \sigma_R\sqrt{\pi c}$ Es la tenacidad a la fractura en modo 1, es decir, a tracción. se mide en un elemento plano a tracción, al que se le hace una entalla.



## Ideas
- El acero tiene una tenacidad de entre $50 - 250MPa \sqrt{m}$
- Un esfuerzo en una pieza puede verse como líneas de flujo en la pieza, y si las líneas de flujo se ven comprimidas por un cambio de geometría (huecos, grietas, cambios de sección)...

## Por leer
- Caso de estudio: Selección por tenacidad para cilindros de gas a baja presión. Página 218 del Ashby
- 