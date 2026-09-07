---
id: 8y9948wx801lgfadllfi50f
title: 4 - Circuitos Neumáticos
desc: ''
updated: 1683655782172
created: 1683653349947
---

## Notación

- Existen cuatro zonas en un circuito neumático:
  - Elementos de trabajo: Actuadores neumáticos
  - Elementos de regulación: Reguladores de caudal y válvulas reguladora de caudal y de escape rápido. Su segundo dígito siempre es '0', y su tercer dígito irá de acuerdo a la norma de 'avance y retroceso'
  - Órganos de gobierno: Válvulas que controlan los actuadores (deben ser neumáticas únicamente)
  - Captadores de información: Válvulas auxiliares (deben ser de actuación mecánica y manual) que controlan las válvulas de gobierno.
  - Unidad de mantenimiento: Elementos auxiliares, como compresores, válvulas y demás elementos que sirven a todo el circuito. Su primer dígito siempre es '0', y su segundo dígito es normal, de acuerdo con su numeración.


> Si una válvula está afectando el avance, su segunda posición será par. Si una válvula está gobernando el retroceso, su segunda posición será impar.

## Secuencias

_(ver ejemplo de las diapositivas)_

- Cada movimiento de avance representa un '+', cada movimiento de retroceso es un '-'.
- Cada uno de los movimientos de la secuencia se denota por etapas. Si dos o más cilindros se realizan simultáneamente, los movimientos deben registrarse en la etapa.
- Una secuencia debe terminar siempre en su posición inicial. Cada cilindro debe realizar al menos un circuito completo.  
  Ejemplo: 1+ / 2+ / 2- / 3+ / 2+ / 2- / 3- / 1-
- 
