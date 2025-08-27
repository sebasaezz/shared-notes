---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/4-dinamica-de-cuerpos-rigidos-en-el-plano/4-7-principio-de-impulso-momentum-para-cuerpos-rigidos/momento-o-momentum-angular/","tags":["I2FIS1514"]}
---

Considerar a una partícula en posición $\vec{r}$ y [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.7 Impulso y momentum lineal/Momento o momentum e impulso lineal\|momento lineal]] $\vec{p}$.
Se va a definir al momento angular $\vec{L}$ naciendo del [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.2 Producto vectorial. Ecuaciones vectoriales de rectas y planos en el espacio/Producto cruz\|Producto cruz]] entre esta posición y la sumatoria de fuerzas. Todo para llegar a una propiedad de conservación de este momentum.
$$
\sum_{}^{}\vec{F}=\frac{d\vec{p}}{dt}
$$
$$
\vec{r}\times\sum_{}^{}\vec{F}=\vec{r}\times \frac{d\vec{p}}{dt}
$$
De aquí se va a tener que:
- [x] revisar despeje  [due:: 2024-12-05T15:44:00]  [completion:: 2025-04-20]
$$
\sum_{}^{}\tau=\frac{d(\vec{r}+\vec{p})}{dt}=\frac{d\vec{L}}{dt}\tag{1}
$$
De aquí, integrando, lo más importante será que:
$$
\boxed{L=I\omega} 
$$
Se puede llegar a un principio similar al principio de impulso-momentum integrando la ecuación 1:
$$
\vec{L}_{f}-\vec{L}_{i}=\int_{t_{i}}^{t_{f}} \tau_{\text{ext}} \, dt 
$$
De aquí también resulta muy útil derivar denuevo y llegar a que:
$$
\sum_{}^{}\tau_{\text{ext}}=I\alpha
$$
- [x] tarea de prueba  [due:: 2024-12-01T13:00:00]  [completion:: 2025-04-20]