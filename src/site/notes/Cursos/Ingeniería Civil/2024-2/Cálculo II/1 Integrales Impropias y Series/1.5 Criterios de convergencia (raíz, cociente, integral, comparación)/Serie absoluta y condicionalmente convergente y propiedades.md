---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-5-criterios-de-convergencia-raiz-cociente-integral-comparacion/serie-absoluta-y-condicionalmente-convergente-y-propiedades/","tags":["I1MAT1620"]}
---


> [!definition] serie absolutamente convergente
> Una serie $\sum a_{n}$ se llama **absolutamente convergente** si la serie de valores absolutos $\sum |a_{n}|$ converge.
{ #357ae8}


> [!theorem] convergencia de series absolutamente convergentes
> Una serie [[#^357ae8|absolutamente convergente]] siempre va a converger. 
{ #8fcaf0}


`\begin{proof}`

Utilzando el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/1 Limites y Continuidad/Teorema de compresión (sandwich) y límites notables\|teorema del sandwich]]:

Suponiendo que es absolutamente convergente ($\sum |a_{n}|$ converge)

Entonces $\sum2|a_{n}|$ también converge.

$$
\begin{align}
-|a_{n}| & \leq a_{n}\leq |a_{n}| \\
0 & \leq a_{n}+|a_{n}|\leq 2|a_{n}|
\end{align}
$$

Ahora se puede aplicar el [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.1 Integrales impropias. Criterios de comparación/Teorema de comparación y teorema de comparación al límite#^7b850a\|test de comparación]] (primer caso), se tendrá que si $\sum 2|a_{n}|$ converge, y la función al interior es mayor o igual que $a_{n}+|a_{n}|$, entonces $\sum(a_{n}+|a_{n}|)=\sum a_{n}+\sum |a_{n}|$ converge, implicando que $\sum a_{n}$ converge.

`\end{proof}`

> [!definition] serie condicionalmente convergente
> Una serie $\sum a_{n}$ se llama **condicionalmente convergente** si es convergente, pero no [[#^357ae8|absolutamente convergente]].