---
id: 2zwj3dhtz7xtkcctafqh382
title: Notas
desc: ''
updated: 1708038400948
created: 1707478663864
---

## Clase 2 (09/02/2024)

**Pasos para empezar a realizar un procedimiento CAM:**

- Elegir el punto 0
- Programar coordenadas absolutas o incrementales.
- Elaborar plan de trabajo en pasos individuales: Herramienta, velocidad de giro, refrigernate, recorridos, avances, etc.
- Escribir el programa.
- Simulación.

> Importante: Al cambiar de herramientas, es necesario cambiar la altura respecto a la herramienta original para evitar un daño de la pieza o de la máquina.

**Ejercicio:** Maquinar el perfil de la siguiente pieza.

![](/assets/images/2024-02-09-07-40-19.png)

```gcode
  O0123
  G17 G21 G32 G40 G80
  T1M6
  G54
  S3000M3
  G90 G0 X-35 Y-21.
  G43 Z5 H1
  M8
  G1 Z-3 F250
  Y-14 F500
  X-28
  G3 X-21 Y-7 J7
  G1Y0
  G2 X21 I21
  G1 Y-7
  G3 X28 Y-14 I7
  G1 X35
  Y-21
  X-35
  G0 Z5
  M9
  G32
  M5
  G53 G0 Y0
  M30
```

![](/assets/images/2024-02-09-07-40-55.png)

### Para adelantar
- Códigos G, M vistos en clase

## Clase 3 (14/02/2024)

### Compensaciones
- Compensación radial: Consiste en realizar una compensación de 
- Compensación axial: Realizar una compensación de altura dependiendo de la altura de la herramienta con la que se trabaja.

> Todas las herramientas tienen una altura diferente. Por lo tanto, es necesario tener en cuenta la altura de cada herramienta relativa a la altura de la primera herramienta.

**Ejercicio:** Mecanizar la siguiente pieza

![](/assets/images/2024-02-14-06-32-27.png)

```gcode
  G17 G21 G32 G40 G80 G54
  G90
  T1 M6 (Selección de herramienta)
  S3000
  M3
  G0 X-42 Y0
  G41 D10 (Definir compensación radial por la izquierda, con diámetro 10)
  Z10
  G1 Z-1 F500
  Y7
  G3 X-28 Y21 R14 (Arco en sentido antihorario)
  G2 X-14 Y35 R14 (Arco en sentido horario)
  G1 Y42
  G3 X-7 Y49 R7
  G1 X0
  Y0
  X-42
  Z10 (Elevación de pieza)
  G32
  M5
  M30 (Fin de programa)
```

### Ciclos de taladrado

- Taladrado simple (`G81`): 
- Taladrado por picoteo (`G83`): En el taladrado a alta profundidad es necesario extraer o romper la viruta.
  - Extracción de viruta
     ```gcode
        G83
     ```
  - Rompimiento de viruta
     ```gcode
        G83
     ```

**Ejercicio:** Realizar el perfilado para la siguiente pieza

![](/assets/images/2024-02-14-07-26-20.png)

[Simulador](https://ncviewer.com/)

```gcode
   G17 G21 G32 G40 G80 G54
   G91
   T1 M6
   S3000
   M3
   G0 X0 Y0
   G41 D10
   Z10
   G1 Z-1 F500
   Y20
   X10
   Y30
   G90
   G2 X35 Y60 R15
   G1 X55 Y20
   G91
   X25
   Y30
   X10 Y-5
   X10 Y5
   G90
   Y0
   X0
   G42 D10
   Z10 Y-5
   Z0
   G91
   G2 X30 R15
  
```