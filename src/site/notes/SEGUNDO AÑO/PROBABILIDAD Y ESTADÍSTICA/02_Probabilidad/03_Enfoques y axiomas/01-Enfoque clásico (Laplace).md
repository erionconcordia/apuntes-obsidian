---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/03-enfoques-y-axiomas/01-enfoque-clasico-laplace/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #enfoque_clasico #laplace #equiprobabilidad

>[!informacion] Vinculación
>Este enfoque es la aplicación directa de las [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/01_Fundamentos matemáticos/03-Técnicas de conteo\|03-Técnicas de conteo]], ya que la resolución de probabilidades aquí se reduce puramente a contar resultados.

---
## 1. Definición y el "Principio de razón insuficiente"
El enfoque clásico, formalizado históricamente por Pierre-Simon Laplace, es el método más antiguo e intuitivo para calcular probabilidades, surgido del análisis de los juegos de azar.

**Basado en:** Principio de razón insuficiente

>[!definicion] Principio de razón insuficiente
>Este principio establece que, si no tenemos ninguna razón o evidencia para pensar que un resultado es más probable que otro, debemos asumir que **todos los resultados experimentales tienen exactamente la misma probabilidad de ocurrir**.

---
## 2. La fórmula de Laplace
Si un experimento tiene un espacio muestral $\ohm$ que contiene un número finito $N$ da resultados posibles, y asumimos que todos son **igualmente probables** (equiprobables), le asignamos una probabilidad de $1/N$ a cada punto muestral.

Por lo tanto, la probabilidad de que ocurra un evento $A$ que contiene exactamente $n$ resultados favorables se define como el cociente entre el número de elementos en $A$ y el número total de elementos en el espacio muestral.
$$
P(A)=\frac{\text{Número de resultados favorables (n)}}{\text{Número total de resultados posibles (N)}}
$$
>[!warning] Advertencia
>No confundir $n$ y $N$ con el número de muestra y el número de población.

---
## 3. Ejemplos clásicos (aplicación de la cátedra)

#### Ejemplo 1: Arrojar un dado equilibrado
*¿Qué probabilidad tengo de obtener al menos un 4 al arrojar un dado equilibrado?*

Como el dado está "equilibrado", aplicamos la razón insuficiente: las 6 caras son equiprobables.

$\ohm=\{1,2,3,4,5,6\}\to N=6$
$A=\text{"Obtener al menos un 4"}=\{4,5,6\}\to n=3$
$$
P(A)=\frac{3}{6}=0.5\to50\%
$$

#### Ejemplo 2: Lanzamiento de monedas
*¿Qué probabilidad tengo de obtener dos caras al arrojar una moneda tres veces consecutivas?*

Cada lanzamiento es independiente. Si usamos la regla del producto para contar el espacio muestral: $2\cdot 2\cdot 2=8$ resultados posibles.

$\ohm=\{ CCC,CCX,CXC,XCC,XXC,XCX,CXX,XXX\} \ \to \ N=8$
$A=\text{"Obtener exactamente dos caras (C)"}=\{CCX,CXC,XXC\} \to n=3$
$$
P(A)=\frac{3}{8}=0.375\to37.5\%
$$
---
## 4. Limitaciones del enfoque clásico
En la ingeniería moderno, el enfoque de Laplace presenta tres defectos gravísimos que obligan a usar otros métodos.

1. **Exige equiprobabilidad:** Sólo funciona si todos los resultados tienen la misma probabilidad de ocurrir (ej. dados "legales"). Si un dado está cargado o un proceso de manufactura tiene sesgos, este enfoque falla inmediatamente.
2. **Limitado a espacios finitos:** El número de resultados posibles ($N$) debe ser finito. Si evaluamos variables continuas (como el tiempo de falla de un componente o el voltaje), el denominador tiende a infinito y la fórmula colapsa.
3. **Circularidad:** Define la "probabilidad" asumiendo que los eventos son "igualmente probables", lo cual es un argumento circular y lógicamente débil para la ciencia.

