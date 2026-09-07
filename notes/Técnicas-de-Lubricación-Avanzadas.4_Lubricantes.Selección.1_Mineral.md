---
id: snvqe102h10pwnwruvx6a6j
title: 1 - Selección de aceite mineral
desc: ''
updated: 1737674355401
created: 1737156936599
---

A continuación se especifican los pasos para seleccionar un aceite mineral:

1. Seleccionar un aceite preliminar teniendo en cuenta las recomendaciones del fabricante de la máquina.
2. Trazar la curva del aceite mineral seleccionado  en el _Gráfico ASTM D341_, con su viscosidad en $cSt$ a 40°C y a 100°C. Ubicar el rango de la temperatura de operación de diseño $T_{op,d}$ y hallar el rango de viscosidad de diseño mínima y máxima para garantizar una operación _OC_.
3. Verificar que el aceite mineral utilizado sí es el adecuado con base en la temperatura real de trabajo $T_{op,r}$. De lo contrario, se debe hacer el procedimiento para hallarlo con el fin de utilizar el aceite mineral correcto.
4. Seleccionar el nombre y la marca del aceite a utilizar, teniendo en cuenta los datos consignados en los formatos de catalogación.

## Caso: Selección de aceite mineral para un compresor de tornillo CTCCH

### Enunciado

Se requiere seleccionar el aceite para un compresor de tornillo de _Cámara de Compresión Húmeda_ (CTCCH), constituido por tornillos macho y hembra, que giran a 1800rpm, y cuatro rodamientos de rodillos a rótula.

El sistema de lubricación está constituido por aceite, un depósito, filtro separador, enfriador, bomba de engranajes, filtro y tuberías de entrada y salida de aceite del compresor.

![](/assets/images/2025-01-17-18-56-56.png)

![](/assets/images/2025-01-17-18-57-09.png)

### Datos del lubricante

![](/assets/images/2025-01-17-18-58-13.png)
![](/assets/images/2025-01-17-18-59-47.png)

### Desarrollo

1. **Ubicación de parámetros de diseño iniciales:** En el _Gráfico ASTM D341_ se ubican 32cSt @ 40°C, y 5cSt @ 100°C.

2. **Parámetros de diseño en condición _OC_:** Se localiza el rango de la temperatura de operación de diseño $T_{op,d}$ y de viscosidad en condición _OC_:
   
   - $50°C \le T_{op, OC} \le 58°C$.
   - $15cSt \le V_{OC} \le 22cSt$

  ![](/assets/images/2025-01-17-19-01-40.png)

3. **Parámetros de diseño en condición _OF_ y _EF_:** Se localiza el rango de la viscosidad en condición _OF_ y _EF_, siendo la viscosidad  _EF_ un 20% menor que la mínima del rango OC. Luego, se halla la temperatura en condición _EF_ proyectando en la intersección de $V_{EF}$ en la curva del lubricante:  
   
   - $V_{EF} \le 12cSt$; $12cSt \le V_{OF} \le 15cSt$
   - $T_{op, EF} \ge 64°C$; $58°C \le T_{op, OF} \le 64°C$

   ![](/assets/images/2025-01-17-19-33-50.png)
   
4. **Cálculo de temperatura real:** Se halla el rango de temperatura de operación real $T_{op,r}$ a partir del rango en el que fluctúa la temperatura ambiente de diseño $T_{a,d}$ en el lugar de operación:

   $T_{op,r} = T_a + \Delta T_f$  
   
   Diferencias de temperatura de diseño mínima y máxima:
   - $\Delta T_{f,min} = 50°C - 15°C = 35°C$
   - $\Delta T_{f,max} = 58°C - 23°C = 35°C$
  
   Temperaturas de operación real mínima y máxima
   - $T_{op,min,r} = 25°C + 35°C = 60°C$
   - $T_{op,max,r} = 38°C + 35°C = 73°C$

   Los anteriores son los valores reales de temperatura a los que va a operar el compresor si se utilizara el lubricante referido por el fabricante. Por lo tanto, es necesario reelegir el lubricante para disminuir la temperatura real de operación en la condición _OC_.

5. **Ajuste del lubricante a temperatura real:** Se proyecta la vertical de la $T_{op,max,r} = 73°C$ hasta un 10% por encima del valor mínimo de la viscosidad original en condición _OC_, es decir, $16.5cSt$; se traza una curva paralela a la del lubricante anterior, y se halla el valor de la viscosidad a 40°C, que en este caso es de $75cSt$.
   
6. **Estandarización del lubricante:** El aceite comercial más cercano es el _ISO 68_. En este caso, $60°C \le T_{op,OC} \le 73°C$. Este rango no es el óptimo para obtener el 100% de la vida disponible de la máquina, ya que el máximo en la zona de fricción debe ser de 65°C; sin embargo, es el más óptimo en este caso.

   ![](/assets/images/2025-01-17-20-36-08.png)

