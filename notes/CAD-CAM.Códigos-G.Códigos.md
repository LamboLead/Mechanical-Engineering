---
id: c62i67ik03n7034cqxyse53
title: Códigos
desc: ''
updated: 1708662240224
created: 1707869615133
---

# Códigos M

## Inicio, pausa y final de programa
| Código | Nombre | Descripción | Ejemplo |
|:---:|---|---|---|
| `M00` | Parada programada incondicional |  |
| `M01` | Parada programada condicional |  |
| `M02` | Fin de subprograma |  |
| `M30` | Fin de programa |  |

## Rotación del cabezal
| Código | Nombre | Descripción | Ejemplo |
|:---:|---|---|---|
| `M03` | Giro del cabezal en sentido horario |  |
| `M04` | Giro del cabezal en sentido antihorario |  |
| `M05` | Parada del cabezal sin orientación |  |

## Control de refrigerante
| Código | Nombre | Descripción | Ejemplo |
|:---:|---|---|---|
| `M08` | Apertura del líquido refrigerante |  |
| `M09` | Cierre del líquido refrigerante |  |

## Selección de Velocidad de giro
| Código | Nombre | Descripción | Ejemplo |
|:---:|---|---|---|
| `M19` | Parada del cabezal orientado un ángulo bajo _S_ |  |
| `S` | Selección de velocidad de giro |  |

## Selección de herramienta
| Código | Nombre | Descripción | Ejemplo |
|:---:|---|---|---|
| `M06` | Realizar cambio de herramienta |  |
| `T01`, `T02`, ... | Selección de herramienta |  |

**Ejemplo:** Realizar un cambio a la herramienta 6
```gcode
  G32 (Llevar el husillo a la posición de cambio de herramienta)
  T6 M6
```