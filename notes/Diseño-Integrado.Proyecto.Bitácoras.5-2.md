---
id: fvjf13l7ut8hdm1798dlof0
title: 7. Revisión de diseño de detalle (5 feb)
desc: ''
updated: 1739839887998
created: 1739836789875
---

**Fecha:** 5 de febrero de 2025.   
**Hora:** 8:00.   
**Lugar:** Salón de reuniones del bloque 4.

## Resumen
Se le mostró al profesor el trabajo realizado y se recibieron comentarios al respecto.

---

## Contenido

> El profesor está muy preocupado porque no hay avances.

**Análisis estático:**

- El diagrama de cuerpo libre presentado no es diagrama de cuerpo libre, ya que éste requiere añadir las fuerzas externas asociadas a todo el ensamblaje: reacción de la cama, reacción en las correas, y el peso del individuo, por ejemplo.
- El análisis estático requiere añadir todas las fuerzas asociadas con el individuo. Para realizar el análisis de esfuerzos con MEF es necesario realizar un buen análisis estático y un buen DCL.

**Análisis de esfuerzos:**

- En el punto E tal vez no hay empotramientos, se restringirían desplazamientos y coeficiente de fricción. Se debe también añadir las fuerzas de las correas para fijar los 
- Es necesario optimizar los elementos de la malla, con ese primer modelo obtenido se puede refinar la malla en los puntos B y D en futuras simulaciones de MEF.
- Añadir las fuerzas (o restricciones) de las correas en el modelo, que permitan mejorar la fidelidad del modelo.

**Dimensionamiento de la pieza:**

- ¿Es necesario añadir un torquímetro? Si ya se tiene una curva característica del actuador, tal vez no sea necesario.

**Selección del material y proceso de manufactura:**

- El termoformado es el proceso de manufactura utilizado en fabricación de prótesis.
- El número de piezas es un indicador importante para definir el proceso de manufactura. Si hay producción en masa, el mejor proceso es el de inyección (aunque el diseño del molde es más complejo).
- El proceso de manufactura debe quedar completamente especificado (todos los parámetros requeridos para fabricar la pieza)

**Pieza comercial:**

- Cuando los actuadores ya incluyen un sistema de control, es necesario evaluar que las variables a controlar sean suficientes.
- Tener en cuenta que el cambio de piezas y mantenimiento debe evitar crear cualquier tipo de inconveniente en ambientes hospitalarios
- En las recomendaciones del producto, recomendar que la máquina se utilice en ambientes que no sean ricos en gases sensibles a la chispa.
- Consejo: Definir la cantidad de piezas a partir del número de centros de rehabilitación.

## Asistentes
- Manuela Valencia Gil
- Juan Camilo Rengifo Colorado
- Jorge Andrés Montoya
- Daniel Hernández Figueroa
- Juan David López