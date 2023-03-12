---
id: 593m2bnk7mj9fck8b1mhsz0
title: Diagrama de Karnaugh
desc: ''
updated: 1677119225971
created: 1677106686100
---

Es una representación gráfica a partir de una _tabla de verdad_ que permite identificar los diferentes resultados de una operación que involucra el Álgebra Booleana. Este mapa puede utilizarse desde 2 hasta 5 variables.

Consiste en formar grupos dentro de una tabla de verdad de acuerdo con las siguientes reglas:

## Reglas de simplificación

1. **Las agrupaciones son exclusivamente de unos**. Ningún grupo puede contener algún cero.   
   ![](/assets/images/2023-02-22-18-34-02.png)
2. **Las agrupaciones pueden hacerse únicamente horizontal y verticalmente**. Las diagonales están prohibidas.  
   ![](/assets/images/2023-02-22-18-34-27.png)
3. **Los grupos deben contener $2^n$ elementos** (1, 2, 4, 8, ...)
   ![](/assets/images/2023-02-22-18-34-44.png)
4. **Cada grupo deberá ser tan grande como sea posible**  
   ![](/assets/images/2023-02-22-18-35-07.png)
5. **Todos los unos tienen que pertenecer mínimo a un grupo**. Aunque pueden pertenecer a más de uno.   
   ![](/assets/images/2023-02-22-18-35-24.png)
6. **Puede existir solapamiento de grupos**   
   ![](/assets/images/2023-02-22-18-35-53.png)
7. **La formación de grupos también puede producirse con las celdas extremas de la tabla**. Las celdas superiores pueden agruparse con las inferiores, y las de la extrema derecha con la de las extrema izquierda.   
   ![](/assets/images/2023-02-22-18-36-16.png)
8. **Tiene que resultar el menor número de grupos posible**   
   ![](/assets/images/2023-02-22-18-36-45.png)
9.  **En la tabla de verdad, sólo puede cambiar el valor de una variable a la vez**
  ![](/assets/images/2023-02-22-18-37-10.png)

## Ejemplo

**Selección de candidatos**   
En una empresa están en proceso de selección aspirantes a un puesto de trabajo. El proceso consta de 5 pruebas, y para aprobar, el candidato debe cumplir alguna de las siguientes condiciones:
- Aprobar la segunda y tercera prueba
- Aprobar la segunda y cuarta prueba

![](/assets/images/2023-02-22-21-26-57.png)