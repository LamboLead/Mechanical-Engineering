---
id: pksy0k5hj9nhuksoxcl3kiq
title: Funcionamiento
desc: ''
updated: 1684346813012
created: 1684343542671
---

## Control de motores DC con Arduino

Para poder controlar motores DC con Arduino es necesario utilizar un controlador de velocidad Puente-H. El Arduino enviará señales PWM de velocidad y dirección al controlador para controlar su movimiento.

Para poder elegir el controlador adecuado para el motor, es necesario conocer:
- Voltaje de operación del motor
- Corriente promedio
- Corriente en paro

### Controlador Puente-H doble L298N

Este es uno de los controladores más utilizados para controlar motores DC. Usa transistores BJT para realizar su función y, por lo tanto, no es uno de los más eficientes.

- Voltaje de motor: 5-35V
- Corriente promedio: 2A
- Corriente máxima: 3.5A
- Voltaje lógico: 3.3-5.5V

[Control](https://youtu.be/ygrsIqWOh3Y?t=756)   
[Link de compra](https://www.didacticaselectronicas.com/index.php/robotica/controladores-1/controlador-puente-h-l298n-controladores-driver-drivers-puente-h-para-motores-paso-a-paso-dc-l298n-detail)

![](/assets/images/2023-05-17-12-25-54.png)

- ENA/ENB: Controla la dirección del motor A y B
- IN1, IN2: Controla la velocidad del motor A
- IN3, IN4: Controla la velocidad del motor B

![](/assets/images/2023-05-17-12-27-24.png)

### Controlador Puente-H doble TB6612FNG

Este es un controlador que usa transistores MOSFETS para realizar su función y, por lo tanto, es más eficiente que el L298N.

- Voltaje de motor: 4.5-13.5V
- Corriente promedio: 1.2A
- Corriente máxima: 3.2A
- Voltaje lógico: 2.7-5.5V

[Control](https://youtu.be/ygrsIqWOh3Y?t=1147)   
[Link de compra](https://www.didacticaselectronicas.com/index.php/robotica/controladores-1/driver-dual-motor-dc-tb6612fng-tb6612fng-controlador-controladores-drivers-para-motor-driver-motor-motores-paso-a-paso-motor-dc-de-doble-canal-duales-detail)