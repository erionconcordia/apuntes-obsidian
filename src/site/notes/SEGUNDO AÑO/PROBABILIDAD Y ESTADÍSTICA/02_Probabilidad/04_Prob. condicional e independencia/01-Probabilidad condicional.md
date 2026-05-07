---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/04-prob-condicional-e-independencia/01-probabilidad-condicional/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #probabiidad_condicional

>[!dato] Pregunta disparadora
>¿Cómo se modifica el cálculo de una probabilidad si se conoce cierta información previamente?

---
## 1. Concepto de Probabilidad condicional
En muchas aplicaciones, la información de que un evento $B$ "ha ocurrido" altera la probabilidad asignada a un evento $A$. A la nueva probabilidad actualizada de $A$, basada en el conocimiento de que $B$ ya sucedió, se le llama probabilidad condicional.

>[!definicion] Definición: Probabilidad condicional
>Dados dos sucesos $A$ y $B$ en un espacio muestral $\ohm$, la probabilidad condicional del suceso $A$ dado que ocurrió $B$ se denota como $P(A|B)$ o $P(A/B)$ y se define como:
>$$P(A/B)=\frac{P(A\cap B)}{P(B)},\ \ \ \ \ \text{siempre que P(B)>0}$$

#### Demostración
**Axioma 1:**
$P(A/B)\geq0$
$$P(A/B)=\frac{P(A\cap B)}{P(B)}$$
Donde: $P(B)>0$ y $P(A\cap B)\geq0$, entonces, se demuestra el axioma 1: $$P(A/B)\geq0$$
**Axioma 2:**
$P(\ohm/B)=1$
$$P(\ohm/B)=\frac{P(\ohm\cap B)}{P(B)}=\frac{P(B)}{P(B)}=1$$

**Axioma 3:**
 $P(A_1\cup A_2/B)=P(A_1/B)+P(A_2/B)$
Aplicamos la definición de probabilidad condicional:
$$
P(A_1\cup A_2/B)=\frac{P((A_1\cup A_2)\cap B)}{P(B)}
$$
En el numerador tenemos una unión de conjuntos con intersección $B$. Por teoría de conjuntos, podemos distribuir esa intersección:
$$(A_1\cup A_2)\cap B=(A_1\cap B)\cup(A_2\cap B)$$
Entonces:
$$P(A_1\cup A_2/B)=\frac{P((A_1\cap B)\cup(A_2\cap B))}{P(B)}$$
Sabemos desde el principio que $A_1$ y $A_2$ son mutuamente excluyentes (no se tocan). Por puro sentido común, si $A_1$ y $A_2$ no tienen nada en común, entonces el pedacito de $A_1$ que toca $B$ y el pedacito de $A_2$ que toca a $B$, tampoco pueden tener nada en común, entonces:
$$(A_1\cap B)\cap(A_2\cap B)=\emptyset \ \ \ \ \to \ \ \ \ \text{(Son mutuamente excluyentes)}$$
Uso el tercer axioma en el numerador de la fracción:
$$P((A_1\cap B)\cup(A_2\cap B))=P(A_1\cap B)+P(A_2\cap B)$$
Sustituimos el numerador por esta nueva suma:
$$P(A_1\cup A_2/B)=\frac{P(A_1\cap B)+P(A_2\cap B)}{P(B)}=\frac{P(A_1\cap B)}{P(B)}+\frac{P(A_2\cap B)}{P(B)}$$
Entonces, terminamos por demostrar que:
$$P(A_1\cup A_2/B)=P(A_1/B)+P(A_2/B)$$
Se cumple el axioma 3.

>[!done] Demostrado

---
## 2. Interpretación visual: El espacio muestral reducido
Físicamente, ¿qué estamos haciendo al dividir entre $P(B)$? Al saber con certeza que el evento $B$ ha ocurrido, nuestro espacio muestral $\ohm$ ya no nos sirve. El espacio muestral se reduce netamente al conjunto $B$.

![Pasted image 20260424150627.png\|261](/img/user/IM%C3%81GENES/Pasted%20image%2020260424150627.png)

Por lo tanto, para que ocurra $A$, el resultado debe estar forzosamente en la intersección $A\cap B$. La fórmula simplemente calcula qué porción representa la intersección $A\cap B$ respecto a la totalidad del nuevo espacio de referencia $B$.

---
## 3. Regla de la multiplicación (Probabilidad conjunta)
Al despejar el numerador de la fórmula de probabilidad condicional multiplicando por $P(B)$, obtenemos una de las reglas más útiles en estadística, conocida como la regla del producto o multiplicativa.
$$
P(A\cap B)=P(B)\cdot P(A/B)
$$
>[!observacion] Nota
>Como la intersección es conmutativa, también es válido escribir:
>$$P(A\cap B)=P(A)\cdot P(B/A)$$

Esta regla es fundamental cuando analizamos experimentos que ocurren en etapas sucesivas (muy comunes en los diagramas de árbol), ya que nos permite calcular la probabilidad de que ocurran dos eventos en conjunto multiplicando la probabilidad del primero por la probabilidad condicional del segundo.

---
# Ejemplo práctico
Se toma una muestra de registros con los siguientes resultados cruzados:

| °F      | H1  | H2  | H3  | *Total* |
| ------- | --- | --- | --- | ------- |
| **500**     | 16  | 10  | 20  | 46      |
| **600**     | 14  | 9   | 15  | 38      |
| ***Total*** | 30  | 19  | 35  | 84      |
Resolución de las probabilidades condicionales:

**1. Probabilidad de que sea un registro del $H_1$ si se sabe que fue expuesto a 600°**
$$P(H_1/600°)=\frac{P(H_1\cap 600°)}{P(600°)}$$
En la tabla de valores vemos que la intersección entre $H_1$ y 600° es 14, y el total de la fila 600° es 38. Por lo tanto, la probabilidad es:
$$P(H_1/600°)=\frac{14}{38}\approx0.368$$
*Nos olvidamos de los 84 registros totales y miramos solamente la fila de los 38 que estuvieron a 600°.*

**2. Probabilidad de que ocurra $H_1$**
$$
P(H_1)=\frac{30}{84}\approx0.357
$$

**3. Probabilidad de que ocurra 500° si ocurrió $H_3$**
$$
P(500°/H_3)=\frac{P(500°\cap H_3)}{P(H_3)}
$$
La intersección de 500° y $H_3$ es 20. El total de registros del horno $H_3$ es 35. Entonces:
$$
P(500°/H_3)=\frac{20}{35}\approx0.571
$$

**4. La probabilidad de que ocurra $H_3$ si ya ocurrió 500°**
$$
P(H_3/500°)=\frac{P(H_3\cap 500°)}{P(500°)}
$$
La intersección sigue siendo 20, pero ahora la condición cambió. El universo se reduce a la fila de 500° (total 45). Entonces:
$$
P(H_3/500°)=\frac{20}{46}\approx0.434
$$
>[!warning] Alerta de orden
>Notemos como $P(500°/H_3)$ da un resultado distinto al de $P(H_3/500°)$. El orden en la condicional importa muchísimo físicamente porque define cuál es la información que se asume como 100% segura (el nuevo universo).

