---
id: hc30bfyeirq3x3dg4081y7y
title: Proyecto
desc: ''
updated: 1684358402426
created: 1682567043553
---

El proyecto de la materia consiste en la realización de un sistema que siga los siguientes pasos:

1. El paquete entra a **cinta 1**, donde es transportado hacia la **báscula**
2. La **báscula** mide el peso del paquete y lo clasifica en _paquete pequeño_ o _paquete grande_. Una luz indicadora para cada tipo de paquete se encenderá de forma correspondiente a la clasificación.
3. El paquete es transportado por la **cinta 2** hasta el **elevador**. El **elevador** subirá el paquete hasta un plano superior.
4. Una vez el paquete suba hasta el plano superior:
   1. Si el paquete es _pequeño_, el **cilindro A** lo empujará hacia la **cinta 3**, y lo dejará en la **tolva 1**.
   2. Si el paquete es _grande_, el **cilindro B** lo empujará hacia la **cinta 4**, y lo dejará en la **tolva 2**.
5. El elevador sólo puede moverse hacia el plano inferior una vez que el **cilindro A** y **cilindro B** han llegado a su posición final.

## Requerimientos

- Todos los subsistemas y componentes deben acoplarse.
- Todos los componentes electromecánicos deberán poder ser controlados por Arduino.

### Bandas transportadoras
- Las bandas deberán utilizar elementos comerciales y elementos que ya han sido adquiridos.
- Se deben tener motores independientes para cada banda transportadora.

### Paquetes a clasificar

Para que el ensamblaje pueda clasificar correctamente los paquetes, es necesario que estos cumplan con las siguientes características (serán cubitos hechos en MDF y cortados a láser)

### Método de clasificación por peso

### Actuadores


### Mecanismo de elevación
- Se utilizará un pequeño elevador (ver figura)
- El elevador deberá soportar 

### Tareas

- Averiguar cómo funcionan los circuitos Puente-h

## Ideas

### Bandas transportadoras
- Utilizar correas para sincronizar el movimiento de los rodillos.

### Clasificación por peso
- Ver [este tutorial](https://www.youtube.com/watch?v=sxzoAGf1kOo)