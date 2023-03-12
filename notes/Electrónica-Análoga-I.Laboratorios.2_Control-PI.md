---
id: dzwtl790eginu5g2aldiim3
title: 2 - Sistemas de Primer Orden y Control PI
desc: ''
updated: 1678399929778
created: 1678380633002
---

En esta guía se pretende realizar una simulación de un sistema de primer orden y hacer un controlador PI.

Ver [[guía completa | D:\Documentos\Ingeniería mecánica\Semestre VIII\Electrónica Análoga I\Laboratorio\2_Control-PI\Guía.pdf]]

## Ejercicios

1. Diseñe un circuito que represente una planta de primer orden de la forma $G_p(s) = \frac{M}{\tau_s + 1}$.
   
   Elija un $V_i$ de onda cuadrada, con 1 voltio pico, un duty cycle del 50% y un semiperiodo tal que permita el tiempo de estabilización del sistema.

   ![](/assets/images/2023-03-09-17-08-35.png)  
   _Figura 1: Respuesta de sistema de primer orden a una señal de entrada de onda cuadrada_
   
2. Diseñe un controlador PI de la forma: $PI(s) = K_p + \frac{K_i}{s}$, con las siguientes características:
   - Que el sistema controlado en lazo cerrado tenga un error de estado estacionario de 0, un tiempo de estabilización $\tau_s <= 150ms$ y un amortiguamiento $\rho <= 0.6$
   - Para $V_i$ utilizar una señal de onda cuadrada, con duty cycle del 50%, amplitud y frecuencia adecuadas al tiempo de estabilización del sistema (hallar con cálculos).  

  ![](/assets/images/2023-03-09-12-07-52.png)   
  _Figura 2: Señal sub-amortiguada obtenida del controlador PI_
  
  Además, recalcular los parámetros para que el sistema tenga una respuesta sobreamortiguada como la de la figura 7. Se puede utilizar una señal de entrada manual.

  > Para obtener una respuesta sobre-amortiguada del sistema se debe elegir un valor de $\rho > 1$ y un $\tau_s >= 1s$

  ![](/assets/images/2023-03-09-12-05-09.png)   
  _Figura 2: Respuesta sobre-amortiguada de controlador PI_