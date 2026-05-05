---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/01-conceptos/04-estad-descriptiva/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #estadística #análisis_de_datos #fórmulas

## Estadística Descriptiva
Es la rama encargada de organizar, resumir y describir las características más prominentes de un conjunto de datos (ya sea una muestra o una población). No saca conclusiones más allá de los datos analizados.

---
#### Herramientas visuales
**Histogramas**
Representación de la distribución de frecuencias de variables continuas o discretas.

**Gráficas de caja y bigotes (Boxplots)**
Muestran el centro, la dispersión (rango intercuartílico), la asimetría y los valores atípicos (outliers).

**Gráficos de puntos y diagramas de tallo y hojas**
Útiles para visualizar la concentración, dispersión y brechas en conjuntos de datos numéricos

---
#### Estrategia de gráficos
**Gráficos de puntos y diagramas de tallo y hojas:**
Usarlos cuando tenemos pocos datos ($n<30$) y queremos un vistazo rápido sin perder la información original. Si miramos un tallo y hojas, podemos reconstruir el conjunto de datos exacto número por número, **pero** si tenemos 10.000 datos, hacer puntitos es imposible y el gráfico se vuelve una mancha ilegible.

**Histogramas**
Usarlos cuando tenemos muchos datos (generalmente $n>30$) y queremos ver la "forma" general de la distribución. Este gráfico nos permite ver instantáneamente si los datos se agrupan en el centro (forma de campana), si están tirados hacia un lado (asimetría), o si hay dos picos (distribución bimodal). Como desventaja se pierden los datos individuales; si sabemos que hay 15 datos entre 100 y 110 $\ohm$, no logramos saber si son todos 101 o todos 109.

**Diagrama de caja y bigotes (boxplots)**
Usarlos cuando queremos comparar varios grupos de datos simultáneamente o cuando nuestra prioridad absoluta es encontrar valores atípicos (outliers). Como ventaja: es imbatible para comparar; imaginemos que queremos comparar el tiempo de vida útil de capacitores de tres marcas distintas (A, B y C), si ponemos tres histogramas juntos, es un lío visual, pero si ponemos tres bloxplots uno al lado del otro, vemos instantáneamente qué marca tiene la mediana más alta, cuál es más consistente (caja más angosta) y cuál tiene capacitores fallados que mueren rápido (los puntitos outliers fuera de los bigotes)