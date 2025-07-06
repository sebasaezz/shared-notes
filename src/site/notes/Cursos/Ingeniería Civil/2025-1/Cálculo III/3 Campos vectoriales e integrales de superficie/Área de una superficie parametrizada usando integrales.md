---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/area-de-una-superficie-parametrizada-usando-integrales/","tags":["I3MAT1630"]}
---

# Concepto
Se quiere calcular el área de una superficie $S$. Sea el dominio de una parametrización $\vec{r}(s,t)$, $\mathcal{D}$ este dominio se subdivide en rectángulos $dA=ds\,dt$. Cada uno de estos corresponde a una parte de la superficie. Esta relación se puede aproximar linealmente.
Sean las subdivisiones $D_{ij}$, entonces se quiere obtener:
$$
\sum_{i,j}^{}\operatorname{area}(\vec{r}(D_{ij}))
$$
La aproximación es tomar el cuadrado en un punto $(s_{ij}, t_{ij})$ a el area en el punto $\vec{r}(s_{ij}, t_{ij})$ que es un paralelogramo tratando de aproximar un área abstracta.
El cuadrado tenía una esquina $(s_{ij}, t_{ij}+\Delta t)$ entonces esta esquina en el paralelogramo será $\vec{r}(s_{ij}, t_{ij}+\Delta t)$. La aproximación lineal será:
$$
\vec{r}(s_{ij}, t_{ij}+\Delta t)-\vec{r}(s_{ij}, t_{ij})\approx r_{t}(s_{ij}, t_{ij})\Delta t
$$
con $r_{t}$ la derivada parcial con respecto a $t$. Lo mismo con $s$:
$$
\vec{r}(s_{ij}+\Delta s, t_{ij})-\vec{r}(s_{ij}, t_{ij})\approx r_{t}(s_{ij}, t_{ij})\Delta s
$$
Ahora la aproximación del área será:
$$
\begin{align}
\operatorname{area}(\vec{r}(D_{ij})) & \approx\lvert\lvert (\vec{r}_{t}\Delta t )\times \vec{r}_{s}\Delta s \rvert\rvert \\
 & \approx\lvert\lvert \vec{r}_{s}\times \vec{r}_{s} \rvert\rvert(s_{ij}, t_{ij}) \Delta s\Delta t 
\end{align}
$$
Ahora sumando los cuadraditos:
$$
\operatorname{area}(S)\approx \sum_{i,j}^{}\lvert \lvert \vec{r}_{t}\times \vec{r}_{s} \rvert \rvert (s_{ij},t_{ij})\Delta s\Delta t 
$$
Llevando el límite, se tiene una integral doble:
$$
\iint_{\mathcal{D}} \lvert \lvert \vec{r}_{t}\times \vec{r}_{s} \rvert \rvert   \, dA 
$$

Si se hace el despeje de una superficie de revolucion por $f(x)$, entonces se va a llegar que el área es: $\mapsto$
$$
2\pi \int_{a}^{b} f(x)\sqrt{ 1+f'(x)^{2} } \, dx 
$$

# Definición
# Ejemplo
Calcule el área de de una esfera de radio $\rho$.
Su parametrización es:
$$
\vec{r}(\theta,\phi)=\langle  \rho \sin \phi \cos\theta,\rho \sin \phi \sin\theta,\rho \cos \phi\rangle 
$$
Calculando las derivadas:
$$
r_{_{\phi}}=\langle \rho \cos \theta \cos \phi, \rho \sin\theta \cos \phi, -\rho \sin \phi \rangle 
$$
$$
r_{\theta}=\langle -\rho \sin \phi \sin\theta, \rho \sin \phi \cos\theta, 0 \rangle 
$$
Ahora se puede desarrollar el producto cruz entre estos dos vectores, llegando a: $\rho^{2}\sin \phi$. 
Entonces el área será:
$$
\begin{align}
\operatorname{area}(S) & =\iint _{D} \rho^{2}\sin \phi\,dA \\
 &= \int_{0}^{\pi} \int_{0}^{2\pi} \rho^{2}\sin \phi \, d\theta  \, d\phi  \\
 & =2\pi \rho^{2}
\end{align}
$$
