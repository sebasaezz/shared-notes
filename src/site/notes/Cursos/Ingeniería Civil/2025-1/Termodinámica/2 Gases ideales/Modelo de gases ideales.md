---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/2-gases-ideales/modelo-de-gases-ideales/","tags":["I2IIQ1003"]}
---

Un gas ideal asume que la distancia entre átomos es infinita. No hay interacciones moleculares. Este modelo es ideal para cuando las presiones son bajas ($\leq 1\, \pu{ atm}$) o temperaturas altas (2 o 3 veces la de saturación) y se tienen gases poco complejos y con baja polaridad como $H_{2}$ o $O_{2}$. Si no se deben considerar modelos con [[Cursos/Ingeniería Civil/2025-1/Termodinámica/5 Gases reales/Factor de compresibilidad (Z)\|Factor de compresibilidad (Z)]].
En gases ideales, si se tiene un proceso isotérmico, $\Delta U=0$. Eso significa que:
$$
Q=-W
$$
Si la temperatura se mantiene constante, entonces $U$ se mantiene constante. Es decir, $U$ solo es función de la temperatura.
$$
U^{ig}=U^{ig}(T)
$$
Para un gas ideal, se cumple lo siguiente:
$$
PV_{m}=RT
$$
Nota: $V_{m}$ es volumen molar.
Entonces:
$$
\begin{align}
H^{ig} & =U^{ig}+PV^{ig}\tag{1} \\
 & =U^{ig}+RT
\end{align}
$$
Entonces, la entalpía de un gas ideal solo depende de la temperatura:
$$
H^{ig}=H^{ig}(T)
$$
Diferenciando la ecuación 1 con presión y volumen contante con respecto a $T$:
$$
\boxed{C_{P}-C_{V}=R} 
$$
[[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/5 Calorimetría/Calorimetría, capacidad calorífica y calor latente\|Recordando que]]:
- $\left( \frac{ \partial H }{ \partial T } \right)_{P}=C_{P}$
- $\left( \frac{ \partial U }{ \partial T } \right)_{V}=C_{V}$
[[Cursos/Ingeniería Civil/2024-1/Química para Ingeniería/4 Termoquímica. Energía y Quimíca/El trabajo (w) en termodinámica (gases)\|Se sabe que]]:
$$
W=-\int_{V_{1}}^{V_{2}} P \, dV
$$
Y que $P=\frac{RT}{V_{m}}$, entonces:
$$
\begin{align}
W_{m} & =-RT\int_{V_{1}}^{V_{2}} \frac{1}{V_{m}} \, dV  \\
W_{m} & =-RT\ln \frac{V_{2}}{V_{1}}
\end{align}
$$

En resumen: 
- **Si no cambia la temperatura**: $\Delta H^{ig}=0$ y $\Delta U^{ig}=0$ y el trabajo se calcula con la ecuación de arriba.
- **Si cambia la temperatura:** Se aplican las integrales de $C_{P}$ y $C_{V}$ para obtener $\Delta H^{ig}$ y $\Delta U^{ig}$. 

# Resumen con distintos procesos
## Proceso isotérmico
De un estado 1 a 2:
$$
\Delta U_{12}^{ig}=0
$$
$$
\Delta H_{12}^{ig}=0
$$
$$
Q_{m}=-W_{m}=RT\ln \frac{V_{2}}{V_{1}}
$$
$V_{1}$ y $V_{2}$ no tienen que ser molares ya que están en una fracción.
Notar que:
$$
\begin{align}
P_{i}V_{i} & =RT \\
V_{i} & =\frac{RT}{P_{i}}
\end{align}
$$
entonces:
$$
\frac{V_{2}}{V_{1}}=\frac{RTP_{1}}{RTP_{2}}=\frac{P_{1}}{P_{2}}
$$
$$
Q_{m}=-W_{m}=RT\ln \frac{P_{1}}{P_{2}}
$$

## Isocórico
$$
\Delta U=W+Q
$$
Cuando $V=cte$, $W=0$. y $\Delta U_{12}=Q$.
$\Delta U_{12}$ es la integral de $C_{V}$.
# Ejemplo
Vapor lleva a cabo un proceso de compresión isotérmica reversible a 350ºC, desde 20 bar hasta 40 bar. Asumiendo el que vapor estará como gas ideal. Calcular el calor, trabajo, los cambios en energía interna y entalpía. La capacidad calorífica de gas ideal del vapor está dada por:
$${\frac{C_{P}^{i g}}{R}}=4{,}3954186·10^{-3}T+{0,}00001405·T^{2}-{1,}564·10^{-8}T^{3}+{6,}32·10^{12}T^{4}+{8,}37136·10^{-12}T^{5}$$
Se tiene un caso isotérmico. Entonces $\Delta U=\Delta H=0$. Además:
$$
Q_{m}=-W_{m}=RT·\ln\left( \frac{V_{2}}{V_{1}} \right)=RT·\ln\left( \frac{P_{1}}{P_{2}} \right)
$$
$$
\begin{align}
Q_{m} & =RT·\ln\left( \frac{P_{1}}{P_{2}} \right) \\
 & =8{,}314 \frac{\, \pu{ J}}{\, \pu{ mol·K}}·(350+273{,}15)\, \pu{ K}·\ln\left( \frac{20\, \pu{ bar}}{40\, \pu{ bar}} \right) \\
 & =-3591{,}3 \, \pu{ \frac{J}{mol}}
\end{align}
$$
$$
q=-3591{,}3\, \pu{ \frac{\cancel{ J }}{\cancel{ mol }}}· \frac{1}{18} \, \pu{ \frac{\cancel{ mol }}{\cancel{ g }}}· \frac{1000\, \cancel{ \pu{ g} }}{\, \pu{ kg}}· \frac{1000\, \pu{kJ}}{1\, \pu{ \cancel{ J }}}=-199{,}5 \, \pu{ \frac{kJ}{kg}}=-w
$$
