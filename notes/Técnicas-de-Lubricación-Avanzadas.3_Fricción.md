---
id: dyco2gqzutt25jmc2vkjli8
title: 3 - Fricción
desc: ''
updated: 1736978367140
created: 1736909595486
---

## Tipos de fricción

El tipo de fricción sobre el cual opera el mecanismo define el grosor de la película lubricante $h_l$, y por lo tanto, el tipo de lubricación bajo el cual trabaja el mecanismo:
  
  | Tipo de fricción actuando en la película | Tipo de lubricación |
  |---|---|
  | Fricción sólida permanente | Lubricación Límite (LL) |
  | Fricción mixta permanente | Lubricación Elastohidrodinámica (EHD) |
  | Fricción fluida | Lubricación Hidrodinámica (LHD) |
  | Fricción fluida artificial | Lubricación Hidrostática (LH) |

### Fricción vs. Velocidad, carga y viscosidad

La **curva de Stribeck** describe el comportamiento del coeficiente de fricción $\mu$ en función del parámetro $\eta n/(C_d/A_r)$, con:

- $C_d$: Carga dinámica en el sistema tribológico.
- $n$: Velocidad relativa entre ambas superficies.
- $\eta$: Visosidad del lubricante...

Cuando la velocidad $n$ aumenta, la fricción disminuye y tiende a ser fluida ($\mu = 0.003$). Además, cuando $n$ disminuye, la fricción aumenta y puede ser mixta ($\mu=0.011$) o sólida ($\mu=0.088$).
  
![](/assets/images/2025-01-14-19-50-35.png)

**_(Completar todos los casos de lubricación en la curva de Stribeck. Módulo 1-3_Tipos de lubricación, página 8-37)_**

### Fricción sólida

La fricción sólida se da en régimenes de velocidad bajos, casi en reposo. Al ponerse el mecanismo en operación, sólo está presente la _Capa límite 1_, la velocidad $n$ es baja, pero la carga dinámica $C_d$ es alta, por lo que según la curva de Stribeck, el coeficiente de fricción sólida es alto.

![](/assets/images/2025-01-15-15-00-17.png)

**¿Por qué aparece?** La fricción sólida permanente y lubricación límite (LL) se dan cuando el movimiento es oscilatorio o, generalmente para velocidades menores o iguales a 10rpm.

**Lubricantes utilizados:** Lubricantes sólidos como el grafito o el bisulfuro de molibdeno, que sólo forman la _Capa límite antifricción 1_.

**Mecanismos en los que aparece:** Torones de los cables metálicos, eje de la pinza de sujeción de cabinas de un cable aéreo, en el pasador de cadenas de rodillos, guías de compuertas en embalses de las plantas hidroeléctricas, etc.

![](/assets/images/2025-01-15-15-06-56.png)

![](/assets/images/2025-01-15-15-07-18.png)

### Fricción mixta

Ocurre cuando la velocidad en el mecanismo aumenta, o si la carga disminuye, de tal forma que el parámetro $\eta n/P$ es mayor, haciendo que la fricción sólida empiece a cambiar por mixta, y el coeficiente de fricción mixta empieza a disminuir.

![](/assets/images/2025-01-15-15-09-35.png)

En este tipo de fricción, las crestas en cada superficie se deforman elásticamente, y los modificadores de fricción forman la _Capa Límite 1_, impidiendo que éstas se suelden. La capacidad de carga de dichos aditivos se evalúa con la prueba de las cuatro bolas ASTM D2783 para aceites, y ASTM D2596 para grasas.

![](/assets/images/2025-01-15-15-18-32.png)

**¿Por qué aparece?** La fricción mixta permanente y lubricación Elastohidrodinámica (EHD) aparecen cuando aumenta la velocidad relativa entre ambas superficies, por lo que sólo las crestas de cada superficie interactúan. Por lo tanto, los esfuerzos que soportan dichas crestas son muy altos, y aún es necesario utilizar modificadores de fricción para evitar fricción excesiva en dichos contactos.

**Lubricantes utilizados:** Si la carga es muy alta, se deben utilizar lubricantes con modificadores de fricción _EP3_ o _EP4_. Además, como las velocidades no son muy altas, la viscosidad del lubricante debe ser relativamente alta. 

**Mecanismos en los que aparece:** En la mayoría de los engranajes de los reductores de velocidad, regularmente para relaciones de transmisión de 1 a 4 en adelante. Sin embargo, es necesario analizar cada caso y concluir al respecto.

### Fricción fluida

Ocurre al aumentar la velocidad relativa entre ambas superficies, de una forma tal que el parámetro $\eta n/P$ aumente, y la zona de fricción pase de mixta a fluida. El coeficiente de fricción es mínimo, y no se presenta desgaste adhesivo.

![](/assets/images/2025-01-15-15-40-52.png)

En este régimen de fricción la lubricación es Hidrodinámica (LHD), por lo que se genera la _Capa fluida 3_, que otorga una excelente capacidad de amortiguamiento garantizando la vida disponible de los elementos mecánicos.

![](/assets/images/2025-01-15-15-50-34.png)

**¿Por qué aparece?** En este régimen de operación (fricción fluida), las superficies de fricción se separan completamente por acción del lubricante, y la _Capa Fluida 3_ está presente en un 100%, con un espesor aproximado de $5\mu m$. Por lo tanto, la lubricación es hidrodinámica (LHD).

