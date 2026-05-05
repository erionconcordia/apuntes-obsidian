---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/03-descripcion-de-un-conjunto-de-datos/01-organizacion-tabular/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #estadística_descriptiva #tablas_de_frecuencias #datos_agrupados

El primer paso de la estadística descriptiva, una vez que se han recolectado los datos "crudos" o desorganizados, es **ordenarlos y tabularlos**. Esta clasificación y agrupación nos permite condensar la información para identificar rápidamente un valor típico, evaluar su grado de dispersión y buscar patrones que a simple vista son invisibles.

Dependiendo del tipo de variable y la cantidad de datos, la cátedra divide este proceso en dos grandes métodos: **Tablas de Frecuencias Simples** y **Datos Agrupados**.

---
## 1. Tablas de frecuencias simples
Se utilizan principalmente para datos **categóricos (cualitativos)** o para datos numéricos **discretos** que asumen una cantidad pequeña de valores distintos.

Revisar: [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/01_Estadística descriptiva/01_Conceptos/03-Variables y escalas de medición\|03-Variables y escalas de medición]]

En este tipo de tabla, se lista cada valor único de la variable y se cuentan sus ocurrencias. La estructura analítica que debemos dominar incluye las siguientes columnas:

**Variable ($x_i$):** Cada uno de los valores únicos o categorías posibles que tomó la variable en la muestra.

**Frecuencia absoluta ($f_i$):** Es el recuento exacto de cuántas observaciones del conjunto de datos cayeron en ese valor particular $x_i$. La sumatoria de todas las $f_i$ siempre debe ser igual al tamaño de la muestra $n$.

**Frecuencia relativa ($f_{ri}$):** Es la fracción o proporción de veces que ocurre el valor. Se calcula dividiendo la frecuencia absoluta entre el número total de observaciones: $f_{ri}=f_i/n$.

**Frecuencia absoluta acumulada ($F_i$):** Es la suma de la frecuencia absoluta del valor $x_i$ actual más todas las frecuencias absolutas de los valores anteriores.

**Frecuencia relativa acumulada ($F_{ri}$):** Es la proporción total de observaciones que son menores o iguales al valor actual.

Por ejemplo, se proporcionan los siguientes datos: 1, 1, 2, 3, 3, 1, 2, 1, 1, 2.

| $x_i$ | $f_i$ | $f_{ri}$ | $F_i$ | $F_{ri}$ |
| ----- | ----- | -------- | ----- | -------- |
| 1     | 5     | 0.5      | 5     | 0.5      |
| 2     | 3     | 0.3      | 8     | 0.8      |
| 3     | 2     | 0.2      | 10    | 1        |
|       | 10    | 1        |       |          |

---
## 2. Datos agrupados (Distribuciones de frecuencias por clases)
Cuando trabajamos con variables numéricas continuas (mediciones como voltaje, resistencia o temperatura) o con variables discretas que tienen un rango muy amplio de valores, crear una tabla simple generaría cientos de filas con frecuencia 1 o 2, lo cual no resume nada.

En estos casos, se debe subdividir el eje de medición en intervalos de clase o "clases" (representados como un rango, por ejemplo $[10,20)$) de modo que cada observación de la muestra caiga en exactamente una clase.

Conceptos clave para armar al tabla de datos agrupados:

**Número de clases:** No hay una regla inviolable, pero generalmente se utilizan entre 5 y 20 clases. Como "regla empírica" rápida en problemas grandes, se recomienda usar aproximadamente la raíz cuadrada del número total de observaciones:
$$\text{Número de clases}\approx\sqrt{n}$$
**Amplitud o ancho de clase:** Por lo general, los intervalos deben tener el mismo ancho. Sin embargo, si los datos están muy alargados (sesgados con valores muy extremos), se pueden usar anchos desiguales para evitar dejar muchas clases vacías en los extremos.

**Manejo de fronteras:** ¿Qué pasa si una medición es exactamente 20.0 y tus clases son $[10,20)$ y $[20,30)$? Para evitar que el dato caiga en dos intervalos, por convención, el intervalo incluye el límite inferior pero excluye el límite superior. Es decir, si cae en la frontera, se coloca en el intervalo a la derecha de la misma.

**Marca de clase o punto medio:** Al agrupar los datos dentro del intervalo, por ejemplo $[10,20)$, perdemos la información sobre los valores exactos individuales (no sabemos si esos datos eran un 11, un 15 o un 19). Para poder calcular estadísticos como la media aritmética posteriormente, debemos calcular el punto medio del intervalo, el cual actuará como el representante oficial de todos los datos en esa clase:
$$\text{Marca de clase}=mca=\frac{L_{inf}+L_{sup}}{2}$$
Por ejemplo:

| $x_i$     | $f_i$ | $f_{ri}$ | $F_i$ | $F_{ri}$ | $mca_i$ |
| --------- | ----- | -------- | ----- | -------- | ------- |
| [329-370) | 5     | 0.217    | 5     | 0.217    | 349.5   |
| [370-411) | 7     | 0.304    | 12    | 0.474    | 390.5   |
| [411-452] | 11    | 0.478    | 23    | 1        | 431.5   |

>[!informacion] La pérdida de información vs. la ganancia de comprensión
>Agrupar los datos implica un sacrificio: perdemos el valor numérico exacto de cada observación original para ganar una visión general del comportamiento del sistema. Esta tabla agrupada es el esqueleto matemático que luego utilizaremos para graficar el **Histograma**, donde finalmente diagnosticaremos la forma y dispersión del fenómeno físico.


