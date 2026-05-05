---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/04-medidas-de-posicion/02-grafica-de-caja-y-bigotes-boxplot/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #estadística_descriptiva #representaciones_gráficas #boxplot 

## 1. ¿Qué es y para qué sirve?
La gráfica de caja y bigotes (o boxplot) es un resumen visual diseñado para reflejar las propiedades más prominentes de una muestra o conjunto de datos basándose en medidas que son resistentes a los valores atípicos (es decir, que no se ven drásticamente afectadas por datos extremos).

Sirve principalmente para evaluar cuatro aspectos fundamentales de un vistazo:
1. El **centro** de los datos.
2. La **dispersión** o variabilidad.
3. La **asimetría** (hacia dónde se alargan los datos).
4. La identificación rápida de valores **atípicos** (anomalías u observaciones extremas).
---
![Pasted image 20260422110248.png\|510](/img/user/IM%C3%81GENES/Pasted%20image%2020260422110248.png)
## 2. Anatomía del boxplot
El boxplot se construye a partir del "**resumen de cinco números**": el valor mínimo, el primer cuartil ($Q1$ o cuartil inferior), la mediana, el tercer cuartil ($Q3$ o cuartil superior) y el valor máximo.

Visualmente, se compone de las siguientes partes:

**1. La caja central:** Es un rectángulo que va desde el primer cuartil ($Q1$) hasta el tercer cuartil ($Q3$). Esta caja encierra el 50% central de los datos. La longitud o anchura de esta caja se llama **Rango intercuartílico** ($IQR$) o dispersión de los cuartos ($f_s$), calculado como $IQR=Q3-Q1$. Es una medida de dispersión muy confiable.

**2. La mediana ($Q2$):** Es un segmento de línea vertical (u horizontal, si el gráfico está rotado) que divide la caja. Esto indica el centro exacto de la distribución de los datos. La posición de esta línea dentro de la caja te dice mucho sobre la asimetría en la mitad central de tus datos.

**3. Los bigotes:** Son líneas que se extienden hacia afuera desde ambos extremos de la caja. Estos bigotes no siempre van hasta el valor máximo y mínimo absoluto. Se extienden hasta la observación más pequeña y la más grande que no sean considerados valores atípicos.

**4. Valores atípicos (outliers):** Se representan como puntos, asteriscos o círculos individuales más allá de las puntas de los bigotes (límites inferior y superior).
- **La regla del 1.5:** Técnicamente, cualquier observación que se aleje de la caja por una distancia superior a $1.5\cdot IQR$ (hacia arriba de $Q3$ o hacia abajo de $Q1$) se considera una anomalía o valor extremo. A esta distancia mínima se la conoce como límite inferior ($Q1-1.5\cdot IQR$) y límite superior ($Q3+1.5\cdot IQR$); la función de este límite es definir a partir de dónde empieza la "zona de anomalías".
---
## 3. ¿Cómo leer e interpretar un boxplot?
Cuando vemos un boxplot en nuestros problemas, debemos hacernos las siguientes preguntas:
1. ¿Dónde está el centro?
2. ¿Qué tan dispersos están los datos?
3. ¿Hay asimetría?
4. ¿Hay datos raros?

Respondiendo cada una de las preguntas:
1. Miramos la línea de la mediana. Eso te da el valor típico representativo.
2. Observamos el tamaño de la caja ($IQR$) y la distancia total entre las puntas de los bigotes (el rango de todos los típicos). Una caja muy ancha indica mucha variabilidad en la muestra.
3. Si la línea de la mediana está exactamente en el centro de la caja y los bigotes miden lo mismo, la distribución es simétrica. Si la aja es más grande del lado derecho de la mediana (o el bigote derecho es mucho más largo), hay asimetría positiva (la "cola" de los datos se alarga hacia valores mayores), y si ocurre lo contrario, hay asimetría negativa.
4. Buscamos los asteriscos fuera de los bigotes. En control de calidad o manufactura, un valor extremo alerta al investigador de que el proceso puede tener problemas o que un procedimiento asume normalidad de forma errónea.