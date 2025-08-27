---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/integral-indefinida-primitiva-o-antiderivada-general/","tags":["ExMAT1610"]}
---


Se sabe que:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/teorema-fundamental-del-calculo-tfc-y-propiedades/#64cf22" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] Teorema Fundamental del Cálculo (TFC)
> **Parte 1**
> Utilizando el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Teorema de valor medio integral#^c8dc0f\|Teorema de valor medio integral#^c8dc0f]].
> Dada una función se considera la siguiente función integral:
> $
> g(x)=\int_{a}^{x} f(t) \, dt : a\leq x\leq b
> $
> $g$ es continua en $[a,b]$, y derivable en $(a,b)$. Se cumple que:
> $
> g'(x)=f(x)
> $
> **Parte 2**
> De esto se desprende que para $f(x)$ tal que $F(x)$ es la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Integral indefinida, primitiva o antiderivada general\|antiderivada general]] de $f$, se cumplirá que:
> $\int_{a}^{b} f(x) \, dx=F(b)-F(a) =F(x)]^{b}_{a}$

</div></div>
 

Así, para una integral indefinida en la forma:

$$
\int f(x) \, dx =F(x)+c:c\in\mathbb{R}
$$

Donde $F(x)$ es la antiderivada particular.

# Propiedades

Se pueden usar todas las [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Propiedades de la integral definida\|Propiedades de la integral definida]], y las [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Antiderivadas particulares notables, propiedades y leyes\|Antiderivadas particulares notables, propiedades y leyes]] más la constante de integración.