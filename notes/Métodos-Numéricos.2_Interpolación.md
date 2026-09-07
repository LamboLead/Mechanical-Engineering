---
id: 3t9k6e91b2q6djch2e4l0ad
title: 2 - Interpolación
desc: ''
updated: 1733427942207
created: 1733425574656
---


```matlab
f = @(x) 100*exp(-x.*x)./(4*x.*x+1)
fplot(f, [-2,3]) % Grafica la función en el intervalo (-2, 3)
x = linspace(-2, 3, 5) % Crea un vector de cinco valores igualmente espaciados entre -2 y 3
y = f(x) % Hallar imágenes del vector x

% ¿Cómo realizar la instrucción de productoria?

[C, L] = lagran(x, y) % Coeficientes de la potencia más grande a la más pequeña

# Verificación de la función de interpolación
polyval(C, x(1)) % Evaluación del vector x (que debería ser igual a y)
y(1)

xx = linspace(-2, 3, 5000);
yy = polyval(C, xx); % Evalúa el polinomio en el vector 'xx'


% Newton
[C, D] = newpoly(x, y) % Coeficientes de polinomio interpolante con Newton

[Cn, DD] = newpoly(x, y) % Cn son los coeficientes, DD es la tabla de diferencias divididas. El polinomio interpolante debería ser igual al de LaGrange
```

Ejercicio anterior de clase:

```matlab
[Xc, Yc] = nodoschebyshev(f, 4, -2, 3) % Devuelve los nodos de Chebyshev (función, grado del polinomio, intervalo[0], intervalo[1])

plot(xc, yc, 'r.', 'LineWidth', '2')

[Cne, DD] = newpoly(xx, yy);
[Cnc, DD] = newpoly(xc, yc);
yye = polyval(Cne, xx); % Nodos igualmente espaciados
yyc = polyval(Cnc, xx); % Nodos de Chebyshev

```