---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/01-fundamentos-matematicos/03-tecnicas-de-conteo/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #técnicas_de_conteo #combinatoria

Si los resultados de un experimento son igualmente probables, el cálculo de las probabilidades se reduce a contar: la probabilidad de un evento es simplemente el número de resultados favorables dividido por el número total de resultados posibles en el espacio muestral. Sin embargo, cuando el experimento es complejo, elaborar una lista manual

---
## 1. Regla del producto
Es la regla base de toda combinatoria. Se aplica cuando un evento o experimento está compuesto por una secuencia de pasos u operaciones.

>[!definicion] Definición: Regla del producto
>Si una operación se puede ejecutar de $n_1$ formas, y por cada una de éstas se puede llevar a cabo una segunda operación en $n_2$ formas, y una tercera en $n_3$ formas, y así sucesivamente, entonces la serie de $k$ operaciones se puede realizar en $n_1\cdot n_2 \cdot \text{...} \cdot n_k$ formas.

**Diagramas de árbol:** Son una excelente herramienta visual para representar esta regla. Partiendo de un punto inicial, se trazan ramas para cada opción de la primera etapa ($n_1$ ramas). Desde la punta de cada una de esas ramas, se trazan nuevas ramas para las opciones de la segunda etapa ($n_2$), y así sucesivamente. Al contar las puntas finales del árbol, obtienes el total exacto que da la multiplicación.

![Pasted image 20260423133637.png\|375](/img/user/IM%C3%81GENES/Pasted%20image%2020260423133637.png)

---
## 2. Permutaciones

>[!warning] ¡El orden SÍ importa!

Con frecuencia, el espacio muestral consta de todos los arreglos u ordenaciones posibles de un grupo de objetos.

>[!definicion] Definición: Permutación
>Una permutación es un arreglo ordenado de todo o parte de un conjunto de objetos. En las permutaciones, el conjunto {$A,B,C$} se considera distinto del conjunto {$B,A,C$} porque el orden de aparición es relevante.

**Notación factorial**
Para calcular permutaciones se usa el factorial de un número, denotado por $n!$. Se define como el producto descendente de enteros:
$$n!=n(n-1)(n-2)...(2)(1)$$
Por definición matemática: $0!=1$.

**Fórmula principal**
El número de permutaciones (arreglos ordenados) de $n$ objetos distintos tomados de $r$ a la vez (donde $r\leq n$) se denota como $P_{r,n}$ o $_nP_r$  se calcula como:
$$
_nP_r=\frac{n!}{(n-r)!}
$$

**Casos especiales de permutaciones**
- Permutaciones circulares:
  Si vamos a ordenar $n$ objetos en un círculo (donde no hay un principio ni un fin predeterminado), el número de arreglos es $(n-1)!$.
- Objetos indistinguibles:
  Si tenemos $n$ objetos en total, pero algunos de ellos son idénticos entre sí (por ejemplo, $n_1$ son de un tipo, $n_2$ de otro, etc.), el número de permutaciones distintas es:
$$
\frac{n!}{n!n2!...n_k!}
$$
---
## 3. Combinaciones

>[!check] ¡El orden NO importa!

>[!definicion] Definición: Combinación
>Una combinación es un subconjunto no ordenado. Seleccionar las piezas defectuosas {$pieza_1,pieza_8$} es exactamente el mismo evento que seleccionar {$pieza_8,pieza_1$}.

**Fórmula principal**
El número de combinaciones de $n$ objetos distintos tomados de $r$ a la vez se denota frecuentemente como $(_{r}^n$) (se lee "$n$ sobre $r$") o $C_{r,n}$. Se calcula dividiendo el número de permutaciones entre las formas en que se pueden ordenar internamente esos $r$ elementos seleccionados (es decir, dividiendo por $r!$):
$$\left(_{r}^n\right)=\frac{n!}{r!(n-r)!}$$
---
>[!cuidado] Permutación vs. Combinación
>El error más común al resolver probabilidades clásicas es confundir qué fórmula usar. Siempre debemos preguntarnos al leer el enunciado: **¿Cambia el resultado físico si altero el orden de selección?**
>- Si asignamos cargos distintos (ej. presidente y tesorero), entonces el orden altera el resultado $\to$ **PERMUTACIÓN** ($nPr$).
>- Si elegimos un comité de personas iguales, o seleccionamos piezas de un lote para inspeccionarlas en un laboratorio, entonces el orden no altera el resultado $\to$ **COMBINACIÓN** ($_r^n$).


