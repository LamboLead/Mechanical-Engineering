---
id: 8fxmogqcf29t338jyj2ivwz
title: Estructura de datos
desc: ''
updated: 1709734716675
created: 1709073969127
---

A continuación se muestra la estructura de la base de datos a elegir para el aplicativo de selección de materiales.

## Tablas

### _units_

Esta tabla pretende guardar todas las unidades de medida utilizadas en el aplicativo.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la unidad | INTEGER |
| `Name` | Nombre de la unidad | TEXT |
| `Units` | Unidades en Sistema Internacional | TEXT |
| `Measures` | Nombre de la propiedad física o característica relacionada con la unidad de medida | TEXT |

### _properties_

Esta tabla pretende guardar las propiedades mecánicas, físicas y químicas más relevantes de los materiales y presentaciones presentes en el aplicativo.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la propiedad | INTEGER |
| `Name` | Nombre de la propiedad | TEXT |
| `Symbol` | Texto en LaTEX con el símbolo correspondiente de la propiedad | TEXT |
| `Unit_Id` | Asocia la unidad de medida con el campo `units.Id` | INTEGER |

### _characteristics_

Esta tabla pretende guardar las características cualitativas y cuantitativas más relevantes de los materiales y presentaciones presentes en el aplicativo.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la característica | INTEGER |
| `Name` | Nombre de la característica | TEXT |
| `Unit_Id` | Asocia la unidad de medida con el campo `units.Id` | INTEGER |

### _geometry_classification_

Esta tabla pretende guardar los tipos de geometrías a analizar en la aplicación.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la clasificación | INTEGER |
| `Name` | Nombre de la clasificación de la geometría | INTEGER |

### _geometries_

Esta tabla pretende guardar todas las geometrías disponibles para las cuales se puede conseguir determinado material.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la geometría | INTEGER |
| `Name` | Nombre de la geometría | TEXT |
| `GeometryClassification_Id` | Asocia el tipo de geometría con el campo `geometry_classification.Id` | TEXT |
| `Image` | Imagen de la geometría, con sus dimensiones especificadas | BLOB |

### _r_dimensions_geometries_

Esta tabla pretende relacionar geometrías con las dimensiones asociadas a dicha geometría.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|---|
| `Id` | Id de la relación entre dimensión y geometría
 | INTEGER |
| `Variable` | Letra que aparecerá en la imagen del campo `geometries.Image` | TEXT |
| `Units_Id` | Asocia la unidad de medida con el campo `units.Id` | INTEGER |
| `Geometry_Id` | Asocia la geometría con el campo `geometries.Id` | INTEGER |

### _application_classification_

Esta tabla pretende guardar información sobre los tipos de aplicaciones de ingeniería a trabajar dentro de la aplicación.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id del tipo de aplicación | INTEGER |
| `Name` | Nombre del tipo de aplicación | TEXT |

### _applications_

Esta tabla pretende guardar información sobre las diferentes aplicaciones de ingeniería a seleccionar dentro de la aplicación.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|---|
| `Id` | Id de la aplicación | INTEGER |
| `Name` | Nombre de la aplicación | INTEGER |
| `ApplicationClassification_Id` | Asocia el tipo de aplicación con el campo `application_classification.Id` | INTEGER |
| `Description` | Descripción detallada de la aplicación | TEXT |

### _r_applications_geometries_

Esta tabla pretende relacionar todas las aplicaciones de ingeniería con las geometrías disponibles para dicha aplicación (por ejemplo, 'flexión' con 'Vigas en I').

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la relación | INTEGER |
| `Image` | Imagen que muestra la geometría y su respectiva aplicación | BLOB |
| `Geometry_Id` | Asocia la geometría con el campo `geometries.Id` | INTEGER |
| `Application_Id` | Asocia la aplicación con el campo `applications.Id` | INTEGER |

### _material_classification_

Esta tabla pretende guardar información sobre las clasificaciones y subclasificaciones de los materiales existentes en la aplicación.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la clasificacion de materiales | INTEGER |
| `Name` | Nombre de la clasificación | TEXT |
| `ParentId` | Id de la clasificacion a la que pertenece la actual | INTEGER |

### _materials_

Esta tabla prentende guardar información sobre todos los materiales existentes en la aplicación.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id del material | INTEGER |
| `Name` | Nombre o denominación del material | TEXT |
| `CommonName` | Nombre común del material en el mercado | TEXT |
| `MaterialClassification_Id` | Asocia el tipo o clasificación del material con el campo `material_classification.Id` | INTEGER |
| `Image` | Imagen del material en su naturaleza | BLOB |
| `Composition` | Composición química de los elementos que conforman al material | TEXT |

### _suppliers_

Esta tabla pretende guardar la información relativa a los proveedores consultados para la recolección de información de materiales y sus presentaciones en este aplicativo.

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id del proveedor | INTEGER |
| `Name` | Nombre del proveedor (empresa) | TEXT |
| `Phone` | Teléfono del proveedor | TEXT |
| `Address` | Dirección del proveedor | TEXT |

### _r_materials_presentations_

Esta tabla pretende relacionar los materiales de la tabla de `materials` con las presentaciones en las que se encuentran en el mercado colombiano y sus proveedores, de la tabla `suppliers`.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la relación | INTEGER |
| `Name` | Nombre completo de la presentación en la que se encuentra el elemento | INTEGER |
| `Price` | Precio por kilo de dicha presentación del material | FLOAT |
| `Image` | Imagen relativa al material y su presentación | BLOB |
| `Material_Id` | Asocia el material relacionado a la presentación con el campo `materials.Id` | INTEGER |
| `Supplier_Id` | Asocia el proveedor relacionado a la presentación con el campo `suppliers.Id` | INTEGER |
| `CatalogCode` | Código de la presentación del material en el inventario o catálogo de dicho proveedor | TEXT |

### _r_presentations_properties_

Esta tabla pretende relacionar cada una de las presentaciones de los materiales con sus propiedades mecánicas, físicas y químicas.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la relación | INTEGER |
| `Value` | Valor de dicha propiedad | Value |
| `RMaterialsPresentations_Id` | Asocia la presentación de cierto material con el campo `r_materials_presentations.Id` | INTEGER |

### _r_presentations_characteristics_

Esta tabla pretende relacionar cada una de las presentaciones de los materiales con sus características.

**Campos:**

| Nombre | Descripción | Tipo |
|:---:|---|
| `Id` | Id de la relación | INTEGER |
| `Value` | Valor de la característica del material/presentación | TEXT |
| `RMaterialsPresentations_Id` | Asocia la presentación de cierto material con el campo `r_materials_presentations.Id` | INTEGER |


## Preguntas
- Sabemos que los materiales que nos dan los proveedores vienen por presentaciones ¿La presentación en la que se encuentra cierto material en el mercado debería ser la misma que la geometría inicial ingresada por el usuario?
- Sabemos que dependiendo de la presentación y sus procesos de manufactura se van a tener diferentes propiedades para un material. ¿Es necesario discriminar cada presentación que ofrezca algún proveedor para organizar las características y propiedades? O simplemente se dejarían las propiedades y características para el material.
- ¿Qué dimensiones mínimas debería ingresar el usuario? ¿Cómo saber qué dimensión debería ser libre para que el programa la calcule?
- ¿Qué otras características y propiedades son de importancia para el aplicativo?