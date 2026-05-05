---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/02-conceptos-basicos/04-operaciones-con-sucesos/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #eventos_compuestos #operaciones

>[!informacion]  Vinculación
>El sustento matemático de las operaciones que veremos a continuación se encuentra detallado en: [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/01_Fundamentos matemáticos/02-Revisión de teoría de conjuntos\|02-Revisión de teoría de conjuntos]].

---
## 1. Unión de Sucesos ($A\cup B$)
La unión de dos eventos A y B es el evento que contiene todos los resultados que pertenecen a A, a B, o a ambos.
![Pasted image 20260424105658.png\|212](/img/user/IM%C3%81GENES/Pasted%20image%2020260424105658.png)

**Lectura probabilística:** Ocurre si ocurra $A$ "o" ocurre $B$ (inclusive si ocurren ambos al mismo tiempo)

**Ejemplo:** Sea $P$ el evento de que un empleado de una petrolera fume cigarrillos y $Q$ el evento de que ingiera bebidas alcohólicas. El evento compuesto $P\cup Q$ representa el conjunto de empleados que fuman, que beben, o que hacen ambas cosas.

## 2. Intersección de Sucesos ($A\cap B$)
La intersección de dos eventos $A$ y $B$ es el evento que contiene todos los resultados que son comunes tanto a $A$ como a $B$.
![Pasted image 20260424105640.png\|221](/img/user/IM%C3%81GENES/Pasted%20image%2020260424105640.png)

**Lectura probabilística:** Ocurre si ocurren $A$ y $B$ de manera simultánea.

**Ejemplo:** Sea $E$ el evento de que una persona seleccionada en la facultad sea estudiante de ingeniería, y sea $F$ el evento de que la persona sea mujer. Entonces $E\cap F$ es el evento de que la persona seleccionada sea una estudiante mujer de ingeniería.

## 3. Complemento de un suceso ($A'$ o $A^c$)
El complemento de un evento $A$ respecto del espacio muestral $\ohm$ es el subconjunto de todos los elementos de $\ohm$ que no está en $A$.
![Pasted image 20260424105926.png\|205](/img/user/IM%C3%81GENES/Pasted%20image%2020260424105926.png)

**Lectura probabilística:** Es el evento de que NO ocurra el evento $A$.

**Ejemplo:** Si inspeccionamos cartas, y $A$ es el evento de que una carta seleccionada sea roja, entonces $A'$ es el evento de que la carta seleccionada NO sea roja (es decir, que sea negra).

## 4. Diferencia de sucesos ($A-B$ o $A\cap B'$)
![Pasted image 20260424110113.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260424110113.png)
**Lectura probabilística:** Ocurre $A$ pero no ocurre $B$.

**Ejemplo:** Si $A$ es el evento de que un producto tenga defectos de longitud y $B$ es que tenga defectos de textura, el evento $A-B$ representa a los productos que tienen defectos de longitud pero su textura está en perfectas condiciones.

---
# El uso de las Leyes de De Morgan en probabilidad
Las propiedades del álgebra de conjuntos son atajos fundamentales para calcular probabilidades. Entre todas las leyes, tu cátedra destaca unas que son vitales para simplificar problemas complejos: las **Leyes de De Morgan**.

Estas leyes nos enseñan cómo interactúa la negación (el complemento) con las uniones e intersecciones, transformando "O" en "Y" y viceversa:

**1. El complemento de una unión es la intersección de los complementos:**
$$(A\cup B)'=A'\cap B'$$
- Traducción: *"Que no ocurra ni A ni B" es exactamente lo mismo que "Que no ocurra A **y** que no ocurra B".*

**2. El complemento de una intersección es la unión de los complementos:*
$$(A\cap B)'=A' \cup B'$$
- Traducción práctica: *"Que no ocurran A y B al mismo tiempo" es lo mismo que "Que no ocurra A **o** que no ocurra B".*

>[!tip] Tip para problemas
>En problemas de confiabilidad de sistemas, a menudo pedirán calcular la probabilidad de que el "sistema no falle" (Complemento). Para un sistema donde basta que falle un componente $(A\cup B)$, la probabilidad de que todo funcione perfecto es justamente $(A\cup B)'=A'\cap B'$, es decir, que el componente $A$ funcione bien y el $B$ también.

