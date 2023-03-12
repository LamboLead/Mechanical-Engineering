---
id: wk89xfjyq7radvx7bxj51h8
title: Ejercicios
desc: ''
updated: 1678379348872
created: 1677106669513
---

- [Algebra de Boole simple](#algebra-de-boole-simple)
- [Álgebra con Diagrama de Karnaugh](#álgebra-con-diagrama-de-karnaugh)

## Algebra de Boole simple

1. **Sistema de mando de una puerta giratoria**   
   Una puerta ha de ser controlada, de tal manera que se pueda abrir y cerrar desde cualquier habitación. Además, debe ser posible abrir la puerta desde una de las habitaciones y cerrarla desde la otra. La puerta no se mueve si se presionan simultáneamente los interruptores A y B.

   ![](/assets/images/2023-02-22-18-23-28.png)

2. **Sistema de votación**  
   Diseñar un sistema de aprobación de propuestas mediante un piloto en la votación de una junta compuesta por cuatro miembros, donde el miembro A es el presidente, y en caso de empate en la votación, el voto del presidente define la decisión.

   ![](/assets/images/2023-02-22-18-23-44.png)

3. **Control de ascensor**  
   Generar la función de control para el movimiento de la cabina de un ascensor de dos pisos. En cada piso hay un pulsador para llamar el ascensor a dicho piso (P1, P2) y en cada piso hay un sensor de final de carrera (S1, S2) que indicará en qué piso se encuentra la cabina.

   ![](/assets/images/2023-02-22-21-25-08.png)


## Álgebra con Diagrama de Karnaugh

1. **Control de nivel**
   Se quiere controlar el nivel de un tanque que tiene un consumo aleatorio. El tanque es alimentado por dos bombas (B1, B2), las cuales tienen sus respectivos pozos de alimentación, cuyos sensores (T1, T2) indican si los pozos tienen agua. El tanque tiene dos sensores de nivel superior e inferior (NS, NI):
   - Si el tanque está lleno (NS), no funcionan ninguna de las bombas.
   - Si el nivel está por debajo del nivel inferior (NI), funcionan las dos bombas (B1, B2) siempre y cuando cada una tenga agua en su pozo (T1, T2).
   - Si el nivel está entre el nivel inferior y el nivel superior, la bomba 1 tiene prelación (B1). Si su pozo no tiene agua, entonces la bomba 2 (B2) se activa.   
   ![](/assets/images/2023-02-22-20-58-19.png)  
  _Diagrama del ejercicio_


  