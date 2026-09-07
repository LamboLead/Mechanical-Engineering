---
id: ejby97yev65adglceykjbun
title: 2 - Quality Function Deployment
desc: ''
updated: 1709006353351
created: 1708963266910
---

_Página del Dieter: 124 (pdf)_

El **QFD** (Quality Function Deployment) es una herramienta de planeación y de solución de problemas para enfocar la atención del equipo de diseño en la satisfacción de las necesidades del usuario a lo largo de todo el proceso de desarrollo del producto (PDP).

> La metodología **QFD** determina los requerimientos de importancia para cada fase del PDP y las utiliza para identificar las características técnicas de cada fase que más contribuyen a la satisfacción de los requerimientos.

## Etapas del proceso QFD

La metodología QFD abarca cuatro 'casas', que son:

![](/assets/images/2024-02-26-20-10-55.png)

### 1. Planeación de producto _(Product planning)_

También conocida como la '**Casa de la Calidad**', traduce las _necesidades del cliente_ en variables medibles llamadas _características de ingeniería_. 

> La **Casa de la calidad** indica la relación entre las necesidades del cliente y las características de ingeniería (parámetros de rendimiento y prestaciones) más importantes para satisfacerlas.

![](/assets/images/2024-02-26-21-11-15.png)

A continuación se muestra el proceso que ocurre dentro de la Casa de la Calidad.

1. **Requerimientos del cliente (RC)**   
   Especifica todos los requerimientos del cliente y su calificación de importancia (de 1 a 5). Estos requerimientos pueden ser agrupados en categorías identificadas a partir de un diagrama de afinidad.

   > Los requerimientos del cliente definen el '¿qué?' cumplir con el producto.

2. **Características de ingeniería (CE)**    
   Son varibles medibles del rendimiento y características del producto identificadas por el equipo de diseño para satisfacer los requerimientos de los clientes.  

   - Algunas _CE_ pueden ser 'peso', 'fuerza', 'velocidad', 'consumo', 'confiabilidad', etc.
   - En la parte superior de las _CE_ se define la dirección de mejora. Los símbolos $\uparrow, \downarrow$ indican que un mayor y menor valor para la característica es mejor, respectivamente.

   > Un buen acercamiento al planteamiento de características de ingeniería consiste en preguntarse '¿Qué puedo controlar que me permite cumplir las necesidades de mi cliente?'

3. **Matriz de correlación**   
   Muestra el grado de interdependencia entre las _CE_. Por ejemplo, si una característica cambia y ésta posee una correlación positiva con otra, esta última también debe ser evaluada.

   ![](/assets/images/2024-02-26-22-40-36.png)

4. **Matriz de Relaciones**   
   Es el centro de la Casa de la Calidad. Relaciona los requerimientos del cliente (filas) con las características de ingeniería (columnas).    
   La intersección entre los RC y CE representa el nivel de relación que existe entre ellos, representados por los siguientes símbolos (exponentes):

   | Símbolo | Nivel de relación | Valor |
   |:---:|---|---|
   | $\bullet$ | Fuerte | 9 |
   | $\bigcirc$ | Media | 3 |
   | $\Delta$ | Débil | 1 |
   | (en blanco) | No hay | 0 |
   
5. **Ranking de importancia**   
   Determina el ranking de las características de ingeniería más importantes para cumplir con los requerimientos del cliente.
   1. La **importancia absoluta** de cada _CE_ se halla multiplicando el valor numérico de cada celda de la _Matriz de Relaciones_ por cada uno de los valores de importancia de cada _RC_. Se suman los resultados para cada columna y se ponen en la columna **5a**.
   2. La **importancia relativa** de cada _CE_ es la misma importancia absoluta, normalizada en una escala del 0 al 1, expresada en porcentaje.
   3. El **orden de importancia** hace un ranking de los _CE_ dsde 1 hasta el número de _CE_ en la Casa de Calidad.
   
6. **Asesoramiento de clientes**    
   Muestra cómo los productos líderes en la competencia cumplen los RC. Esta información proviene directamente de encuestas a clientes, consultores y departamentos de marketing.

   ![](/assets/images/2024-02-26-22-46-58.png)

7. **Asesoramiento técnico**    
   Indica cómo los productos de la competencia puntúan (de 1 a 5) en alcanzar los niveles de cada una de las _CE_.    
   Aquí también puede incluirse un valor de _dificultad técnica_ que indica la probabilidad de alcanzar los valores deseados cada una de las _CE_ (de 1 para baja a 5 para alta probabilidad).

8. **Valores objetivo**
   Define los objetivos a alcanzar. Estos guían la selección y evaluación de conceptos potenciales de diseño.

### 2. Despliegue de piezas
### 3. Planeación de procesos
### 4. Planeación de producción
