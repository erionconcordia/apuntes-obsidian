---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/04-medidas-de-posicion/01-medidas-de-posicion/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

**Tags:** #estadística_descriptiva #medidas_posicion #cuartiles #porcentiles #IQR

Mientras que las medidas de centralización buscan el "medio" y las de dispersión buscan qué tan "esparcidos" están los datos, las **medidas de posición** (o cuantiles) tienen un objetivo distinto: dividen un conjunto de datos ordenados en partes iguales para indicar la ubicación relativa de un valor específico dentro de la muestra o población.

---
## 1. Percentiles
Los percentiles son medidas que dividen el conjunto de datos ordenados (de menor a mayor) en 100 partes iguales.
- **Interpretación:** El percentil $k$ (denotado también como $P_k$) es un valor tal que el $k$% de las observaciones en la muestra son menores o iguales a él, y el $(100-k)$% restante de las observaciones son mayores.
- **Ejemplo:** Si el puntaje de resistencia de una viga se encuentra en el percentil 95 $(P_{95})$, esto significa que esta viga resiste más que el 95% de todas las vigas analizadas, y sólo el 5% superior la supera.

---
## 2. Cuartiles ($Q1,Q2,Q3$)
Para obtener un resumen más rápido de la distribución de los datos, no solemos usar los 99 percentiles, sino que dividimos la muestra en **cuatro partes iguales** (del 25% cada una) utilizando tres cortes llamados **cuartiles**.

**Primer Cuartil $(Q1)$**
Equivale al percentil 25 $(P_{25})$. Separa el 25% más bajo a los datos del 75% superior.

**Segundo Cuartil $(Q2)$**
Equivale al percentil 50 $(P_{50})$. Este valor es exactamente la mediana $\tilde{x}$, ya que divide al muestra en dos mitades idénticas.

**Tercer Cuartil $(Q3)$**
Equivale al percentil 75 $(P_{75})$. Separa el 75% inferior de los datos del 25% más alto (el "cuarto superior").

>[!tip] Regla visual
>Los cuartiles dividen los datos algo así:
>![Pasted image 20260423111145.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260423111145.png)

---
## 3. Rango intercuartílico (IQR o $f_s$)
El rango intercuartílico (a veces denotado como *dispersión de los cuartos* $f_s$) es una de las medidas de variabilidad más importantes en la estadística moderna.

**Fórmula:** Se calcula restando el primer cuartil al tercer cuartil:
$$IQR=Q3-Q1$$
**Significado**
El $IQR$ representa la distancia geométrica o longitud que abarca exactamente el 50% central de los datos.

**Propiedad fundamental**
A diferencia del rango ($R=Máx-Min$) o de la varianza, el $IQR$ es una medida resistente a los valores atípicos (outliers). Como su cálculo ignora por completo las observaciones comprendidas en el 25% más pequeño y el 25% más grande de la muestra, un error de medición extremo en una máquina no alterará en absoluto el valor del $IQR$.

>[!dato] Conexión directa con el Boxplot
>El $IQR$ es el corazón de la [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/01_Estadística descriptiva/04_Medidas de posición/02-Gráfica de caja y bigotes (boxplot)\|02-Gráfica de caja y bigotes (boxplot)]]
>1. Es el valor que determina el "ancho" exacto de la caja central.
>2. Es el multiplicador matemático que se utiliza para calcular las fronteras de anomalías: los límites inferior ($Q1-1.5\cdot IQR$) y superior ($Q3+1.5\cdot IQR$) más allá de los cuales un dato se considera un valor atípico o "raro".



