---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/4-la-integral/integrales-trigonometricas/","tags":["ExMAT1610","Técnicas-de-integración"]}
---

# Uso de  [[Conocimientos/Matemática/Pure Mathematics/Structures (algebra)/Algebra/Trigonometría/Identidades trigonométricas#^25ecb8\|identidades pitagóricas]]

Ejemplo:

$$
\int \cos ^{3}(x) \, dx =\int (1-\sin ^{2}x)\cos x \, dx 
$$

[[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Regla de sustitución\|Regla de sustitución]]

$$
\int (1-u^{2}) \, du:u=\sin x \implies du=\cos (x)dx 
$$
$$
\implies u- \frac{u^{3}}{3}+C=\sin x- \frac{\sin x}{3}+C
$$
# Estrategia para la evaluación de $\int \sin ^{m}(x)·\cos ^{n}(x) \, dx$
## Si $n$ es impar

Si la potencia de coseno es impar es decir $n=2k+1\mathbf{k}\in \mathbb{Z}^{+}_{0}$, se extrae el coseno y se usa [[Conocimientos/Matemática/Pure Mathematics/Structures (algebra)/Algebra/Trigonometría/Identidades trigonométricas#^25ecb8\|identidades pitagóricas]].

(lo mismo de si $m$ es impar)

## Si $m$ es impar

Si la potencia de seno es impar es decir $m=2k+1\mathbf{k}\in \mathbb{Z}^{+}_{0}$, se extrae el seno y se usa [[Conocimientos/Matemática/Pure Mathematics/Structures (algebra)/Algebra/Trigonometría/Identidades trigonométricas#^25ecb8\|identidades pitagóricas]].

$$
\int \sin ^{2k+1}(x)\cos ^{n}(x) \, dx =\int \sin ^{2k}\sin(x)\cos ^{n}(x) \, dx 
$$
$$
\int (1-\cos ^{2}x)^{k}\sin(x)\cos ^{n}(x) \, dx 
$$
## Si $m$ y $n$ son impares

Se aplican las siguientes [[identidades de ángulo medio\|identidades de ángulo medio]]:

$$
\boxed{\sin ^{2}(x)=\frac{1}{2}(1-\cos(2x))} 
$$
$$
\boxed{\cos ^{2}(x)=\frac{1}{2}(1+\cos(2x))} 
$$

Ahora se tiene:

$$
\sin(x)\cos(x)=\frac{1}{2}\sin(2x)
$$
# Estrategia para la evaluación de $\int \tan ^{m}(x)·\sec ^{n}(x) \, dx$

Nuevamente se aplican las identidades trigonométricas pitagóricas.

## Para $n$ par

Se extra un factor $\sec ^{2}x$ y $\sec ^{2}x=1+\tan ^{2}x$ 

Ahora se sustituye $u=\tan x$

### Ejemplo:

Para

$$
\int \tan ^{6}(x)\sec ^{4}(x) \, dx 
$$

Se extrae un factor de $\sec^2(x)$:

$$
\int \tan ^{6}(x)\sec ^{4}(x) \, dx = \int \tan ^{6}(x)\sec ^{2}(x)(1+\tan^2(x)) \, dx
$$

Luego se realiza la sustitución $u=\tan x$:

$$
\int u^6(1+u^2) \, du
$$

Resolviendo:

$$
\int u^6(1+u^2) \, du = \int (u^6 + u^8) \, du = \frac{u^7}{7} + \frac{u^9}{9} + C
$$

Finalmente, se reemplaza $u$ por $\tan x$:

$$
\frac{\tan^7(x)}{7} + \frac{\tan^9(x)}{9} + C
$$

## Para $m$ impar

Se extrae un factor de $\tan (x)\sec (x)$ y se utiliza que $\tan ^{2}(x)=\sec ^{2}(x)-1$ y se sustituye.

Es decir, para:

$$
\int  \tan ^{2k+1}(x)\sec ^{n}(x) \, dx = \int (\tan ^{2}(x))^{k}\sec ^{n-1}(x)\tan(x)\sec(x) \, dx 
$$
$$
\int (\sec ^{2}(x))^{k}\sec ^{n-1}\tan(x)\sec(x) \, dx 
$$
- [x] Revisar corolarios de ppt  [scheduled:: 2024-06-17]  [completion:: 2024-07-27]

> [!failure]- Failure 
>   Error: This is a chat model and not supported in the v1/completions endpoint.   Did you mean to use v1/chat/completions?