---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/2-ecuaciones-diferenciales-homogeneas/ecuacion-de-ricatti/","tags":["ExMAT1640"]}
---

# Concepto
Típicamente, una ecuación de grado $2$ no tiene una fórmula, pero si se conoce UNA solución particular de la misma ecuación ya se puede resolver. 
# Definición

> [!theorem] ecuación de Riccati
> Una ecuación de Riccati tiene la forma:
> $$
> \frac{ dy }{ dx } =A(x)+B(x)y+C(x)y^{2}
> $$
> Y si se conoce una solución $y_{0}(x)$, entonces la sustitución:
> $$
> y=u+y_{0}
> $$
> la va a transformar en una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/2 Ecuaciones diferenciales homogeneas/Ecuación de Bernoulli (EDO)\|ecuación de Bernoulli]].
> Si se hace le reemplazo:
> $$
> y=\frac{1}{u}+y_{0}
> $$
> Entonces se va a transformar en una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/EDOs lineales de primer orden y factor integrante\|EDO lineal de primero orden]].

`\begin{proof}`
Sea:
$$
\frac{ dy }{ dx } =A(x)+B(x)y+C(x)y^{2}
$$
Con solución $y_{0}$, se hace el reemplazo:
$$
y=u+y_{0}
$$
El cual si se integra se obtiene:
$$
\frac{ dy }{ dx } =\frac{ du }{ dx } +\frac{ dy_{0} }{ dx } 
$$
Como $\frac{ dy }{ dx }=\frac{ dy_{0} }{ dx }$:
$$
\begin{align}
\cancel{ A(x) }+B(x)y+C(x)y^{2}  & =\frac{ du }{ dx } +\cancel{ A(x) }+B(x)y_{0}+C(x)y_{0}^{2} \\
\frac{ du }{ dx }  & =B(x)(y-y_{0})+C(x)(y^{2}-y_{0}^{2})
\end{align}
$$
Por la definición de $u$:
$$
y-y_{0}=u
$$
$$
\begin{align}
(y-y_{0})(y+y_{0}) & =u·(u+2y_{0}) \\
y^{2}+y_{0}^{2} & =u^{2}+2uy_{0}
\end{align}
$$
Finalmente:
$$
\frac{ du }{ dx } =B(x)u+C(x)(u^{2}+2uy_{0})
$$
Esto es una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/2 Ecuaciones diferenciales homogeneas/Ecuación de Bernoulli (EDO)\|ecuación de Bernoulli]], ya que se puede poner de la forma:
$$
\frac{ du }{ dx } =(B(x)+2y_{0}C(x))u+C(x)u^{2}
$$
Y la sustitución
$$
w=u^{1-2}=\frac{1}{u}
$$
La transforma en una [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/EDOs lineales de primer orden y factor integrante\|EDO lineal de primer orden]].
Esto también demuestra el punto 2 del teorema
`\end{proof}`
# Ejemplo
$$
y^{2}+y'=x^{2}+1
$$
$y=x$ funciona, es solución particular.
El cambio será:
$$
y=u+x\implies y'=u'+1
$$
$$
(u+x)^{2}+u'+1=x^{2}+1
$$
$$
u^{2}+2ux+u'=0
$$
Esto es bernullo
