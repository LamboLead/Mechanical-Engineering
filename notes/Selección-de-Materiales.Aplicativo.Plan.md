---
id: 2kbwgslcztcyax9w5h4293w
title: Plan - MSelector
desc: ''
updated: 1711299903224
created: 1711299372288
---

Este documento contiene el plan de trabajo para el desarrollo del aplicativo _MSelector_ para Selección de Materiales.

## 1. Interfaz de usuario

## 2. Actualización de base de datos

1. Buscar o crear una clase que se integre fácilmente con la base de datos (como un XPO para MatLab) y que pueda funcionar como clase pariente de las clases de Materiales, Presentaciones, Proveedores, etc.
2. Crear cada una de las clases que correspondan con la estructura de la base de datos:
   - Materiales
   - Presentaciones
   - Proveedores
   - Propiedades
   - Características
   - Unidades
   - etc...
3. Integrar cada una de las clases anteriores con la interfaz de actualización de base de datos.