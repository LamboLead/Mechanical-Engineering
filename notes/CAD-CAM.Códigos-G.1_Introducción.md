---
id: scmcfxb2qm1vvipteuanhjk
title: 1 - Introducción al mecanizado CNC
desc: ''
updated: 1707869517254
created: 1707866853714
---

**Programa de control numérico:** Es una lista _secuencial_ de instrucciones de mecanizado que se le entrega a una máquina para que las ejecute. Sus instrucciones están escritas en _código G_ y _código M_.

**Códigos G:** Son códigos para ordenar el movimiento de la herramienta.  
**Códigos M:** Son códigos que incluyen acciones necesarias para el mecanizado, como cambio de herramientas, paradas auxiliares, inclusión de lubricante, etc.

## Partes de un programa de control numérico

1. **Encabezado:** Contiene todas las instrucciones que preparan la máquina para su operación.
2. **Movimiento:** Consiste exclusivamente en la programación de los movimientos que ejecuta la máquina.
3. **Cierre:** Contiene todos los códigos G y M que desactivan todas las opciones ordenadas en el encabezado.

## Estructura de una instrucción

La siguiente es la estructura típica de un programa de mecanizado CNC.

**[N] [G] [X Y Z] [F] [S] [T] [M]**

| Letra | Nombre | Descripción |
|:---:|---|---|
| **N** | Número del bloque |  |
| **G** | _Go_ | Especifica el tipo de instrucción de movimiento |
| **X** | Cota en eje X | Distancia a mover en dirección del eje X |
| **Y** | Cota en eje Y | Distancia a mover en dirección del eje Y |
| **Z** | Cota en eje Z | Distancia a mover en dirección del eje Z |
| **F** | _Feed_ | Velocidad de avance |
| **S** | _Speed_ | Velocidad de husillo o rotación |
| **T** | _Tool_ | Número de herramienta |
| **M** | Funciones auxiliares | |

> Aunque para cada instrucción debe mantenerse el orden anterior, no es necesario que estén presentes todos los ítems.

**Ejemplo:**

```gcode
  N135 G01 X1.0 Y1.0 Z0.125 F5.0
```
- **N135:** Bloque actual (número 135).
- **G01:** Tipo de movimiento, en este caso lineal.
- **X1.0 Y1.0 Z0.125:** Coordenadas que indican el punto de fin del movimiento.
- **F5.0:** Velocidad de avance de 5in/min, o 5mm/min

## Ubicación espacial

### Dirección de los ejes coordenados

Para este caso, la dirección de cada dedo representa la dirección positiva del movimiento.

![](/assets/images/2024-02-13-19-03-50.png) ![](/assets/images/2024-02-13-19-03-15.png)

- la base de los dedos será siempre el origen (`X0, Y0, Z0`).
- El eje de rotación siempre será el eje Z.
- En una fresadora, la dirección más larga de la mesa es designada como la dirección X.

### Sistemas coordenados

Es posible definir tres tipos de sistemas coordenados dentro de un programa CNC:

1. Sistema absoluto de máquina.
2. Sistema relativo a la pieza.
3. Sistema flotante.

![](/assets/images/2024-02-13-19-05-30.png)

## Pasos para realizar un programa CNC

1. Elegir el punto de origen del sistema coordenado (comúnmente, relativo a la pieza a mecanizar).
2. Definir el tipo de coordenadas (absolutas o incrementales).
3. Definir un plan de trabajo para cada movimiento, considerando:
   - Herramienta a utilizar.
   - Velocidad de giro del husillo.
   - Necesidad de refrigerante.
   - Recorridos y avances.
4. Escribir el programa, traduciendo los pasos anteriores al lenguaje de programación.
5. Probar el programa en software CAM.
6. Ingresar el programa en la máquina de mecanizado y probar el programa de nuevo.
7. Ejecutar el mecanizado.
8. Verificar medidas de la pieza y compensar diferencias.
9. Optimizar el programa, verificando recorridos y avances de mecanizado (en caso de producción en masa).