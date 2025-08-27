---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/quimica-para-ingenieria/6-equilibrio-quimico/constante-de-equilibrio-kc-y-kp/","tags":["I2QIM100E"]}
---


Dada por la proporción de concentraciones en un momento dado. $K_{c}$ no tiene unidades.

Dada una temperatura constante, $K_{c}$ no debe cambiar.

Para una reacción dada por:

$$
aA+bB \rightleftarrows cC+dD
$$

K es una relación de constantes de velocidad ($\frac{k_{1}}{k_{-1}}$)

# En una reacción en medio acuoso
$$
K_{c}=\frac{[C]^{c}[D]^{d}}{[A]^{a}[B]^{b}}
$$
# En una reacción en medio gaseoso
$$
K_{p}=\frac{P_{C}^{c}P_{D}^{d}}{P_{A}^{a}P_{B}^{b}}
$$
# Relación entre $K_{c}$ y $K_{p}$
## En medio gaseoso

Dada la reacción:

$$
aA_{(g)} \to bB_{(g)}
$$

Y la ecuación de los gases ideales:

$$
PV=nRT
$$

Entonces: $P=\frac{nRT}{V}$

Así:

$$
K_{p}=\frac{(\frac{n_{B}RT}{V})^{b}}{(\frac{n_{A}RT}{V})^{a} }
$$

Pero $\frac{n}{V}$ es concentración, entonces:

$$
K_{p}=\frac{[B]^{b}}{[A]^{a}}(RT)^{b-a}=K_{c}(RT)^{b-a} \implies  \boxed{K_{p}=K_{c}(RT)^{\Delta n}} 
$$

Entonces, si $\Delta n=0$, se tiene una equivalencia:

$$
K_{p}=K_{c}(RT)^{0}=K_{c}
$$

# Interpretación de la constante
- Si $K\gg 1$ entonces el equilibrio estará desplazado hacia los productos.
- Si $K\ll 1$ entonces el equilibrio estará desplazado hacia los reactantes.
# Cálculo de $K_{c}$

La sustancias puras $(l)$ o $(s)$, no se consideran en el cálculo, ya que permanecen constantes.

Ejemplo:

$$
HF_{(ac)}+H_{2}O_{(l)} \rightleftarrows H_{3}O^{+}_{(ac)} + F^{-}_{(ac)}
$$

Entonces $K_{c}=\frac{[H_{3}O^{+}][F^{-}]}{[HF]}$

No se considera a $H_{2}O$ por que es líquido.

# Cuociente de reacción $Q_{c}$

Se aplica la misma fórmula de $K_{c}$, solo que fuera del punto de equilibrio.