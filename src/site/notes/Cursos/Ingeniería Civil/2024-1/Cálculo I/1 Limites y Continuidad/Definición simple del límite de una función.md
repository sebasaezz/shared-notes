---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/1-limites-y-continuidad/definicion-simple-del-limite-de-una-funcion/"}
---

Dada la siguiente expresión:

$$\lim_{ x \to a }f(x)=L$$

$f(x)$ tiende a $L$ cuando $x$ tiende a $a$

Se dice que el límite existe, y es igual a $L$

No se requiera que $f(a)$ exista para que el límite existe, y $f(a)$ no necesita ser igual a $L$.

Ejemplo:

Considere la siguiente función:

$$
f(x)=\frac{x^{2}-1}{x-1}
$$

Dominio: $\mathbb{R}-\{1\}$

Graficar:

Para graficar se puede simplificar, dejando la función con restricción en 1.

$$
f(x)=\frac{x^{2}-1}{x-1}=\frac{(x+1)(x-1)}{x-1}=x+1
$$

definiendo una función $g$ tal que:

$$
g(x)=x+1|x\ne 1
$$

Ejemplo 2:

$$f(x)=\begin{cases}
\frac{x}{\sqrt{|x|}} & , & x\neq 0\\1&,&x=0
\end{cases}$$
$\lim_{ x \to 0 }f(x)=\text{0}$, pero $f(0)=1$
Para llegar a esta conclusión se debe racionalizar, considerando los dos casos del valor absoluto.
Así:
$$f(x)=\begin{cases}
\sqrt{ x } & , & x> 0\\-\sqrt{x  }&,&x<0\\1&,&x=0
\end{cases}$$
# Límites laterales
Un límite está definido si los dos límites laterales son iguales.
Es decir:
$$

\lim_{ x \to a }f(x) 

$$
está definido sí y solo sí
$$

\lim_{ x \to a^{-} }f(x)=\lim_{ x \to a^{+} }f(x)

$$
