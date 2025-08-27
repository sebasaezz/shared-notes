---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/2-dinamica-de-particulas/2-4-trabajo-y-energia-cinetica/energia-cinetica-y-principio-de-trabajo-y-energia/","tags":["ExFIS1514"]}
---

$$
\boxed{U_{c}=U_{k}=E_{c}=E_{k}=K= \frac{1}{2}mv^{2}} 
$$

> [!quote]
> La energía cinética es **siempre, siempre siempre** **siempre** mayor a cero.
> _(Alejandro Varas, 2024)_

# Principio de trabajo y energía
$$
W=K-K_{0}=\frac{1}{2}mv^{2}
$$
Esto solo sucede para fuerzas conservativas.

> [!theorem] principio de conservación de la energía
> $$
> \begin{align}
> W=K_{f}-K_{i} & \implies K_{i}+W=K_{f} \\
>  & \implies K_{i} + \underbrace{ [W_{c}+W_{nc}] }_{ \text{conser. + no c.} }=K_{f} \\
>  & \implies \boxed{K_{i}+[(U_{i}-U_{f})+W_{nc}]=K_{f}} 
> \end{align}
> $$
> De aquí, se pueden agrupar términos y ocupar la [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.5 Energía potencial/Energía mecánica\|Energía mecánica]].
> $$
> \begin{align}
> [U_{i}-U_{f}]+W_{nc} & =K_{f}-K_{i} \\
> \underbrace{ K_{i}+U_{i} }_{ E_{i} }+W_{nc} & =\underbrace{ K_{f}+U_{f} }_{ E_{f} } \\
> \end{align}
> $$
> 
> $$
> \boxed{E_{i}+W_{nc}=E_{f}} 
> $$
> Notar que para que esta ecuación tenga sentido, $E_{f}\leq E_{i}$, el trabajo realizado por las fuerzas no conservativas ($W_{nc}$) debe ser negativo. Esto siempre sucede.
# Ejemplo
Un objeto de masa $m=2 \pu{ kg}$ se desplaza con $\vec{v}=10 \frac{\pu{ m }}{s}\hat{x}$. Cuál es su energía cinética.
$$
K=\frac{1}{2}(2\pu{ kg})\left( 10 \frac{\pu{ m}}{\pu{ s}^{2}} \right)=100 \pu{ J }
$$