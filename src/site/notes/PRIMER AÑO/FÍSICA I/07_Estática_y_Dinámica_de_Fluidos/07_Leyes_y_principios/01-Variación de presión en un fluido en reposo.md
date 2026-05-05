---
{"dg-publish":true,"permalink":"/primer-ano/fisica-i/07-estatica-y-dinamica-de-fluidos/07-leyes-y-principios/01-variacion-de-presion-en-un-fluido-en-reposo/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Si tenemos en cuenta el siguiente diagrama, tomando como referencia de que el fluido está en reposo, es decir, la fuerza neta es cero, podemos deducir:
![Pasted image 20250714191154.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250714191154.png)
$$\sum\vec{F_Y}=0$$
$$\vec{F_1}-\vec{P}-\vec{F_2}=0 \ (1)$$
Para cada variable tenemos lo siguiente:
- $\vec{F_1}=P\cdot A$
- $\vec{F_2}=(P+dP)\cdot A$
- $\vec{P}=m\cdot\vec{g}=\rho \cdot\vec{g}\cdot A \cdot dy$
Entonces, concluimos reemplazando las expresiones en la ecuación $(1)$:
$$P\cdot A - (P+dP)\cdot A - \rho\cdot\vec{g}\cdot A\cdot dy=0$$
$$P - P-dP - \rho\cdot\vec{g}\cdot dy=0$$
$$-dP-\rho\cdot\vec{g}\cdot dy=0$$
$$\frac{dP}{dy}=-\rho\cdot\vec{g} \ \ (2)$$
Con la ecuación diferencial (2) podemos obtener otra serie de resultados, por ejemplo, podemos calcular la diferencia de presión entre dos puntos en el fluido, podemos calcular cómo varía la presión en el fluido, entre otros más.

#### Diferencia de presión entre dos puntos:
Partiendo de la expresión $(2)$: $\frac{dP}{dy}=-\rho\cdot\vec{g}$
$$dP=-\rho\cdot\vec{g}\cdot dy$$
$$\int_{P_1}^{P_2}dP=\int_{y_1}^{y_2}-\rho\cdot\vec{g}\cdot dy$$
$$\int_{P_1}^{P_2}dP=-\rho\cdot\vec{g}\cdot \int_{y_1}^{y_2}dy$$
$$P_2-P_1=-\rho\cdot\vec{g}\cdot(y_2-y_1)$$Y así conseguimos la diferencia de presión entre dos puntos de un fluido que se encuentran a diferente altura.

#### Variación de la presión como función de la profundidad

Utilizamos la ecuación anterior: $P_2-P_1=-\rho\cdot\vec{g}\cdot(y_2-y_1)$, entonces:
- $P_2=P_{atm}=P_o$
- $P_1=P$
![Pasted image 20250714194836.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250714194836.png)
Por lo tanto:
$$P_o-P=-\rho\cdot\vec{g}\cdot h$$
$$P=P_o+\rho\cdot\vec{g}\cdot h$$
Y esta última expresión podemos definirla como **presión en un fluido de densidad uniforme**.