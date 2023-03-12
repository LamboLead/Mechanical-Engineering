---
id: 4j1rbgeki7zxvpdlypsdcv0
title: 1 - Amplificadores Operacionales Básicos
desc: ''
updated: 1678381049348
created: 1676496604094
---

En esta guía se pretende hacer uso de los amplificadores operacionales inversor, no inversor, sumador y restador.

Ver [[guía completa | D:\Documentos\Ingeniería mecánica\Semestre VIII\Electrónica Análoga I\Laboratorio\2_Amplificadores-operaciones-básicos\Guia_Practica_1_G1.pdf]]   

## Ejercicios

1. Diseñar un circuito para implementar, simultáneamente, las siguientes funciones:  
$V_{out} = 2V_{in} - 3$ y $V_{out} = 3V_{in}-2$, utilizando únicamente un generador de funciones y una fuente dual.   
  Utilice una onda seno como $V_{in}$ con una frecuencia de $50kHz$ y amplitud $0.5\mu V$. Se deben obtener las siguientes señales:

  ![](/assets/images/![](/assets/images/2023-02-15-16-36-13.png).png)
  ![](/assets/images/2023-02-15-16-36-25.png)

  Utilizar el OPAM LF353, con la siguiente distribución de pines:   
![](/assets/images/2023-02-15-16-37-27.png)

  Además, la fuente dual que dará energía al OPAM tiene un voltaje igual a $\plusmn10V$.

1. Diseñe otro circuito para adecuar la salida de un [sensor de temperatura LM35](https://kaimte.com/product/details/texas-instruments/lm35dz-lft1.html?gclid=Cj0KCQiAorKfBhC0ARIsAHDzsltleP5Zj4srKlQkfg5xVaaaHIKoT_6VMLG0kLq7WRjrH_HK6SMBORwaAq0NEALw_wcB) (figura 4) a una escala de 0V a 10V para temperaturas entre 0°C y 100°C, sabiendo que el sensor  LM35 entrega $10mV/°C$.   
   ### Recomendaciones
   - Utilice el menor número posible de OPAMs para cada circuito, justificando que su decisión corresponde al menor número de amplificadores operacionales.
   - Aproximar los valores de resistencias obtenidos a valores comerciales.

  ![](/assets/images/2023-02-15-16-40-15.png)