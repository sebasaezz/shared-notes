---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/2-gases-ideales/procesos-adiabaticos-reversibles-en-gases-ideales/","tags":["I2IIQ1003"]}
---

Un proceso adiabático tiene la restricción de que $dQ=0$. Esto se logra por métodos de aislación.
Aplicando la [[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/4 Primera ley de la termodinámica/Primera ley de la termodinámica\|Primera ley de la termodinámica]]:
$$
\Delta U=\int_{T_{1}}^{T_{2}} C_{V}^{ig} \, dT =W
$$
Esto se puede escribir de forma diferencial:
$$
dU=C^{ig}_{V}dT=dW
$$
En los problemas usualmente se conoce dos funciones de estado iniciales y una final. Para obtener la segunda final se debe seguir un camino restringido por $dQ=0$. Es decir, de la restricción se pueden sacar ecuaciones.
Como:
$$
dW=-PdV
$$
$$
C^{ig}_{V}dT=-PdV^{ig}
$$
Como $PV_{m}=RT$:
$$
C^{ig}_{V}dT=-\frac{RT}{V_{m}^{ig}} dV^{ig}
$$
$$
\frac{1}{R} \frac{C^{ig}_{V}}{T}dT=-\frac{dV^{ig}}{V_{m}}
$$
Integrando:
$$
-\ln\left( \frac{V_{2}}{V_{1}} \right)=\frac{1}{R}\int_{T_{1}}^{T_{2}} \frac{C^{ig}_{V}}{T} \, dT 
$$
Si se aproxima a las capacidad caloríficas con su [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Media log-x\|Media log-x]]:
$$
\bar{C}^{ig}_{V,\log}=\frac{\int_{T_{1}}^{T_{2}} C_{V}^{ig} \, \frac{dT}{T} }{\ln(T_{2}/T_{1})}
$$
Entonces:
$$
\ln\left( \frac{V_{1}}{V_{2}} \right)=\frac{1}{R} \bar{C}_{V,\log}^{ig}\ln\left( \frac{T_{2}}{T_{1}} \right)
$$

$$
\boxed{\frac{V_{2}}{V_{1}}=\left( \frac{T_{2}}{T_{1}} \right)^{-\bar{C}^{ig}_{V,\log}/R}} 
$$
Ahora, como $\frac{V_{2}}{V_{1}}=\frac{P_{1}}{P_{2}}· \frac{T_{2}}{T_{1}}$:
$$
\frac{P_{1}}{P_{2}} · \frac{T_{2}}{T_{1}}=\left( \frac{T_{2}}{T_{1}} \right)^{-\bar{C}_{V,\log}^{ig}/R}
$$
$$
\frac{P_{2}}{P_{1}}=\left( \frac{T_{2}}{T_{1}} \right)^{1+ \bar{C}_{V,\log}^{ig}/R}
$$
De las propiedades del [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Modelo de gases ideales\|Modelo de gases ideales]], se sabe que:
$$
C_{P}-C_{V}=R
$$
$$
\frac{C_{P}-C_{V}}{R}=1
$$
$$
\frac{C_{P}}{R}=1+ \frac{C_{V}}{R}
$$
Entonces:
$$
\boxed{\frac{P_{2}}{P_{1}}=\left( \frac{T_{2}}{T_{1}} \right)^{C_{P}/R}} 
$$
Pero como $T=\frac{PV}{R}\implies$ $\frac{T_{2}}{T_{1}}=\frac{P_{2}}{P_{1}}· \frac{V_{2}}{V_{1}}$

$$
\begin{align}
\frac{P_{2}}{P_{1}} & =\left( \frac{P_{2}}{P_{1}}· \frac{V_{2}}{V_{1}} \right)^{C_{P}/R} \\
\left( \frac{P_{2}}{P_{1}} \right)^{1- C_{P}/R} & =\left( \frac{V_{2}}{V_{1}}  \right)^{C_{P}/R} \\
\left( \frac{P_{2}}{P_{1}} \right)^{-C_{V}/R} & =\left( \frac{V_{2}}{V_{1}}  \right)^{C_{P}/R} \\
\frac{P_{2}}{P_{1}} & =\left( \frac{V_{2}}{V_{1}} \right)^{-C_{P,\log}^{ig}/C_{V,\log}^{ig}}
\end{align}
$$
Usualmente a la razón entre capacidades caloríficas medias logarítmicas se le denomina [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Índice adiabático\|Índice adiabático]] $\bar{\gamma}$, o simplemente $\gamma$ si los valores son constantes, y la expresión se muestra de la forma:
$$
\boxed{P_{1}(V_{1})^{\bar{\gamma}}=P_{2}(V_{2})^{\bar{\gamma}}} 
$$
