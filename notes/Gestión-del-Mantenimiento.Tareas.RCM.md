---
id: et7l1tn4jlrs19dh37dmjt6
title: Revisión bibliográfica - Reliability Centered Maintenance
desc: ''
updated: 1683568789932
created: 1683232044809
---

## Artículo: _Reliability-Centered Maintenance: A Case Study_
Fecha de publicación: Diciembre de 2000   
Autores: Randall G. Wilmeth, de Xcel Energy; y Michael W. Usrey, de la Universidad de Colorado.   
Link: http://dx.doi.org/10.1080/10429247.2000.11415089

### Introducción: ¿En qué consiste la implementación del RCM en este caso?
  
La implementación de RCM se da en una empresa proveedora de energía eléctrica llamada _Xcel Energy_, producto de una unión de varias empresas: _Northern States Power (NSP)_ y _New Century Energies (NCE)_, cuya existencia fue el resultado de la unión entre _Southwestern Public Service Co. (SPS)_ y _Publici Service Company of Colorado (PSCO)_ . Una de las oportunidades de ahorro de dinero post-unión que el equipo encontró fue en el programa de mantenimiento del equipamiento de subestaciones eléctricas. La plataforma RCM del _Electric Power Research Institute_ (EPRI) fue recomendada como base para reemplazar este programa de mantenimiento.

La empresa Xcel Energy recientemente completó la primera fase de un piloto de plan de mantenimiento RCM para el equipamiento de transmisión de potencia. Sus resultados indican que programas de mantenimiento previos resultaron en pocas o demasiadas acciones de mantenimiento del equipamiento en cuestión.

Varias oportunidades de ahorro de costos son presentadas, aunque se extrae la conclusión de que es necesario implmentar RCM en una escala más grande para que estos puedan tener un efecto significativo sobre las finanzas de la empresa.

A continuación en el artículo, se explica el origen y evolución de _Reliability Centered Maintenance_, su definición concreta (que no se añadirá a la reseña), y su proceso de un análisis previo al proceso de implementación; así como su integración en un CMMS.

Más adelante se muestran ejemplos de implementaciones fallidas y satisfactorias de programas de mantenimiento basados en RCM, y el tema más importante, cómo se llevó a cabo el estudio piloto para la implementación de RCM de SPS y sus resultados, lecciones aprendidas y conclusiones.

### Análisis previo al proceso de implementación de un programa de mantenimiento basado en RCM

La mayoría de las aplicaciones de RCM por fuera de industrias ampliamente reguladas utilizan una versión simplificada del RCM, que omite la construcción de un historial de fallas para cada pieza del equipamiento de estudio, y deja la construcción de los análisis de modo y efectos de falla en la experiencia y conocimiento del usuario que las utiliza.

Los siguientes son siete pasos para realizar una implementación simplificada del modelo de RCM de EPRI para la transmisión de potencia:

1. Establecer el enfoque y alcance del estudio para definir los límites del trabajo.
2. Identificar interfaces para definir específicamente las entradas requeridas y las conexiones que no serán objeto de estudio.
3. Especificar funciones importantes del objeto de estudio, ya que el RCM pretende preservar las funciones más importantes del mismo.
4. Identificar modos dominantes de falla para ser evaluados.
5. Identificar modos críticos de falla. Las consecuencias de falla son evaluadas para cada modo dominante para determinar su severidad. Si son severas, el modo se define como 'crítico'. Los modos de falla 'no críticos' no se tendrán en cuenta en el estudio.
6. Identificar las causas dominantes de falla, que son identificadas para aquellos modos que se definen como críticos. Sólo las causas que puedan prevenirse con mantenimiento serán consideradas en el estudio.
7. Seleccionar tareas de mantenimiento rutinarias utilizando lógica de decisión, teniendo en cuenta cada una de las causas dominantes de falla, así también se considera cambiar el diseño y la operación para poder operar el equipo hasta la falla.

### Desarrollo: ¿Cómo se llevó a cabo el estudio?

En _Southwestern Public Service Co._ fueron seleccionadas fuentes de poder de DC como el objeto de estudio para realizar un estudio piloto de RCM por su relativa simplicidad y su importancia, ya que estas se utilizan para dar poder a equipo de protección en las subestaciones.

**Enfoque:** La fuente de poder DC en una subestación se considera como un sistema, ya que este incluye una batería y su respectivo cargador o fuente principal de DC. Se consideraron dos subestaciones, cuya diferencia radica en que una está equipada con alarmas remotas, y la otra no.
**Fronteras del sistema e interfaces:** La batería, su cargador y los cables que los conectan componen las fronteras físicas del sistema.   
Las interfaces son ítems que se originan por fuera de dichas fronteras, y se asume que estarán siempre disponibles para soportar el equipamiento o la operación del sistema. Fueron identificadas las siguientes interfaces:
- Entrada AC al cargador de baterías.
- Conexión a tierra del cargador de baterías.
- Cable de DC.
- Alarmas remotas SCADA (para subestación que las equipa).

![Diagrama de bloques de una fuente de DC](/assets/images/2023-05-05-11-39-05.png)   
_Figura 1: Diagrama de bloques de una fuente de poder DC_

