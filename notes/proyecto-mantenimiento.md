---
id: 6aezac6xb3g7zq1q1suriwb
title: Proyecto de Mantenimiento
desc: ''
updated: 1789531378548
created: 1788744349613
---

## Conceptos importantes:

- Remaining Useful Life


## Ideas

- Todo sistema de  mantenimiento puede tener retroalimentación para saber si está siendo efectivo, midiendo costos, trabajos realizados, disponibilidad... ¿cómo brindar retroalimentación a un sistema de mantenimiento de una flota o vehículo?
- Hay que entender a los clientes y qué es lo que les interesa: ¿Cuánto cuesta un vehículo parado por una falla?
- Idea: Investigar PEM y cómo complementarlo con mantenimiento predictivo.
- 

## Proyectos

1. Mantenimiento predictivo de motores con análisis de aceites y telemetría en tiempo real (LAP)
2. Planeación de inventarios y operación basados en datos de falla y predicción de fallas por vehículo
   1. Planeación y asignación de recursos para realizar mantenimientos
   2. Planeación de inventarios basado en la condición de equipos y demanda del mercado
   3. Idea: Se detecta una falla de forma temprana > Se llama al cliente para realizar el cambio respectivo > Se solicita el repuesto con anterioridad > 
   4. Idea: Se analiza el inventario y pedido de repuestos con anterioridad, ingresando vehículos activos actualmente, parámetros como odómetro, muestras de aceite, zona geográfica donde operan los vehículos, calidad del combustible, patrones de conducción del conductor, etc; para predecir la cantidad de repuestos/grupo de repuestos a solicitar para uno/varios motor(es).
3. Análisis de vibraciones, sonidos, termografía, aceites, etc; para predecir fallas en mecanismos específicos del motor (árbol de levas, camisas y anillos, casquetes, etc.)
4. Implementación de control de calidad de principio a fin: Estandarización de procedimientos, minimización de garantías de taller, maximización de la conformidad del cliente, y minimización del tiempo de mantenimiento.
5. Mantenimiento preventivo como estrategia comercial: Identificar horas/km de recorrido y avisar al cliente sobre el preventivo correspondiente


---

## Planteamiento de proyecto

1. Planteamiento y justificación del problema: Plantear y entender por qué resolver este problema
2. Estado del arte
   1. Búsqueda de proyectos similares
   2. Recolección de fuentes de información: Telemetría, análisis de aceites, tasas de falla de los componentes y de los motores por dichas fallas, venta y cotización histórica de repuestos, manuales, uso y recorrido de vehículos, calidad de fluidos, zonas geográficas, patrones de conducción del conductor...
   3. Búsqueda de modelos de predicción de demanda
3. Prototipo
   1. Alimentación de los datos: Asegurar un flujo de información constante para alimentar los modelos
   2. Preparación de los datos: Recolección de características, filtrado y formateo correcto de datos
   3. Ingeniería de características: Recolectar las características con las que se entrenarán los modelos 
   4. Optimización de hiperparámetros: Entrenamiento y realización de pruebas con diferentes modelos de predicción, encontrando los modelos que mejor se desempeñan en diferentes ciclos en el tiempo.

![](/assets/images/2026-09-15-23-02-54.png)