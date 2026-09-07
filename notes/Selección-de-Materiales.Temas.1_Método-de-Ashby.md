---
id: ubuzao5km6kgc9x22krqoo0
title: 1 - Método de Ashby para selección de materiales
desc: ''
updated: 1724257656993
created: 1710287193808
---

A continuación se explica detalladamente el Método de Ashby para la selección de materiales con un enfoque en el diseño.

Para lograr seleccionar materiales de forma óptima, es necesario seguir los siguientes pasos:

1. **Traducción de los requerimientos:** Es necesario convertir los requerimientos de diseño (es decir, lo que la pieza _debería_ hacer o cumplir), en restricciones y objetivos que puedan aplicarse a una base de datos de materiales.
2. **Filtración:** Eliminar los materiales que no pueden cumplir con las restricciones definidas anteriormente.
3. **Puntuación:** Clasificar los materiales restantes por su resultado al ser evaluados respecto a un _índice de desempeño_ (por ejemplo, minimizar costo o maximizar resistencia al impacto).
4. **Documentación:** Explorar a profundidad los candidatos resultantes más prometedores, a partir de otros criterios cualitativos (por ejemplo, implementaciones en otros proyectos de ingeniería, capacidad de manufactura, etc).

## 1. Traducción de requerimientos de diseño

En todos los casos de selección de materiales para una pieza, se definen los requerimientos de diseño que una pieza debe cumplir (es decir, definir qué debe hacer la pieza); por ejemplo, que soporte cierta carga, que contenga cierta presión, que transmita el calor, etc.

Estos requerimientos deben estar sujetos a restricciones o **_variables fijas_**: Algunas dimensiones deben ser fijas, que la componente debe soportar las cargas o presiones sin fallar, y muchas otras. En conclusión, el diseñador debe cumplir cierto _objetivo_: Hacer la pieza lo más barata, ligera, o segura posible; o alguna combinación de estas.

Algunos parámetros pueden ser ajustados para optimizar el objetivo a partir de **_variables libres_**: Algunas dimensiones originales de la componente pueden cambiarse, y por supuesto, el material a seleccionar.

En resumen, la primera fase de un proceso de selección de materiales para una pieza o componente consiste en definir:
- **Funciones:** ¿Qué debe realizar la componente?
- **Restricciones:** ¿Qué condiciones no negociables deben cumplirse? ¿Qué condiciones negociables o deseables podrían cumplirse?
- **Objetivo:** ¿Qué debería maximizarse o minimizarse?
- **Variables libres:** ¿Qué parámetros puede cambiar el diseñador?

## 2. Filtración: Definición de límites de atributos

De los requerimientos de diseño, también pueden definirse límites que filtran la lista completa de materiales. Por ejemplo, si existen requerimientos como "el componente debe funcionar en agua hirviendo", o "el componente debe ser ópticamente transparente", dicho requerimiento impone atributos límite como _temperatura máxima de servicio_, o _transparencia óptica_.

## 3. Puntuación: Índices de desempeño



> Ningún material se considera inapropiado para alguna aplicación hasta que se demuestra lo contrario.

## Ejemplo: Selección de un material para un visor de un casco de policía

Se requiere seleccionar un material para el visor de un casco para proveer la máxima protección al rostro del usuario en caso de impacto.

**Requerimientos de diseño:**
- Transparencia: El visor debe ser ópticamente transparente para poder ver con claridad a través de él.
- Forma curva: Para proteger el rostro por el frente, los costados y por debajo, el visor debe ser curvo; es decir, el material debe ser moldeable.

### Traducción de requerimientos

A partir de los requerimientos definidos para la pieza, se definen:
- **Función:** Ofrecer la máxima protección contra el impacto rostro del usuario.
- **Restricciones:** Transparencia y capacidad de ser moldeado.
- **Objetivo:** La propiedad que mide la resistencia a la fractura de los materiales es la resistencia a la fractura $K_{1C}$; por lo tanto, el objetivo del diseñador consiste en maximizar $K_{1C}$.
- **Variables libres:** Espesor y material del visor.




---

Un buen ejercicio de selección de materiales requiere contestar las siguientes preguntas:
- ¿Qué materiales existen?
- ¿Qué propiedades nos disinteresan de ellos?
- ¿Cómo obtener un perfil o mapa de propiedades acorde a una aplicación?

---