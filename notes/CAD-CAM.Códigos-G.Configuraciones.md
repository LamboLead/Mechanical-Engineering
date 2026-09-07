---
id: 0y1qdfz3m6vyauwlf7h8qcm
title: Configuraciones
desc: ''
updated: 1708661979579
created: 1707870509829
---

# Configuraciones

A continuación hay una lista de códigos G relacionados con configuraciones

## Sistema de coordenadas y planos

| Código | Nombre | Descripción / Uso| Tener en cuenta |
|:---:|---|---|---|
| `G17` | Mecanizado en plano XY | Utiliza el plano XY para realizar el mecanizado |
| `G18` | Mecanizado en plano XZ o ZX | Utiliza el plano XZ o ZX para realizar el mecanizado |
| `G19` | Mecanizado en plano YZ | Utiliza el plano YZ para realizar el mecanizado |
| `G90` | Sistema de coordenadas absoluto | Define el sistema de coordenadas relativo al origen definido, o a definir. |
| `G91` | Sistema de coordenadas incremental | Define el sistema de coordenadas relativo al último punto de movimiento. |
| `G54` | Coordenadas de trabajo 1 |  |
| `G55-G59` | Coordenadas de trabajo 2-6 |  |

## Unidades de medida

| Código | Nombre | Descripción / Uso| Tener en cuenta |
|:---:|---|---|---|
| `G20` | Usar pulgadas | Configura _pulgadas_ como unidad de medida. |  |
| `G21` | Usar milímetros | Configura _milímetros_ como unidad de medida. |  |

### Posicionamiento y compensación
| Código | Nombre | Descripción / Uso| Tener en cuenta |
|:---:|---|---|---|
| `G32` | Ir a punto de seguridad | Lleva el husillo hasta el punto de seguridad o de cambio de herramienta |
| `G40` | Cancelar compensación radial | Elimina la compensación radial predefinida. |
| `G41` | Definir compensación radial hacia la izquieda | Define una compensación radial cuando la herramienta está a la izquierda de la dirección del contorno. | La compensación se define con el radio de la herramienta utilizando el comando `D` |
| `G42` | Definir compensación radial hacia la derecha | Define una compensación radial cuando la herramienta está a la derecha de la dirección del contorno. | La compensación se define con el radio de la herramienta utilizando el comando `D` |
| `G43` | Adicionar compensación de altura de herramienta |  |
| `G44` | Restar compensación de altura de herramienta |  |

<!-- 
### Pausas
| Código | Nombre | Descripción | Ejemplo |
|:---:|---|---|---|
| `G0` |  |  |
| `G0` |  |  |
| `G0` |  |  |
| `G0` |  |  |
| `G0` |  |  |

![](/assets/images/2024-02-13-19-27-52.png)

![](/assets/images/2024-02-13-19-28-02.png) -->