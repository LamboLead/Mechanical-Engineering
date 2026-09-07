---
id: 5hswefag4bglgtpglb8d3ga
title: Notas
desc: ''
updated: 1732653863465
created: 1732648126751
---

## Sistemas de ecuaciones lineales

### Analizando convergencia

**Instrucciones de casos especiales**

- `eig(A)`: Matriz definida positiva
- `eigs(A)`: Matriz 

**Instrucciones de corolario:**

- `T_j = inv(D)*(L+U)`
- `T_gs = inv(D-L)*U`
- `T_w = inv(D-wL)*((1-w)D+(wU))`

### Calculando iteraciones

Para aproximar la solucion del sistema, se utilizan los archivos de rutinas `*.m`.

---
# Ejercicios

1. Ejemplo de clase pasada

```matlab
A = [2 1 -1; 3 5 -5; 1 -1 -2]
b = [1 -1 0]' % Transpuesta (vector columna)
```

Dado que no hay casos especiales, analizando los corolarios:

```matlab
D = diag(A) % Extraer diagonal principal de la matriz
D = diag(diag(A)) % D se construye así. Crea una matriz diagonal con el vector diag(A)
U = D-triu(A) % Extrae la diagonal superior, incluyendo la diagonal
L = D-tril(A) % Extrae la resta de la matriz diagonal inferior

D+L+U==A % Verificación de que es correcto
D-L-U == A % Verificación de que la matriz es correcta al recuperar la matriz A

format rat % Formato racional
format short % Formato corto
format long % Formato largo

Tj = inv(D)*(L+U) % Matriz de Jacobi
eig(Tj) % Valores propios de la matriz de Jacobi

abs(ans) % Valor absoluto del último valor
```

Luego de verificar convergencia, realizando iteraciones (abriendo la rutina de Jacobi)

```matlab
% jacobi(Matriz de sistema, vector b, aproximación inicial, tolerancia, máx iteraciones)

X = jacobi(A, b, [1 1 1]', 1e-4, 100) % Debería converger a 15
residual = A*X-b

% Normas
norm(residual, 1)
norm(residual, inv)
norm(residual) % Norma 2
norm(residual, "fro") % Norma de frobenius

```

Por Gauss-Seidel:
```matlab
Tgs=(D-L)*inv(U) % Matriz de Gauss-Seidel
eig(Tgs)
radioEspectralTgs=max(abs(eig(Tgs))) % Radio espectral (igual a 0.5)

% gseid(Matriz, vector b (columna), aproximación inicial, tolerancia, máx. iteraciones)
Y = gseid(A, b, [1; 1; 1], 1e-4, 100) % Debería converger en 16 iteraciones; Y = [0.8571; -0.1905; 0.5238]
```

¿A esta matriz se le puede aplicar el método de sobrerelajación? Sí (¿cuándo esto no es posible?)
```matlab
% Sobrerrelajación
w = 1.5
Tw = inv(D-w*L)*((1-w)*D+w*U)
% Revisando convergencia
radioEspectralTw = max(abs(eig(Tw))) % Igual a 1.21

% Tomando w = 0.8
w = 0.8 % radio espectral igual a 0.48. Es mejor

% Evaluando con el método
% sor(Matriz A, vector columna b, aprox. inicial, omega, tolerancia, máx. iteraciones)
Z = sor(A, b, [1; 1; 1], 0.8, 1e-4, 100) % Converge en 14 iteraciones
```

2. Matriz de orden 4x4 tridiagonal especial (ejemplo de sobrerrelajación)

```matlab
A = [1 -2 0 0; -2 5 4 0; 0 4 17 3; 0 0 3 30]
b = [1 2 0 -1]''

eig(A) % Valores propios positivos. Converge por Jacobi, GS y Sobrerrelajación

D = diagg(diag(A))
L = D-tril(A)
U = D-triu(A)
D-L-U==A % Confirmación
Tj = inv(D)*(L+U)
radioEspectralTj=max(abs(eig(Tj)))
w = 2/(1+sqrt(1-radioEspectralTj*radioEspectralTj))
radioEspectralW = w - 1
radioEspectralGS = reTj*reTj % Radio espectral de GS es igual a reTJ^2

X = sor(A, b, [1 1 1 1]', w, 1e-4, 10000) % Converge en 61 iteraciones
```

Entre las tres aproximaciones, ¿cuál está más cerca a la solución del sistema?
R. La que posea un residual más pequeño, o la norma de la última iteración sea más pequeña.

3. Matriz giganta
```matlab
clc % Limpia ventana de comandos
clear % Limpia variables
A = gallery("poisson", 100) % Obtención de matriz 100x100 a partir del problema de Poisson

D = diagg(diag(A))
L = D-tril(A)
U = D-triu(A)
Tj = inv(D)*(L+U)

radioEspectralTj=max(abs(eigs(Tj))) % 'eigs' se utiliza para almacenamientos 'sparce'.
w = 2/(1+sqrt(1-radioEspectralTj*radioEspectralTj))
radioEspectralW = w - 1
radioEspectralGS = reTj*reTj % Radio espectral de GS es igual a reTJ^2
```

## Para sistemas no lineales (Método de Newton)

> Las rutinas no realizan análisis de convergencia. Haciendo uso de ellas se asume que el sistema ya converge.

### Ejercicio

$$
ln(x^2y^2)-xy-1 \\
x^2-y^3-4
$$

```matlab
grafico1 = ezplot('log(x^2*y^2)-x*y-1', [-6 6 -6 6]) % Gráfica de primera función, restringida entre -6, 6 en x, y. Guardado dentro de 'grafico1' sin mostrar

set(grafico1, 'color', [1 0 0])
set(grafico1, 'LineWidth', 2)
hold on
grafico1 = ezplot('x^2*y^3-4')
set(grafico1, 'LineWidth', 2)

% Método de Newton para sistemas no lineales
% newdim(...)
F = @(x) [log(x(1)^2*x(2)^2)-x*y-1, x(1)^2-x(2)^3-4] % función anónima que depende del vector 'x' (con componentes x1, x2). El campo vectorial F es un vector fila en la rutina
JF = @(x) [2/x(1)-x(2) 2/x(2)-x(1); 2*x(1) -3*x(2)^2] % Matriz jacobiana

% Uso de la rutina
[P, iter, err] = newdim(F, JF, [-2 0.5], 1e-4, 1e-4, 80) % Converge en 3 iteraciones


Leer lagrange

```