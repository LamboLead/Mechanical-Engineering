---
id: cu34owyshxfe1oxa1bcfv8k
title: Movimientos básicos
desc: ''
updated: 1708661965758
created: 1708647735428
---

# Movimientos básicos

## Movimiento lineal

| Código | Nombre | Descripción / Uso | Tener en cuenta |
|:---:|---|---|---|
| `G00` | Interpolación lineal en rápido | Mueve la herramienta de forma rápida a algún punto del espacio de trabajo.| La máquina se desplaza con su máxima velocidad |
| `G01` | Interpolación lineal con avance definido | Mecaniza en línea recta. | El avance es especificado con el comando `F` |

**Ejemplos:**
- Mecanizado en diagonal hasta la posición X=50, Y=95; avance 190mm/min.
  ```gcode
    G01 X50 Y95 F190
  ```

## Movimiento circular / en arco

| Código | Nombre | Descripción / Uso | Tener en cuenta |
|:---:|---|---|---|
| `G02` | Arco en sentido horario | Mecaniza arcos y círculos en sentido horario | El avance es especificado con el comando `F` |
| `G03` | Arco en sentido antihorario | Mecaniza arcos y círculos en sentido antihorario | El avance es especificado con el comando `F` |

**Ejemplos:**
- Movimiento circular horario hasta las coordenadas X=22.5, Y=40; radio de arco R=-27.5, avance F=160mm/min
  ```gcode
    G02 X22.5 Y40 R-27.5 F160
  ```

> **Importante:** Para los movimientos en arco:
> - Si el radio especificado es positivo, el punto de rotación será tal que la longitud de arco será mínima.
> - Si el radio especificado es negativo, el punto de rotación será tal que la longitud de arco será máxima.
>
> ![](/2024-02-13-19-50-45.png)