**Funciones principales del sistema:** Una fuente de poder DC tiene una única función: Proveer corriente eléctrica DC para el equipamiento de una subestación eléctrica.

**Modos de falla dominantes:** Se encontraron los siguientes modos y efectos de falla:

![Modos dominantes de falla y efectos de las mismas](/assets/images/2023-05-05-11-48-19.png)   
_Figura 2: Modos dominantes de falla y efectos de las mismas_

Nota: Todos los modos de falla son críticos, quiere decir que todos conllevan a un paro total del equipamiento.

**Criticidad de los modos de falla:** Una medida de la criticidad fue establecida para que los recursos del mantenimiento fueran destinados únicamente donde las consecuencias de la falla son severas. Todas las fallas fueron determinadas como _críticas_.

![Criticidad de la falla de una fuente de poder DC](/assets/images/2023-05-08-11-05-15.png)   
_Figura 3: Criticidad de la falla de una fuente de poder DC_

**Causas dominantes de la falla:** Las causas dominantes de falla de las baterías y cargadores de baterías fueron revisadas y asignadas a todos los modos de falla.

![Causas dominantes de falla y tareas de mantenimiento para la falla: 'pérdida del camino de condudcción de la batería'](/assets/images/2023-05-08-11-04-15.png)   
_Figura 4: Causas dominantes de falla y tareas de mantenimiento para la falla: "pérdida del camino de conducción de la batería"_

**Selección de tareas de mantenimiento:** La lógica de selección de tareas de mantenimiento mencionada en la sección anterior fue usada para determinar si una tarea de mantenimiento económicamente efectiva existe para cada causa de falla dominante. Esta lógica se explica a continuación:

- Si existe una forma viable de monitoreo, entonces se indica un programa de mantenimiento predictivo.
- Si la condición de monitoreo no existe, entonces se recomienda una tarea de mantenimiento preventiva y basada en el tiempo.
- Si una tarea de mantenimiento preventiva no se puede aplicar, entonces uno decide si la falla puede ser tolerada.
- Si una falla no puede ser tolerada, un cambio en el diseño del sistema es pedido a ingeniería.
- Si una falla puede ser tolerada y no es evidente, una tarea de búsqueda de fallas periódica es especificada.
- Si una falla puede ser tolerada y es evidente, el ítem se opera hasta la falla, y uan tarea de mantenimiento correctivo es realizada.

> Este proceso de decisión es realizado para cada una de las fallas dominantes.

> Si bien el RCM es un buen método para especificar tareas de mantenimiento, la frecuencia de dichas tareas se deja al personal encargado de la gesitón del mantenimiento. El objetivo es conseguir una frecuencia que minimice los costos del mantenimiento.

**Comparación de tareas:** Una vez que el proceso de análisis de RCM se ha terminado, se debe realizar una comparación entre las tareas recomendadas de RCM y las tareas preexistentes de mantenimiento, las recomendaciones de fabricante y requerimientos regulatorios.   
Si alguna tarea recomendada no se relaciona con un modo crítico de falla, no está regulada por una autoridad regulatoria, y no invalida una garantía, la tarea es eliminada.

### Resultados del estudio

Fueron estimados un ahorro de 3 horas de trabajo del personal al año. Escalado a todas las fuentes de poder de todas las subestaciones, estos ahorros son considerables.

A continuación se muestran los resultados del análisis financiero de esta estrategia de mantenimiento:
![Análisis financiero de dicha estrategia de mantenimiento](/assets/images/2023-05-08-11-28-30.png)   
_Figura 5: Análisis financiero de dicha estrategia de mantenimiento_

### Lecciones aprendidas

- Como se esperaba, el proceso de implementación de RCM fue probado como una herramienta efectiva sobre la cual basar un programa de mantenimiento de una subestación eléctrica.
- Existen varios aspectos importantes que necesitan ser analizados para que las organizaciones implementen programas de mantenimiento basados en RCM:
  - La cultura de la compañía, y la capacidad de aceptar y promover el cambio.
  - Desarrollar una forma de medir el éxito del programa.
  - Establecer expectativas y metas realistas.
  - Desarrollar y mantener un CMMS y un programa de mantenimiento para una constante optimización.
- Debe existir un proces para medir el éxito de un programa RCM. Un sistema ideal de medida debería incluir:
  - Costos de mantenimiento preventivos y correctivos para cada uno de los equipos individualmente.
  - Paros causados por fallas en el equipo, incluyendo costos totales de dichos paros.
  - Disponibilidad del equipo.
  - Costos innecesarios evitados por el programa de mantenimiento.
  - Costos estimado del peor, más posible y más probable caso, multiplicado por la probabilidad de que cada uno ocurra.
- Una vez un programa de RCM es implementado, el programa debe ser revisado periódicamente, ya que nuevas fallas, modos y efectos serán encontradas y, por lo tanto, las tareas de mantenimiento y sus frecuencias deben ser actualizadas.
- Antes de la implementación completa del RCM, un CMMS tiene que estar en pie.

### Conclusiones

El programa de mantenimiento de las fuentes de poder DC para SPS puede ser mejorado al implementar RCM. Para experimentar todos los beneficios del RCM, el proceso debe ser aplicado a través de todo el equipo que conforma la subestación eléctrica.