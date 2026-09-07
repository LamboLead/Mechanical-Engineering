---
id: aezdzm1p8lqaeix5lwkwiaa
title: 2 - Aceite sintético
desc: ''
updated: 1737674944540
created: 1737656174446
---

A continuación se especifican los pasos para seleccionar un aceite sintético a partir de un aceite mineral ya utilizado:

1. Seleccionar inicialmente un aceite sintético de referencia en la misma marca y del mismo grado ISO que el aceite mineral ya utilizado, teniendo en cuenta el tipo de aceite sintético que se va a utilizar de acuerdo con las condiciones de trabajo (PAO, PAG, Diéster, etc).
2. Calcular el nuevo rango de la $T_{op}$ en la zona de fricción teniendo en cuenta que se reducen entre 8 y 12°C al utilizar aceite sintético respecto al mineral. Ubicarlas en el gráfico ASTM D341.
3. Verificar que la nueva $T_{op}$ está dentro del rango de la viscosidad de diseño. Si no, ubicarlas, teniendo en cuenta que hay que incrementar en 10% la viscosidad con respecto a la viscosidad mínima de diseño para la $T_{op}$ máxima real en la zona de fricción.
4. Verificar si el grado ISO del aceite sintético de referencia cumple. Si no, hallarlo.

## Caso: Selección de aceite sintético para un compresor de tornillo CTCCH

### Enunciado

Se requiere seleccionar el aceite para el mismo un compresor de tornillo de _Cámara de Compresión Húmeda_ (CTCCH), con las mismas condiciones de operación, que utiliza el aceite mineral seleccionado en el punto anterior.

### Desarrollo

1. **Disminución de $T_{op}$ por lubricante sintético:** Se espera que con este cambio de lubricante la $T_{op}$ disminuya entre 8 y 12°C, entonces se toma en promedio un decremento de 10°C. La temperatura de operación mínima y máxima real, según el caso anterior, serán ahora de $T_{op,min,r} = 50°C$, y $T_{op,max,r} = 63°C$.

2. **Verificación de la viscosidad en _OC_:** Se localizan los valores de $T_{op}$ de 50 y 63°C en el gráfico, y su intersección con la curva del sintético ISO 68 AW están por fuera del valor máximo de 22cSt para la viscosidad en operación _OC_.
   
   ![](/assets/images/2025-01-23-13-46-40.png)

3. **Aceite sintético ideal a utilizar:** Se traza una curva paralela a la del ISO 68 AW que se cruce con la $T_{op,min,r} = 50°C$ y con el valor de la viscosidad máxima $V_{OC} = 22cSt$ en operación _OC_. Luego, por dicha curva se encuentra la escala de la temperatura a 40°C, y se encuentra de la escala vertical que el aceite sintético a utilizar debe tener 30cSt a 40°C.

   ![](/assets/images/2025-01-23-13-52-26.png)

4. **Estandarización del aceite:** Dada la viscosidad hallada, el lubricante sintético comercial más cercano es el ISO 32 AW. Ahora, las temperaturas de operación en condición _OC_ se encuentran entre $T_{op,min,r} = 50°C$ y $T_{op,max,r} = 63°C$, con una viscosidad entre $V_{min,OC} = 23cSt$ y $V_{max,OC} = 17cSt$.

   ![](/assets/images/2025-01-23-18-18-28.png)

5. **Ajuste de rangos _OF_ y _EF_:** Realizar el ajuste de la viscosidad en condición _EF_, siendo un 20% menor a la $V_{min,OC}$. Luego, se proyecta dicho valor en la curva del lubricante seleccionado, y se halla la $T_{op,min,EF}$. Entonces, se hallan los siguientes valores:
   
   - $65°C \le T_{op, OF} \le 75°C$.
   - $75°C \le T_{op, EF}$.
   - $13.6cSt \le V_{OC, OF} \le 17cSt$
   - $V_{OC, EF} \le cSt$
  
  Se concluye entonces que los rangos de temperatura de operación y viscosidad en _OF_ con lubricante sintético se elongaron, dando más oportunidades para corregir problemas cuando la $T_{op}$ se encuentra en _OF_.

   ![](/assets/images/2025-01-23-18-24-40.png)

## Procedimientos posteriores: Cambio de aceite mineral a sintético