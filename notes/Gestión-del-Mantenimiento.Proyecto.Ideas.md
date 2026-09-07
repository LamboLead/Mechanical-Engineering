---
id: no75lh5ucdv8pkhvajrc1ao
title: Ideas
desc: ''
updated: 1684966648160
created: 1679864976278
---

Las siguientes son ideas que se pueden implementar en el proyecto.

### Análisis de calidad
Se puede solicitar una guía que muestre los estándares de calidad de los empaques, o de cada uno de los productos en la cadena de producción a medida que pasan por un proceso. Esto permite saber si la máquina asociada está funcionando adecuadamente.

### Estimación del ciclaje a partir de la producción
El ciclaje que tiene una máquina puede estimarse a partir de la cantidad de productos producidos. Esto puede estimarse a partir de las órdenes de producción o de la cantidad de material gastado en un periodo.

### Yéminus como CMMS
Se puede utilizar a Yéminus como el programa sobre el que se realizará la gestión del mantenimiento en la empresa, ya que esta ya lo utiliza para controlar el sistema productivo y los inventarios de la empresa.


---

# ¿Cómo llevar este proyecto a cabo?
Este proyecto se lleva a cabo a partir del cumplimiento de los siguientes objetivos:

1. **Gestión del mantenimiento:**
   1. Recopilación de información:
      1. Digitalización de manuales de usuario
      2. Recoger y plantear recomendaciones de uso y de mantenimiento del fabricante y demás información relevante de las máquinas a intervenir.
   2. Análisis de criticidad:
      1. Realización de análisis de criticidad
      2. Caracterización de las fallas con ACR.
      3. Realización de FMEA.
   3. Plan de mantenimiento preventivo:
      1. Implementar el sistema de conteo de ciclos de trabajo y horómetro
      2. A partir de la información recolectada y de las recomendaciones de fabricante, realizar un plan de mantenimiento preventivo, con tareas programadas en el sistema.
2. **Canales de comunicación**
   1. Crear notificaciones en el sistema de control o CMMS para garantizar el cumplimiento de las tareas de mantenimiento durante la producción.
3. **Capacitación y estandarización**
   1. Realización de análisis funcional de las máquinas
   2. Creación de hojas de procedimientos
   3. Crear procedimientos para poder realizar X proceso ... **_(completar)_**

### ¿Qué hacer?

- Averiguar sistemas de control sencillos para contar ciclos de trabajo y crear un plan de implementación, con cotizaciones y demás información impornate.
- Cuadrar reunión con César y Mateo para comentarles del plan y de los siguientes aspectos:
  - Se necesita acceso al sistema para poder ingresar la plantilla de órden de trabajo y poder crear los planes de mantenimiento.
  - Se necesita conocer la forma en la que el sistema de control va a comunicarse con el CMMS (JSON, CSV, etc) para poder subir y leer datos de ciclos de trabajo con el sistema.

### ¿Qué presentar?

1. Pequeño contexto sobre el proyecto
2. Objetivos
3. Objetivo 1: Gestión del mantenimiento en el proceso productivo
   1. Recopilación de información (¿?).
   2. Análisis de Criticidad, FMEA y caracterización de las fallas.
   3. Implementación de planes de mantenimiento preventivo.
   4. Generación de KPIs
4. Objetivo 2: Mejora de canales de comunicación   
5. Objetivo 3: Capacitación y estandarización
   1. Análisis funcional y recopilación de información (manuales y demás)
   2. Creación de hojas de especificaciones e instrucciones
   3. Creación de procedimientos para la realización de procesos administrativos (e.g. ¿Cómo caracterizar una falla?) y procesos operativos (e.g. ¿Cómo cambiarle el aceite a esta máquina?)

--- 

## Sistema de control de ciclos de trabajo y horómetro

  Se implementará una tarjeta controladora Arduino para enviar y recibir información desde y hacia el CMMS sobre los _ciclos de operación_ de la máquina.
  - Una vez la máquina se conecte y se encienda, el controlador iniciará la descarga de la información del CMMS sobre ciclos de trabajo (diarios/semanales/mensuales).
  - Una vez que la máquina empieza a trabajar, el Arduino empezará a contar los ciclos de trabajo por medio de un sensor acoplado a algún mecanismo de la máquina.
  - 

