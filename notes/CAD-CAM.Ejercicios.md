---
id: zpg492y8n6pc6yc9fpxnmgv
title: Ejercicios
desc: ''
updated: 1708639189871
created: 1708514306714
---

- **Planeado:** Elabore un programa manual que permita realizar una operación de planeado a la placa 
mostrada en la figura. No tenga en cuenta la compensación de herramienta.   
   ![](/assets/images/2024-02-22-16-30-43.png)

```gcode
(Ejercicio 1: Planeado sencillo)
G17 G54 G21 G90 G32 G80 G40
T1 M6
S3500 M3
G0 X0 Y0
(Inicio de planeado)
G0 X-10 Y-10
Z14 (suponiendo que la pieza tiene altura 20mm)
G91
G01 X210 F10000
G03 Y20 R10
G01 X-210
G02 Y20 R10
G01 X210
G03 Y20 R10
G01 X-210
G02 Y20 R10
G01 X210
G03 Y20 R10
G01 X-210
G02 Y20 R10
G01 X210
G03 Y20 R10
G01 X-210
(Salida segura)
M05
G90
G0 Z100
G0 X0 Y0
G32
M30
```

- **Contorneado:** Elabore un programa manual que permita realizar una operación de perfilado y obtenga la 
forma mostrada. Incluya un inicio seguro al programa. No tenga en cuenta la compensación de herramienta
```gcode
  (Ejercicio 2: Contorneado)
G17 G54 G21 G90 G32 G80 G40
T1 M6 (Herramienta 3mm)
S3500 M3
G0 X0 Y0
Z50
(Inicio de contorneado)
G91
G0 X-10 Y-10
Z0
G90
G1 X0 Y0 F5000
G41 D3
G91
G1 Y20
X10
Y30
G2 X25 Y7 R15
G90
G1 X55 Y20
G91
G1 X25
Y30
X10 Y-5
X10 Y5
Y-50
X-100
G90
G0 Y-5
X25
G91
G1 X15
G41 D3
G3 X-30 R15

(Salida segura)
G90
G0 X-10
M05
G90
G0 Z100
G0 X0 Y0
G32
M30
```


2. Elabore un programa manual que permita obtener la forma mostrada en la figura. No 
tenga en cuenta la compensación de la herramienta (por diámetro, si por longitud) y use 
una herramienta de diámetro 3 mm para la ejecución del programa. El programa debe 
incluir un inicio seguro y todos los códigos necesarios para realizar un mecanizado 
adecuado. Las medidas están en mm.

![](/assets/images/2024-02-21-06-18-59.png)

```gcode
G17 (Mecanizado en plano XY)
G54
G20
G90
G32
G80
G40
G21
G91
T1 M6 (Cambio de herramienta)
G43 Z5 H2 (Añadir compensación de altura) (¿?)
S1000 M3 (Velocidad. Giro de cabezal en sentido horario)
M8 (Refrigerante)
G0 X0 Y0 (Definición de ceros)
(Inicio de planeado)



```