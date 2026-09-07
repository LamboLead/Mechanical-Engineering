---
id: iq7wzntq34rplyca4nlacsc
title: Ciclos de taladrado
desc: ''
updated: 1708661955876
created: 1708645729200
---

# Ciclos de taladrado

## 1. Taladrado simple

Define un ciclo de taladrado simple con un solo retroceso de la broca. Se utiliza en perforaciones no muy profundas, que no requieran hacer evacuación inmediata de la viruta.

![](2024-02-22-18-37-54.png)

**Sintaxis:**
```gcode
  [G98, G99] G81 X_ Y_ Z_ R_ F_
```
**Parámetros:**
- `X, Y`: Coordenadas de inicio de taladrado
- `Z`: Coordenada en Z de profundidad final
- `R`: Punto de retroceso
- `F`: Velocidad de avance

**Alteraciones:**
- `G98`: Terminación en el punto inicial especificado por `Z`
- `G99`: Terminación en el punto de retroceso especificado por `R`

**Ejemplo:** Realizar un ciclo de taladrado con ocho perforaciones, terminando en el punto de retroceso:

![](2024-02-22-19-18-21.png)

```gcode
  G99 G81 Z-27 R1 F3000 (Inicio de ciclo de taladrado simple)
  X2
  Y-3
  X1
  X4
  X5
  Y-3
  X4
  G80 (Fin de ciclo de taladrado)
```

## 2. Taladrado con picoteo

Define un ciclo de taladrado por pasos

```gcode
  G83 G98 X_ Y_ Z_ Q_ V_ R_ D_ F_
```
Parámetros:
- `Z`: Coordenada en Z de profundidad final
- `Q`: Pasos de picoteo (mm)
- `V`: Picoteo inicial (mm)
- `R`: Profundidad inicial a la que se realiza el taladrado (mm)
- `D`: Devolución de taladrado (mm)

![](2024-02-22-18-41-37.png)

> El código `G80` finaliza el ciclo de taladrado