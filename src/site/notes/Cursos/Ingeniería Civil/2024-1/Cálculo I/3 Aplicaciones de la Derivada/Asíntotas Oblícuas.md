---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/asintotas-oblicuas/","tags":["I3MAT1610"]}
---

# Definición

Se dice que una función $f$ tiene una asíntota oblicua si:

- $\lim_{ x \to \infty } (f(x)-(ax+b))=0$
- $\lim_{ x \to -\infty } (f(x)-(ax+b))=0$
## Recta de asíntota

De lo anterior se deriva que:

Si la asíntota por izquierda está definida por la recta $ax+b$, entonces:

$a=\lim_{ x \to -\infty } \frac{f(x)}{x}$

$b=\lim_{ x \to -\infty } (f(x)-ax)$

Si la asíntota por derecha está definida por la recta $ax+b$, entonces:

$a=\lim_{ x \to \infty } \frac{f(x)}{x}$

$b=\lim_{ x \to \infty } (f(x)-ax)$

Como esto se deriva de la primera definición, entonces no se necesita comprobar lo primero.

```mathematica-plot 
raster:
  dim: 2D
  background: None
  size:
    height: Automatic
    width: "250"
general:
  axes: "True"
  axesLabel: "{x, y}"
  frame: "True"
  boxed: "True"
graphs:
  - id: graph_0
    options: {}
    type: plot
    plot:
      expression: (x^3)/(x^2 - 1)
      plotRange:
        x:
          min: "-5"
          max: "5"
        y:
          min: ""
          max: ""
  - id: graph_1
    options:
      plotStyle: Red
    type: plot
    plot:
      expression: x
      plotRange:
        x:
          min: "-5"
          max: "5"
        y:
          min: ""
          max: ""
 
 ```