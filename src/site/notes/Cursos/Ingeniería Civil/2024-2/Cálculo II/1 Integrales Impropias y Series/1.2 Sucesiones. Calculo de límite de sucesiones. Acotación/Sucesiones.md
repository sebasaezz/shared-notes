---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-2-sucesiones-calculo-de-limite-de-sucesiones-acotacion/sucesiones/","tags":["I1MAT1620"]}
---

# Concepto

Funciones con números naturales

# Definición
## Notación

Hay dos notaciones, ahora se muestran ejemplo:

$$
\left\{ \frac{n}{n+a} \right\} _{n=1}^{\infty} \equiv a _{n}=\frac{n}{n+1} \equiv\left\{ \frac{1}{2}, \frac{2}{3}, \frac{3}{4}, \frac{4}{5}, \dots, \frac{n}{n+1},\dots \right\}  
$$
## Sucesiones recurrentes

Sucesiones que se repiten, por ejemplo, la sucesión de Fibonacci

Primero se definen los primeros términos

$a_{1}=1$

$a_{2}=1$

Ahora se define la sucesión:

$$
a_{n+1}=a_{n}+a_{n-1}
$$

Esto nos lleva a una sucesión en la forma:

$$
\left\{ 1,1,2,3,5,8,13,\dots \right\} 
$$

# Convergencia de sucesiones

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-2-sucesiones-calculo-de-limite-de-sucesiones-acotacion/convergencia-o-divergencia-y-limite-de-una-sucesion/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Concepto
# Definición

> [!definition] Límite de una sucesión
> Una [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.2 Sucesiones. Calculo de límite de sucesiones. Acotación/Sucesiones\|sucesión]] $\left\{ a_{n} \right\}$ tiene el límite $L$ y lo expresamos como
> $
> \lim_{ n \to \infty } a_{n} \equiv a_{n} \to L \text{ cuando } n \to \infty
> $
> Si para todo $\varepsilon>0$ hay un correspondiente entero $N$ tal que:
> $
> n>N\implies |a_{n}-L|<\varepsilon
> $


Muy similar a los [[Cursos/Ingeniería Civil/2024-1/Cálculo I/1 Limites y Continuidad/Límites al infinito#^58c26e\|límites al infinito]] de una función

![Pasted image 20240812121001.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/1%20Integrales%20Impropias%20y%20Series/1.2%20Sucesiones.%20Calculo%20de%20l%C3%ADmite%20de%20sucesiones.%20Acotaci%C3%B3n/attachments/Pasted%20image%2020240812121001.png)

Todo el trabajo está en dejar el $N$ en función de $\varepsilon$.

## Similitud entre una sucesión y una función

> [!theorem] similitud entre sucesión y función
> Si $\lim_{ x \to \infty } f(x)=L$ y $f(n)=a_{n}:n\in \mathbb{Z}$ entonces $\lim_{ n \to \infty } a_{n}=L$


Además se pueden aplicar teoremas relacionados a funciones, como el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/1 Limites y Continuidad/Teorema de compresión (sandwich) y límites notables\|Teorema de compresión (sandwich)]].

De aquí que se cumplirá el siguiente teorema:

> [!theorem] límite del valor absoluto de una sucesión cuando tiende a 0
>  $\lim_{ n \to \infty } |a_{n}|=0 \implies \lim_{ n \to \infty } a_{n}=0$

## Teorema de la sucesión monótona

> [!theorem] teorema de las sucesión monótona
> Toda sucesión [[Cursos/Ingeniería Civil/2024-2/Cálculo II/1 Integrales Impropias y Series/1.3 Sucesiones monótonas y acotadas/Sucesiones monótonas y acotadas\|monótona]] y acotada converge a un valor


# Ejemplo
## Ejemplo 1

Demostrar el siguiente límite:

$
\lim_{ n \to \infty } \frac{1}{n}=0
$

Se dice que para todo $\varepsilon>0$ se quiere buscar un número natural $N>0$ tal que:

$
n>N \implies |\frac{1}{n}<\varepsilon|
$

Ahora se puede tomar el valor de $N=\frac{1}{\varepsilon}<n$

Demostrando:

$
\forall\varepsilon>0 \, \,\,\exists N> \frac{1}{\varepsilon}:n>N\implies n> \frac{1}{\varepsilon} \equiv\varepsilon> \frac{1}{n}
$


</div></div>

# Ejemplo