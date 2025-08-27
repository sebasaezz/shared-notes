---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/calculo-i/3-aplicaciones-de-la-derivada/regla-de-l-hopital-y-formas-indeterminadas/","tags":["I3MAT1610"]}
---

# Regla de L'Hopital

Dado un límite donde queda como $\frac{0}{0}$ o $\frac{\pm \infty}{\pm \infty}$ (forma indeterminada), entonces el límite será igual al límite de la derivada del numerador partido en el límite del denominador

## Definición

> [!theorem] Regla de L'Hopital
> Dada $f$ y $g$ tales que alguna de las dos condiciones se cumple:
> - $\lim_{ x \to a } f(x)=0=\lim_{ x \to a } g(x)=0$
> - $\lim_{ x \to a } f(x)=0=\lim_{ x \to a } g(x)=\pm \infty$
> 
> Nota: $a\in\mathbb{R} \lor a=\pm \infty$
> Entonces:
> $$
> \lim_{ x \to a } \frac{f(x)}{g(x)}=\lim_{ x \to a } \frac{f'(x)}{g'(x)}
> $$

## Ejemplo
$$
\lim_{ x \to \frac{\pi}{2} } \frac{\cos x}{1-\sin x}=\lim_{ x \to \frac{\pi}{2} } \frac{-\sin x}{-\cos x}=\lim_{ x \to \frac{\pi}{2} } \tan x
\begin{cases}
\lim_{ x \to \frac{\pi}{2}^{+} } \tan x=-\infty \\
\lim_{ x \to \frac{\pi}{2}^{-} } \tan x=+\infty
\end{cases}
$$
# Formas indeterminadas

Se definen los siguientes casos:

- $\frac{0}{0}$, L'Hopital directamente
- $\frac{\infty}{\infty}$, L'Hopital directamente
- $0·\infty$, se traduce a $\frac{1}{\frac{1}{0}}·\infty=\frac{\infty}{\infty}$
	- E.g.: $\lim_{ x \to 0 } x·\ln x[0·(-\infty)]=\lim_{ x \to 0 } \frac{\ln x}{\frac{1}{x}}[-\frac{\infty}{\infty}]$, ahora aplicar L'Hopital
- $\infty-\infty$, restar y reducir
	- $\lim_{ x \to 1 } \left( \frac{x}{x-1}-\frac{1}{\ln x} \right)[\infty-\infty]=\lim_{ x \to 1 } \left( \frac{x\ln x-x+1}{(x-1)\ln x} \right)\left[ \frac{0}{0} \right]$, ahora aplicar L'Hopital
- $0^{0}$, sacar logaritmo
	- $L=\lim_{ x \to 0^{+} } x^{\sin x}$
	- $\ln L=\ln(\lim_{ x \to o^{+} } x^{\sin x})=\lim_{ x \to 0^{+} } \ln(x^{\sin x})=\lim_{ x \to 0^{+} } \sin x\ln x [0·(-\infty)]$, ahora aplicar tercer punto
	- Finalmente $L=e^{\lim_{ x \to 0^{+} } \sin x\ln x }$
- [x] Hacer ejercicios de estas cosas raras  [completion:: 2025-04-20]