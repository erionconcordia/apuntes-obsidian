---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/03-enfoques-y-axiomas/04-enfoque-axiomatico-kolmogorov/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #enfoque_axiomático #kolmogorov #axiomas_de_probabilidad

>[!informacion] Vinculación
>Los enfoques clásico, frecuencial y subjetivo nos dicen *cómo calcular o estimar* un número para la probabilidad en la vida real. Sin embargo, matemáticamente hablando, necesitamos reglas inquebrantables que garanticen que nuestras asignaciones de probabilidad sean consistentes. Aquí es donde entra el enfoque axiomático.

---
## 1. Introducción y filosofía

>[!importante] Aclaración
>Esto es solamente algo de historia de quién es el creador de la filosofía, no es tan importante en la teoría.

Formalizado por el matemático ruso Andréi Kolmogorov en 1933, este enfoque es el más abstracto y el menos intuitivo de todos. No nos dice explícitamente cómo calcular la probabilidad de un evento específico, sino que introduce la probabilidad como un "término primitivo".

Su inmensa potencia radica en que permite construir una teoría matemática rigurosa de la probabilidad. Al establecer una serie de axiomas (verdades fundamentales que no requieren demostración), este sistema es tan potente que incluye a los enfoques clásico, frecuencial y subjetivo como casos particulares.

---
## 2. Axiomas de la probabilidad
Sea un experimento aleatorio $A$ con su espacio muestral $\ohm$ (denotado como $S$ en la bibliografía). La función $P:\ohm\to\mathbb{R}$ se considera una "función de probabilidad" legítima si, y sólo si, verifica los siguientes tres axiomas:

**Axioma 1: No negatividad**
Para cualquier evento $A$, su probabilidad debe ser mayor o igual a cero:
$$
P(A)\geq0
$$
*Interpretación:* Refleja la noción intuitiva de que no pueden existir "oportunidades negativas" de que ocurra un evento.

**Axioma 2: Certeza del Espacio Muestral**
La probabilidad de todo el espacio muestral es 1:
$$
P(\ohm)=1 \ \ \ \ \ (\text{o }P(S)=1\text{ en notación de los libros})
$$
*Interpretación:* Como el espacio muestral contiene absolutamente todos los resultados posibles, al realizar el experimento es 100% seguro que el resultado caerá dentro de $\ohm$. Es la máxima probabilidad posible.

**Axioma 3: Aditividad para sucesos mutuamente excluyentes**
Si $A_1,A_2,...,A_n,...$ es un conjunto (finito o infinito) de eventos mutuamente excluyentes (es decir, disjuntos, donde $A_i\cap A_j=\emptyset$ para cualquier $i\neq j$), entonces la probabilidad de su unión es la suma de sus probabilidades individuales:
$$
P\left(\bigcup_{i=1}^{\infty}A_i\right)=\sum_{i=1}^{\infty}P(A_i)
$$
*Interpretación:* Formaliza la idea de que si se desea la probabilidad de que ocurra "al menos uno" de varios eventos, y es físicamente imposible que ocurran dos al mismo tiempo, las probabilidades individuales simplemente se suman.

---
## 3. Algunas preguntas de relación teórica

**¿Qué diferencia existe entre este enfoque y los anteriores?**
Mientras los otros enfoques son interpretaciones prácticas para asignar un valor al azar (contando casos, repitiendo experimentos o usando el juicio), el enfoque axiomático es una estructura matemática abstracta que simplemente establece las reglas que cualquier probabilidad debe cumplir para ser válida.

**¿Alguno de los otros enfoques es incorrecto?**
¡Ninguno es incorrecto! Todos son válidos y útiles en la ingeniería dependiendo del escenario (juegos de azar, producción en masa o eventos únicos irrepetibles). Todos ellos respetas y satisfacen rigurosamente los tres axiomas de Kolmogorov.

**¿Qué ventaja teórica y metodológica tiene?**
Garantiza consistencia. Nos permite utilizar toda la potencia del análisis matemático y la teoría de conjuntos para derivar propiedades complejas (como los teoremas de Probabilidad Total y Bayes) sin importar si calculamos el número usado en el enfoque de Laplace o el frecuencial.
