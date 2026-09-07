---
id: vpsi5kqj8r5fv1bdpdgije1
title: Lógica
desc: ''
updated: 1709311859319
created: 1708717901518
---

Aquí se especifica la lógica o pasos que se deben seguir para resolver un problema de selección de materiales, y poder traducirlo a código.

## Pasos

1. Recolectar e insertar en la interfaz gráfica todos los parámetros relacionados con la selección del material dentro de la aplicación.
2. Crear varias estructuras de datos que permitan ingresar parámetros con facilidad. Estructuras que obedezcan a:
   1. Geometría
   2. Aplicación
   3. Condiciones adicionales
3. Crear una base de datos de materiales que permita ingresar materiales y sus propiedades con facilidad. 
4. Obtener las ecuaciones que gobiernan cada una de las aplicaciones y las geometrías.
5. Integrar los parámetros y ecuaciones y hallar los índices de desempeño del material.

## Estructuras de datos

### Parámetros

**Geometría del material:**
- Tipo de geometría:
- Dimensiones:

**Aplicación:**
- Tipo de aplicación:
- Cargas a soportar:

**Condiciones adicionales:**
- Condiciones ambientales
- Acabado
- Tolerancias

### Materiales y procesos

#### Materiales

**Campos:**
- Nombre del material (string)
- Composición
  - Composición química en porcentajes (string)
  - Características de la molécula o celda unitaria (string)
  - Imagen de molécula o celda unitaria (string)
  - Tipo de enlace (string)
- _Propiedades físicas_
- _Presentaciones_

#### Presentaciones

**Campos:**
- Nombre
- _Procesos de manufactura_
- Características
  - Resistencia a la corrosión
- _Proveedores_
- Precio por kilo

#### Propiedades físicas

**Campos:**
- Nombre
- Descripción
- Unidades de medida

**Registros:**
- Módulo de Young
- Esfuerzo de fluencia
- Esfuerzo máximo de rotura
- Densidad

#### Procesos de manufactura

**Campos:**
- Tipo
- Nombre
- Descripción

#### Proveedores

**Campos:**
- Nombre
- Teléfono
- Dirección

1. **Parámetros:** Insertar todos los parámetros necesarios para la selección del material. Estos parámetros son:
   - Tipo de geometría y dimensiones relevantes.
   - Tipo de carga y distancia a la cual será aplicada la carga (mostrar un gráfico).
   - Condiciones adicionales:  
      - ¿Corrosión?
      - ¿Acabado?
      - ¿Buenas tolerancias?
2. **Cálculo de modelo:** Crear todas las estructuras de datos relacionadas con la aplicación (ecuación que gobierna la carga, geometría) 

---

## Pasos

1. Crear UI
2. Buscar catálogos de materiales y sus propiedades
   1. Propiedades: Densidad, esfuerzo máximo de fluencia, resistencia máxima...
   2. Características: Resistencia a la corrosión, soldabilidad, resistencia al calor...
3. Llenar los datos de aplicaciones, materiales, geometrías y demás en Excel
4. Crear un código para llenar dichos datos en la DB. Revisarlo cada vez que se inicie la aplicación.
   1. Para cada hoja en el Excel, crear una tabla o revisar que exista
   2. Revisar la estructura de la tabla en SQLite
   3. Revisar que exista cada registro de la hoja de Excel. Si no existe en la hoja, eliminarlo de la DB; o insertarlo si está en el Excel y no existe en la hoja.
5. Crear clases para modelos de aplicaciones, geometrías, etc.
6. Determinar las ecuaciones que gobiernan aplicaciones y geometrías.
7. Crear objetos de aplicaciones y geometrías basados en las interacciones del usuario
8. Aplicarlo todo en la aplicación.