---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/3-integrales-multiples/3-5-cambio-de-variables-a-coordenadas-polares-en-integrales-dobles/cambio-a-coordenadas-polares-en-una-integral-doble/","tags":["I2MAT1620"]}
---

# Concepto
Tomar una integral doble y representarla con coordenadas polares.
# Definición
Donde $0\leq a\leq r\leq b$ y $\alpha\leq\theta\leq\beta$ es lo mismo que decir $\mathcal{R}$
$$
\underset{ \mathcal{R} }{ \iint }f(x,y)dA=\int_{\alpha}^{\beta} \int_{a}^{b} r(f(r\cos \theta,r\sin \theta)) \, dr  \, d\theta 
$$
# Ejemplo
## Ejemplo 1
Evalúes $\iint_{\mathcal{R}}(3x+4y^{2})dA$ donde $\mathcal{R}$ es la región en el semiplano superior acotado por las circunferencias $x^{2}+y^{2}=1 \land x^{2}+y^{2}=4$
Se acota $r$ y $\theta$
$$
1\leq r\leq 2
$$
$$
0\leq\theta\leq 2
$$
$$
\int_{0}^{2\pi} \int_{1}^{2} r(3(r\cos\theta)+4(r\sin\theta)^{2}) \, dr  \, d\theta =15\pi
$$
## Ejemplo 2