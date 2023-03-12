---
id: 1riuu4vuybhcqnar0gqjfd1
title: 1 - Generalidades de Sistemas de Control
desc: ''
updated: 1677846374814
created: 1677360643175
---

El **control** consiste en manipular unas variables en algún sistema para que de este resulten variables con un resultado deseado.

## Índice

- [Índice](#índice)
- [Definiciones generales](#definiciones-generales)
- [Sistemas de control](#sistemas-de-control)
  - [Sistemas de control de lazo abierto](#sistemas-de-control-de-lazo-abierto)
  - [Sistemas de control de lazo cerrado](#sistemas-de-control-de-lazo-cerrado)
- [Elementos de un sistema de control](#elementos-de-un-sistema-de-control)
- [Ejemplo](#ejemplo)


## Definiciones generales

**Planta:** Grupo de piezas o elementos que funcionan interactuando entre sí, y cuyo objetivo es realizar una operación determinada.

**Sistema:** Operación y desarrollo caraterizado por una serie de _cambios graduales_ en su estado.

**Perturbaciones:** Señales o elementos que alteran de manera adversa la salida del sistema. Existen perturbaciones internas (ocurren dentro del sistema) y externas (ocurren por fuera del mismo).

**Variables:** Cantidades cualitativas y cuantitativas que determinan el estado de algún proceso (e.g. Temperatura, presión, luminosidad, caudal, etc). Existen dos variables importantes en el control:  

- **Variable manipulada:** Variable que el sistema de control manipula directamente para afectar la variable controlada.  
- **Variable controlada:** Variable dentro de un proceso que se puede medir y controlar a partir de la variable manipulada.

**Set-point:** Punto de ajuste al que se desea llevar la variable manipulada.

**Error:** Diferencia entre el valor del set-point y el valor de la variable manipulada.

## Sistemas de control

Es un sistema implementado a una planta para controlar sus variables durante un proceso. Se clasifican en:

### Sistemas de control de lazo abierto

Son sistemas de control en los que la salida no afecta la acción de control.  
> Los sistemas de control de lazo cerrado no funcionan bien ante perturbaciones, y son temporizados

**Ejemplos:** Lavadora, tostadora, semáforos antiguos.

![](/assets/images/2023-02-25-17-17-49.png)   
_Figura 1: Diagrama de bloques de un sistema de control de lazo abierto_

Donde:
- **IN/Entrada:** Valor deseado o _Set-point_
- **OUT/Salida:** Variable de salida
- **GC:** Controlador
- **GP:** Actuador o elemento final de control
- **P:** Proceso o planta
- **H:** Medición

### Sistemas de control de lazo cerrado

Son sistemas de control en los que existe una relación directa entre la salida y la variable de entrada.

La _señal de error_ actuante es la diferencia entre la señal de entrada y de realimentación.

> Los sistemas de control de lazo cerrado también se conocen como **realimentados**

![](/assets/images/2023-02-25-17-23-01.png)     
_Figura 2: Diagrama de bloques de un sistema de control de lazo cerrado_

Donde:
- **IN:** Variable de entrada o _set-point_
- **GC:** Controlador
- **GP:** Actuador
- **P:** Proceso o planta
- **u:** Perturbaciones
- **H:** Medición
- **b:** Error
- **OUT:** Variable de salida

## Elementos de un sistema de control

- **Elemento primero de medida:** Elemento sensor encargado de medir una magnitud y convertirla a una señal.  
- **Elemento transmisor:** Elemento encargado de recibir una señal del elemento sensor y transmitirla a distancia.  
- **Elemento controlador:** Elemento encargado de recibir la señal, procesarla para encontrar el error repecto a la variable deseada y enviar una señal que afecte la variable controlada.  
- **Elemento final de control:** Elemento encargado de recibir una señal del controlador y regular la variable controlada.

## Ejemplo

El siguiente es el diagrama de proceso de un sistema de control de nivel. Realice su diagrama de bloques:

![](/assets/images/2023-02-25-18-03-52.png)
