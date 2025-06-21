---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/4-balance-en-maquinas/entropia-en-gases-ideales/","tags":["I2IIQ1003"]}
---

# Camino de presión constante
Se usa simplemente:
$$
\Delta S_{12}=\int_{T_{1}}^{T_{2}} \frac{C_{p}^{ig}}{T} \, dT 
$$
Que considerando un $C_{p}$ promedio:
$$
\Delta S_{12}=\bar{C}_{p}^{ig}\ln\left( \frac{T_{2}}{T_{1}} \right)
$$
# Camino isotérmico reversible
Se aplica la primera ley:
$$
dU^{ig}=dQ_{rev}-PdV^{ig}
$$
Een el [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Modelo de gases ideales\|Modelo de gases ideales]], si $T=cte$, entonces $\Delta U=0$.
$$
PdV^{ig}=dQ_{rev}
$$
Además, por ley de gases ideales:
$$
V^{ig}=\frac{RT}{P}
$$
Entonces:
$$
dV^{ig}=d\left( \frac{RT}{P} \right)=-\frac{RT}{P^{2}}dP
$$
Reemplazando:
$$
\begin{align}
dQ_{rev} & =-P· \frac{RT}{P^{2}}dP \\
 & =-RT\frac{dP}{P} \\
\implies \frac{dQ_{rev}}{T} & =-R \frac{dP}{P}
\end{align}
$$
Integrando:
$$
\begin{align}
\Delta S_{12}=\int_{1}^{2}  \, \frac{dQ_{rev}}{T} & =-R\int_{P_{1}}^{P_{2}}  \, \frac{dP}{P} \\
 & =-R\ln\left( \frac{P_{2}}{P_{1}} \right)  
\end{align}
$$
# Camino general
Para un camino general, se puede considerar un proceso isobárico y uno isotérmico (dos lineas rectas en un diagrama P-T). De aquí se llega a la forma general para gases ideales:
$$
\begin{align}
\Delta S_{12} & =\int_{T_{1}}^{T_{2}} C_{p}^{ig} \, \frac{dT}{T}-R\ln \left( \frac{P_{2}}{P_{1}} \right) \\
 & =\bar{C}_{p}^{ig}\ln\left( \frac{T_{2}}{T_{1}} \right)-R\ln\left( \frac{P_{2}}{P_{1}} \right)
\end{align}

$$
![Pasted image 20250425080620.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/4%20Balance%20en%20m%C3%A1quinas/attachments/Pasted%20image%2020250425080620.png)
# Proceso adiabático reversible
Que un proceso sea reversible implica que $\Delta S=0$
Si se reemplaza 0 en la ecuación anterior, se llega a la misma ecuación en [[Cursos/Ingeniería Civil/2025-1/Termodinámica/2 Gases ideales/Procesos adiabáticos reversibles en gases ideales\|Procesos adiabáticos reversibles en gases ideales]]:
$$
\frac{P_{2}}{P_{1}}=\left( \frac{T_{2}}{T_{1}} \right)^{C_{p}^{ig}/R}
$$