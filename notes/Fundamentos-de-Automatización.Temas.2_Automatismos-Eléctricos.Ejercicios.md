---
id: elr7aaa2tfr3j2akywmtipv
title: Ejercicios
desc: ''
updated: 1679250728706
created: 1677605740541
---

Los siguientes ejercicios utilizan conceptos de los ejercicios que le preceden. Es recomendable hacerlos en orden.

- [Circuitos simples](#circuitos-simples)
- [Circuitos complejos](#circuitos-complejos)
- [Circuitos temporizados](#circuitos-temporizados)
- [Inversión de marcha](#inversión-de-marcha)
- [Circuitos con protección](#circuitos-con-protección)
- [Fotosensores](#fotosensores)


## Circuitos simples

Circuitos sencillos que utilizan pulsadores, contactores y relés.

- **Encendido por pulsadores:**   
  Diseñe el circuito de mando de un sistema que puede prenderse desde dos pulsadores diferentes, y puede apagarse desde otro pulsador

  **R:** Se integra un circuito de autosostenimiento para encender la bobina **KM1** encendido por dos pulsadores **S1** y **S3**. El pulsador **S3** normalmente cerrado interrumpe el circuito de autosostenimiento, apagando el sistema.

  ![](/assets/images/2023-03-12-15-24-56.png)

- **Encendido de motores en secuencia:**  
  Diseñe un circuito para encender tres motores mediante pulsadores en una secuencia determinada: M1, M2, M3.

  **R.** Cada una de las bobinas **KM1**, **KM2**, **KM3** tendrán un contacto correspondiente para dejar pasar la corriente hacia los circuitos de autosostenimiento y a los motores en sí.

  ![](/assets/images/2023-03-12-18-11-24.png)

  Así mismo, se puede simplificar el circuito si _la salida del circuito de autosostenimiento se utiliza para darle energía a los motores_.

  ![](/assets/images/2023-03-12-18-13-09.png)

- **Apagado de motores en secuencia:** Modifique el diseño anterior para que los motores puedan apagarse en el orden: Primero M1, luego M2 y por último M3.
  
  **R.**
  1. Agregar pulsadores normalmente cerrados para interrumpir el circuito de autosostenimiento para **KM1**, **KM2**, **KM3**. Esto logra que los motores puedan apagarse independientemente.  
  ![](/assets/images/2023-03-12-18-38-41.png)

  1. Reorganizar los elementos para que:
     - **S2** no tenga efecto si **M1** no está encendido, y **S3** no tenga efecto si **M2** no está encendido.
     - **M2** no se pueda apagar si **M1** está encendido, y **M3** no se pueda apagar si **M2** está encendido. Esto se logra poniendo un contacto que reemplace los pulsadores normalmente cerrados **S5** y **S6**
  ![](/assets/images/2023-03-12-18-57-19.png)

## Circuitos complejos

Circuitos de mayor complejidad que utilizan pulsadores, contactores, relés y sensores de final de carrera.

- **Control de bandas transportadoras:**  
  Se desea diseñar el circuito de mando para una banda transportadora. Esta inicia siempre y cuando hay un objeto sobre la banda y después de pulsar el botón de _Start_. El objeto se desplaza hacia la derecha, y al finalizar, otro final de carrera debe detener el objeto apagando la banda.
  
  **R.** Se agrega un sensor de final de carrera normalmente abierto **S3** que, cuando está cerrado, energiza la bobina **KM1** y a su vez mantiene el circuito de autosostenimiento.
  El circuito de autosostenimiento se rompe gracias a un final de carrera normalmente cerrado **S2** que, cuando se abre, rompe con dicho circuito y apaga el motor.

  ![](/assets/images/2023-03-14-12-59-30.png)
  
- **Control de dos bandas transportadoras:**  
  Existen dos bandas conectadas entre sí. La banda 1 requiere de un pulsador y un final de carrera para iniciar. Una vez que esta termina, se enciende la banda 2. Ésta transporta el producto hasta el final. Mientras una banda funciona, la otra no puede funcionar.

  ![](/assets/images/2023-03-18-19-39-32.png)   
  _Diagrama del ejercicio_

  **R.** Se sigue la misma lógica del ejercicio anterior, y ahora el sensor de final de carrera que apaga la banda 1 (**S3**) sirve de activador para el circuito de autosostenimiento de la banda 2. De tal forma que ninguna de las dos bandas funciona al mismo tiempo.

  ![](/assets/images/2023-03-18-20-26-50.png)

## Circuitos temporizados

Circuitos que necesitan temporizar algún proceso.

- **Control temporizado de bandas transportadoras:**  
  Realice el mismo ejercicio anterior con la siguiente modificación: Cuando la banda 1 deja de funcionar, se enciende la banda 2 después de 20 segundos. Esta banda transporta el producto hasta el final y allí finaliza el movimiento del sistema. Mientras una banda funciona, la otra no puede funcionar.

  **R.** Se realiza el mismo análisis del ejercicio anterior. Esta vez utilizando un temporizador **KT1** para:
  - Cerrar instantáneamente un contacto **KT1** y mantener el circuito de autosostenimiento.
  - Cerrar el contacto **KT1** de forma temporizada (después de 20 segundos) y, a su vez, encender el motor **M2**.

  ![](/assets/images/2023-03-18-20-51-47.png)
  _Temporizador **KT1** contando_

  ![](/assets/images/2023-03-18-20-51-59.png)
  _Encendido de motor **M2**_

- **Control temporizado con proceso intermedio:**   
  Realice el mismo ejercicio anterior con la siguiente modificación: Modifique el circuito para que el operario pueda bajar la pieza entre el final de la banda 1 y el inicio de la banda 2 para limpiarla, mientras pasan los 20 segundos de espera.
  
  **R.** Se requiere que una vez el objeto haya llegado al final de la banda 2, el operario pueda bajar el objeto de la banda (desconectando el el final de carrera **S3**). Se requiere que el temporizador siga funcionando, incluso después de haber desconectado dicho sensor de final de carrera.

  En el _Ejemplo 1_, puede verse que aún después de haber desconectado el sensor, el temporizador **KT1** se mantiene energizado gracias a su circuito de autosostenimiento, y el circuito en general cumple las condiciones pedidas. Sin embargo, se requiere utilizar temporizadores electrónicos. El uso de estos temporizadores se ve ejemplificado en el _Ejemplo 2_.

  ![](/assets/images/2023-03-18-21-35-37.png)
  _Ejemplo 1: Circuito con implementación de temporizador a trabajo_

  En el _Ejemplo 2_, se puede ver la implementación de un temporizador electrónico, que es activado por medio del relé **KA1** que tiene su propio circuito de autosostenimiento. Dicho circuito es conectado una vez el contacto secundario accionado por el final de carrera **S4** es cerrado (indicando la llegada del objeto al inicio de la segunda banda), y es desconectado cuando el final de carrera **S5** es abierto (indicando la llegada del objeto al final de la segunda banda)
  ![](/assets/images/2023-03-18-22-39-45.png)
  _Ejemplo 2: Circuito con implementación de temporizador electrónico_

## Inversión de marcha

Circuitos que requieren invertir la marcha de algún motor

- **Banda transportadora temporizada con inversión de marcha:**   
  Se requiere mover un objeto con una banda transportadora. Para empezar, el objeto debe estar pulsando el final de carrera **S3**, y el operario debe pulsar el pulsador de inicio. Luego, la banda espera 30 segundos, y empieza a funcionar. Una vez el objeto llegue al final de carrera **S2**, la banda para y espera 10 segundos para invertir su marcha. La banda cuenta con dos pilotos **H1** y **H2** que indican si esta está moviéndose hacia la derecha y hacia la izquierda, respectivamente.

  ![](/assets/images/2023-03-19-13-12-24.png)   
  _Diagrama del ejercicio_

  **R.** 

- **Banda transportadora con un mismo temporizador:**   
  Realice el control de la banda transportadora del ejercicio anterior, esta vez con un tiempo de espera de 30 segundos para cada trayecto. El circuito debe utilizar un único temporizador.

  ![](/assets/images/2023-03-19-13-29-15.png)   
  _Diagrama del ejercicio_

  **R.**

- **Ascensor:**
  Se tiene un ascensor de dos pisos, con pulsadores en cada piso para llamar la cabina, y pulsadores dentro de la cabina para dirigirla al piso deseado. En cada piso hay un final de carrera que indica si el ascensor está en un piso indicado.   
  Las siguientes son condiciones de uso:
  - La cabina no se puede desplazar si no tiene las puertas cerradas.
  - Al llegar a un piso, la cabina abre las puertas de forma automática durante 20 segundos, y luego las cierra.
  - Si en el momento de cierre de las puertas algún objeto se atraviesa, el cierre debe detenerse e iniciar de nuevo la apertura de puertas, y esperar 20 segundos antes de iniciar el cierre.
  - Debe poder abrirse las puertas desde afuera en cualquier momento, una vez estas están cerradas.
  
  **R.**

## Circuitos con protección

Circuitos que requieren de implementación de dispositivos de protección: Fusibles, etc.

Realice el circuito de control de un motor que acciona una banda transportadora, 

## Fotosensores