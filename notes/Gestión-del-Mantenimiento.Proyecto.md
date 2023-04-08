---
id: t1cks71llxu0xjhofock4n3
title: Proyecto
desc: ''
updated: 1679867143778
created: 1676390578065
---

## Requerimientos

Crear un CMMS para realizar la gestión de mantenimiento de los equipos de una empresa.

Este CMMS debería tener:

- Cuadro de mando integrado, con gráficos y KPIs.
- Análisis Funcional de las máquinas
- Análisis de Modo y Efectos de Falla para cada falla
- Análisis de Causa Raíz
- Taxonomía de los equipos de la empresa.
- Procedimientos para comprar repuestos.
- Log o bitácora de las fallas o cualquier acción realizada en las máquinas.

## ¿Por qué un CMMS?

El núcleo de un CMMS consiste en la información, que está registrada en la **orden de trabajo**.  
Este núcleo se compone del plan de mantenimiento preventivo y el mantenimiento correctivo.

**Conceptos**
- Orden de trabajo
- Plan de mantenimiento
- Mantenimiento correctivo
- Ficha técnica

![](/assets/images/2023-02-25-18-31-42.png)

### ¿Que debe tener un plan de mantenimiento?
- Personal a utilizar
- Herramientas
- Insumos
- Pasos
- Recomendaciones y notas

---
## Enfoque del proyecto

Se construirá un CMMS que incluya el esquema de mantenimiento para las dos máquinas más importantes en el proceso productivo de empaques para motores. 

### Requerimientos del CMMS

El software deberá ser:
- Escalable: En caso de que la empresa quiera añadir más equipos en el sistema.
- Integrable con el área y los sistemas de producción.

El software deberá poseer, al menos:
- Un cuadro de mando integrado, que contenga diferentes KPIs e indicadores que muestren datos claves, producto de la gestión del mantenimiento de la empresa.
- Un sistema de bitácoras que permita ver y registrar información sobre el mantenimiento realizado a la maquinaria.
- Un repositorio de manuales y documentos para cada máquina.
- Un canal dedicado de comunicación por el cual el área de mantenimiento y el área de producción se comuniquen de forma directa, con la posibilidad de compartir órdenes de trabajo e información relativa a cada área.

### Pasos
- **Pablo, David:** Investigar cómo funciona Yéminus, y ver si se puede integrar con Excel o alguna otra herramienta.
- Recolección de datos de producción respecto al proceso productivo de empaques:
  - Cantidad de producción realizada en un año.
  - ...
- Recolección de datos de la cortadora y la troqueladora más utilizada:
  - Manuales
  - Mantenimiento
  - Funcionamiento
  - Análisis de funciones

## Preguntas
- ¿Qué debe tener el CMMS en esta empresa?
- ¿Cómo implementar lo que hemos visto en clase al proyecto?

## Preguntas para la empresa
- ¿Cómo es la producción de la empresa? Así se pueden estimar los tiempos de mantenimiento.
- ¿Las prensas hidráulicas tienen sistemas de alivio?
- ¿Cuál es el límite de operación de las máquinas?