**Lubricantes utilizados:** Dado el régimen de velocidad, se utilizan lubricantes de grado ISO 100 o menores, con aditivos antifricción AW.

**Mecanismos en los que aparece:** Rodamientos de bombas centrífugas de alta velocidad (1800rpm). Reductores de velocidad con relaciones de transmisión iguales o por debajo de 1:3.

### Fricción fluida artificial

En este caso, la fricción fluida se da gracias al bombeo de lubricante, separando ambas piezas en contacto.

**¿Por qué aparece?** La fricción fluida artificial y lubricación hidrostática (LH) se da gracias al bombeo intencional de lubricante, que genera la película de lubricante de forma artificial.

**Mecanismos en los que aparece:** Cojinetes de empuje de las turbinas Pelton, Francis y Kaplan, o los cojinetes lisos en los molinos de bolas.

![](/assets/images/2025-01-15-16-08-56.png)

## Factor de seguridad de la película lubricante $\lambda$

La selección del tipo de lubricante va en función del tipo de fricción que se dé en el mecanismo, así como de las condiciones de operación (velocidad, carga dinámica, temperatura y rugosidad). Dicha selección debe garantizar que el **factor de seguridad de la película lubricante** $\lambda$ sea el correcto.

**Factor de seguridad de la película lubricante:** $\lambda = h_l / \rho_p$; con:
- $h_l$: Espesor de la película lubricante.
- $\rho_p$: Rugosidad promedio entre las dos superficies en contacto.

| Factor $\lambda$ | Tipo de fricción | Tipo de lubricación |
|:---:|---|---|
| $\lambda < 1$ | Fricción sólida | Lubricación límite (LL) |
| $\lambda < 1$ | Fricción mixta | Lubricación Elastohidrodinámica (EHL) |
| $\lambda = 1$ | Transición entre fricción mixta y fluída | Lubricación hidrodinámica (LHD) |
| $\lambda > 1$ | Fricción fluida | Lubricación Hidrodinámica (LHD) |

El valor de $\lambda$ depende de las condiciones operacionales reales de cada mecanismo, como la velocidad, carga dinámica, temperatura de operación y rugosidad de las superficies de operación.

### Rugosidad

La rugosidad entre las superficies en contacto la define el fabricante del mecanismo, y para el cálculo del factor $\lambda$ se utiliza la **rugosidad media cuadrada (RMS)** $\rho_p$:

**Rugosidad media cuadrada:** $\rho_p = \sqrt{\rho_1^2 + \rho_2^2} \space [\mu m]$

**Rugosidad estándar:**

La rugosidad está estandarizada bajo la _Norma ISO 468-1982_, que se resume a continuación:

![](/assets/images/2025-01-14-20-31-40.png)

> El **tipo de lubricación** depende del **tipo de fricción** que presente el mecanismo. Una correcta selección del lubricante garantiza un valor correcto del **factor de seguridad de la película lubricante** $\lambda$.

> Como referencia, se puede tener que:
> - Para velocidades superiores a 450rpm, la fricción es fluida y la lubricación es hidrodinámica.
> - Para velocidades inferiores a 450rpm, la fricción puede ser mixta y la lubricación es elastohidrodinámica; o la fricción puede ser sólida y la lubricación puede ser límite.

![](/assets/images/2025-01-14-20-12-11.png)

### Cálculo del factor $\lambda$

#### Cálculo para rodamientos

El cálculo del factor $\lambda$ para rodamientos se realiza con la fórmula común del factor: $\lambda = h_l/\rho_p$.

La película lubricante se calcula con:

$$
  h_l = LCD_{ext}n^{0.74} \space [\mu m]
$$
con:
- $L \space [cSt]$: Viscosidad a la temperatura de operación determinada $T_{op}$.
- $C$: Factor geométrico del rodamiento.
- $D_{ext} \space [m]$: Diámetro exterior del anillo giratorio.
- $n \space [rpm]$: Velocidad del rodamiento.

**Factor geométrico del rodamiento $C$, según el caso:**
![](/assets/images/2025-01-15-16-53-47.png)

**Viscosidad del lubricante $L$:** Se halla con base en el grado ISO del lubricante utilizado y la temperatura de operación determinada. Se traza la curva del aceite en el gráfico _ASTM D341_, con su viscosidad a 40°C y a 100°C. El parámetro $L$ será la viscosidad a la temperatura de operación determinada.

Ejemplo con un aceite ISO 150, con una $T_{op} = 60°C$:
![](/assets/images/2025-01-15-16-58-08.png)   


#### Cálculo para cojinetes lisos

_(página 48)_

#### Cálculo para engranajes

El factor $\lambda$ de la película lubricante para engranajes se halla a partir del siguiente gráfico:

![](/assets/images/2025-01-15-16-35-56.png)

Es necesario Hallar la velocidad lineal a la que se mueve la periferia de los engranajes, con la siguiente fórmula:
$$
v_{lineal} = \pi D_{p,1}n_1 = \pi D_{p,2}n_2 \space [m/s]
$$
con:
- $D_{p,1}, D_{p,2} \space [m]$: Diámetro de paso del piñón 1 y 2, en metros.
- $n_1, n_2 \space [rps]$: Velocidad de rotación del piñón 1 y 2
  
Luego, se trazar una línea vertical en la intersección con el eje $x$ con el valor de velocidad lineal.   
Por último, en la intersección con la curva, trazar una línea horizontal hasta el eje $y$ para hallar el valor de factor $\lambda$.