---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-3-sucesiones-monotonas-y-acotadas/sucesiones-monotonas-y-acotadas/","tags":["I1MAT1620"]}
---


# Monotonía
Sucesiones que crecen o decrecen constantemente

> [!definition] Monotonía de una una sucesión
> Una sucesión $a_{n}$ es creciente si $a_{n}<a_{n+1}\forall n\in\mathbb{N}$, y es decreciente si $a_{n}>a_{n+1} \forall n \in \mathbb{N}$. Una sucesión es monótona si es creciente o decreciente.
{ #78061f}


Para demostrar monotonía, se debe utilizar [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.3 Sucesiones monótonas y acotadas/Desmotración por inducción\|Desmotración por inducción]].
# Sucesiones acotadas

> [!definition] Sucesión acotada
> Una sucesión es acotada por arriba si es que:
> $$
> \exists M: a_{n} \leq M \space\space \forall n\in\mathbb{N}
> $$
> Y una sucesión está acotada por abajo si es que:
> $$
> \exists M: a_{n} \geq m \space\space \forall n\in\mathbb{N}
> $$
> Una sucesión es **acotada** si es que está acotada tanto por arriba como por abajo.
{ #480642}


## Teorema de la sucesión monótona


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-2-sucesiones-calculo-de-limite-de-sucesiones-acotacion/convergencia-o-divergencia-y-limite-de-una-sucesion/#3f27fe" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] teorema de las sucesión monótona
> Toda sucesión [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.3 Sucesiones monótonas y acotadas/Sucesiones monótonas y acotadas\|monótona]] y acotada converge a un valor

</div></div>
 

# Ejemplo

## Ejemplo 1
{ #9a1eb4}


Demostrar que $a_{1}=2, a_{n+1}=\frac{1}{2}(a_{n}+6)$ es creciente

[[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.3 Sucesiones monótonas y acotadas/Desmotración por inducción\|Desmotración por inducción]]:

Primero se demuestra verdadero para $n=1$:

$a_{2}=\frac{1}{2}(2+6)= 4>2$

Se establece la hipótesis de inducción.

Se supone que el $a_{n}<a_{n+1}$ (ya se demostró), y se quiere demostrar que $a_{n+1}<a_{n+2}$

$$
\begin{align}
a_{n} & <a_{n+1} \\
a_{n}+6 & < a_{n+1}+6 \\
\frac{1}{2}(a_{n}+6) & < \frac{1}{2}(a_{n+1}+6) \\
a_{n+1}&<a_{n+2}
\end{align}
$$
