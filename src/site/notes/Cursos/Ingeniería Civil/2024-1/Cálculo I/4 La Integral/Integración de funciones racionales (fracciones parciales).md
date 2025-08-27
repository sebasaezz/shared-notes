---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/integracion-de-funciones-racionales-fracciones-parciales/","tags":["ExMAT1610","Técnicas-de-integración"]}
---

# Concepto

Integrar una función racional

Considerando la siguiente función:

$$
f(x)=\frac{g(x)}{h(x)}
$$
# Para fracciones impropias

Eso es que $\operatorname{gra}g(x)>\operatorname{gra}h(x)$

Se debe dividir el polinomio.

## Ejemplo
$$
\int \frac{x^{3}+x}{x-1} \, dx 
$$
**Dividir:**
$$
\begin{array}{r}
x^{3}+x & : &   x-1 & = & x^{2}+x+2 \\
\Large{\frac{-(x^{3}-x^{2})}{x^{2}+x}} \\
\Large{\frac{-x^{2}-x}{2x}} \\
\Large{\frac{-(2x-2)}{2}}
\end{array}
$$

ahora se cumplirá que:

$$
\int \frac{x^{3}+x}{x-1} \, dx =\int x^{2}+x+2+\frac{2}{x-1} \, dx 
$$

$P(x)=D(x)·C(x)+R(x)$

- [x] revisar división de polinomios  [completion:: 2025-04-20]
# Para fracciones propias

Donde $\operatorname{grad}g(x)>\operatorname{grad}h(x)$

## Caso 1: el denominador es un producto de factores lineales distintos
### Ejemplo
$$
\int \frac{x^{2}+2x-1}{2x^{3}+3x^{2}-2x} \, dx 
$$

Ahora:

$$
\frac{x^{2}+2x-1}{2x^{3}+2x^{2}-2x}= \frac{2x+x^2-1}{x(2x-1)(x+2)}
$$

Ahora se considera que:

$$
\begin{align}
\frac{2x+x^2-1}{x(2x-1)(x+2)} & =\frac{A}{x}+\frac{B}{2x-1}+\frac{C}{x+2} \\
 & =\frac{A(2x-1)(x+1)+Bx(x+1)+Cx(2x-1)}{x(2x-1)(x+1)} \\
 & =\frac{(2A+B+2C)x^{2}+(3A+2B-C)x-2A}{x(2x-1)(x+1)}
\end{align}$$
De esto se tiene el siguiente sistema
$$

\begin{cases}

2A+B+2C & =1 \\

3A+2V-C & =2 \\

-2A & =-1

\end{cases}

$$
_Pivoteando (pura algebrita, mi viejo querido)_
$$

B=\frac{1}{5},A=\frac{1}{2},C=-\frac{1}{10}

$$
Ahora se tiene:
$$

\begin{align}

 \int \frac{x^{2}+2x-1}{2x^{3}+3x^{2}-2x} \, dx & =\int \frac{1}{2x}+\frac{1}{5(2x-1)}+\frac{1}{10(x+2)} \, dx \\

 & =\frac{1}{2}\int \frac{1}{x} \, dx  +\frac{1}{5}\int \frac{1}{2x-1} \, dx +\frac{1}{10}\int \frac{1}{x+2} \, dx  \\

 & =\frac{1}{2}\ln |x|+\frac{1}{5}\ln |2x-1|+\frac{1}{10}\ln |x+2|

\end{align}

$$
## Caso 2: El denominador es un producto de factores lineales, donde algunos se repiten
### Ejemplo
$$\int \frac{2x^{2}+4x+1}{x^{3}-x^{2}-x+1} \, dx =\int \frac{2x^{2}+4x+1}{(x-1)^{2}(x+1)} \, dx $$
Se debe hacer el mismo procedimiento, pero considerando la siguiente ecuación:
$$

\frac{2x^{2}+4x+1}{x^{3}-x^{2}-x+1}=\frac{A}{x+1}+\frac{B}{x-1}+\frac{C}{(x-1)^{2}}

$$
## Caso 3: EL denominador contienen factores cuadráticos irreductibles, de los que ninguno se repite
### Ejemplo
$$

\int \frac{2x^{2}-x+4}{x^{3}+4x} \, dx 

$$
Se trata de escribir la fracción comouna suma de fracciones
$$

\frac{2x^{2}-x+4}{x^{3}+4x}=\frac{2x^{2}-x+4}{x(x^{2}+4)}

$$
Se buscan las variables, pero ahora donde hay una expresión cuadrática se tiene un polinomio de grado 1.
$$

\frac{2x^{2}-x+4}{x(x^{2}+4)}=\frac{A}{x}+\frac{Bx+C}{x^{2}+4}

$$
_resolver sistema de ecuaciones_
## Caso 4: Caso 3 pero repetido
La misma idea del caso 2
### Ejemplo
$$

\int \frac{1-x+2x^{2}-x^{3}}{x(x^{2}+1)^{3}} \, dx 

$$
Ahora se reduce la fracción tal como en el caso 2:
$$

\frac{1-x+2x^{2}-x^{3}}{x(x^{2}+1)^{3}} =\frac{A}{x}+\frac{Bx+C}{x^{2}+1}+\frac{Dx+E}{(x^{2}+1)^{2}}+\frac{Fx+G}{(x^{2}+1)^{3}}

$$
