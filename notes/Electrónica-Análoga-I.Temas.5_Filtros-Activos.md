---
id: na8bomzh17fub5giwugh3o1
title: 5 - Filtros Activos
desc: ''
updated: 1686595312662
created: 1684370080427
---


Un filtro es un circuito que modifica la magnitud de la ganancia y/o la fase de las componentes frecuenciales de la señal de entrada. El filtro se diseña para amplificar o reducir las componentes frecuenciales de una señal. Este tipo de filtros utiliza amplificadores operacionales para su operación.

**Ventajas:**
- No requieren inductores.
- Se pueden diseñar y construir por etapas.
- Cada etapa puede tener una ganancia igual o diferente de 1.

**Desventajas:**
- Requieren una fuente de energía para su polarización.
- El circuito está sujeto a las limitaciones del amplificador operacional.

**Frecuencia de corte:** La frecuencia a la cual la frecuencia del filtro ha caído 3dB por debajo de la ganancia de estado estable (ganancia de DC).

## Tipos de filtros

### Filtro paso bajo (Low-Pass)

Este filtro permite el paso de todas las frecuencias que estén por debajo de la _frecuencia de corte_
**Aplicaciones:** Se utilizan generalmente para eliminar o suprimir ruidos de alta frecuencia.

### Filtro paso alto (High-Pass)
Este filtro permite el paso de todas las frecuencias que estén _por encima de la frecuencia de corte_.

### Filtro banda de paso (Band-Pass)
Este filtro permite pasar las frecuencias que estén _entre dos frecuencias de corte_.

### Filtro banda de rechazo (Stop-Band)
Este filtro permite pasar las frecuencias que estén _por fuera de dos frecuencias de corte_.

## El filtro ideal
Aquel filtro que multiplica por cero las frecuencias que no entran dentro de su rango de operación, y multiplica por la ganancia aquellas que sí.

Este filtro no puede implementarse en la realidad, ya que representa un sistema no causal.

## El filtro real

Es necesario atenuar el efecto del filtro para que pueda ser implementado en la realidad. Es necesario implementar una banda de transición.

k

