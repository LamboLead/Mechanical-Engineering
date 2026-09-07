---
id: z0srusq5hqm07gpixeka40i
title: Fundamentals of Fluid Power
desc: ''
updated: 1747023925575
created: 1743564237570
---

(01/04/2025)

En este MOOC de Coursera se pretende cumplir los siguientes objetivos:

1. Realizar una introducción a componentes, circuitos y sistemas que utilicen un fluido para realizar trabajo.
2. Explicar los aspectos fundamentales para modelar circuitos hidráulicos y neumáticos.
3. Proveer de herramientas clave para diseñar y analizar circuitos hidráulicos para aplicaciones específicas.
4. Realizar una introducción a la modelación de sistemas de potencia por fluidos utilizando software.

## Módulo 1: Potencia de fluidos

La _potencia de fluidos_ es el uso de la energía de un fluido presurizado (usualmente aceite) para transmitir fuerza o movimiento.
 
Ésta se divide en dos:

**Hidráulica:** Utiliza un fluído líquido e incompresible para ejercer fuerza o movimiento
- Trabaja a altas presiones, por lo tanto, alcanza grandes fuerzas.
- Ofrece un control preciso del sistema gracias a su incompresibilidad.

**Neumática:** Utiliza un gas (fluido compresible) para ejercer fuerza o movimiento.
- Trabaja a altas velocidades y bajas fuerzas.
- Difícil de controlar, ya que el aire es compresible.

> Los fluidos tienen una gran densidad energética.

### Cilindros

![](/assets/images/2025-04-08-21-12-25.png)

La fuerza que ejerce un cilindro con un fluido presurizado se resume en la siguiente ecuación:

$$
F = P_{cap}A_{cap} - P_{rod}A_{rod}
$$

### Conceptos

- Presión: Fuerza por unidad de área. Es una variable que se mide relativa a cierto punto.
- Caudal volumétrico o másico: Flujo de fluido en cierta cantidad de tiempo, medido en términos de volumen o masa.
  Para fluidos incompresibles: Metros cúbicos por segundo, litros por minuto, galones por minuto; kilogramos por segundo, o libras por segundo.
  Para fluidos compresibles: 

- Potencia: Capacidad de conversión de energía. En fluidos, equivale a: $Potencia = Presión \cdot Caudal$

## Leyes importantes

**Ley de Pascal:** Todos los puntos de un sistema cerrado se encuentran a una misma presión, siempre y cuando el fluido no se encuentre en movimiento y la gravedad sea despreciable.

**Conservación de masa:** En la física Newtoniana, la masa de los fluidos se conserva en un sistema hidráulico o neumático. Además, en hidráulica se asume que el fluido es incompresible (a pesar de que a grandes presiones, el fluido se comprima entre 2% y 3%. Esta compresibilidad se engloba en una propiedad llamada 'bulk modulus').

![](/assets/images/2025-04-08-22-33-18.png)

## Eficiencia de un cilindro

Hay dos fuentes de pérdida de energía:
- Sellos internos en el pistón
- Sello externo para soportar el pistón
- Viscosidad del fluido, con fricción fluida.
- Caídas de presión de los puertos de admisión y escape.
- Fugas de fluido.
- Compresibilidad del fluido.

![](/assets/images/2025-04-14-20-40-25.png)

**Ejemplo:** ¿Cuál es la fuerza y velocidad máximas de un cilindro en extensión y retracción?

![](/assets/images/2025-04-14-20-46-11.png)

---

## Resources

![](/assets/images/2025-05-11-23-23-58.png)

![](/assets/images/2025-05-11-23-25-24.png)