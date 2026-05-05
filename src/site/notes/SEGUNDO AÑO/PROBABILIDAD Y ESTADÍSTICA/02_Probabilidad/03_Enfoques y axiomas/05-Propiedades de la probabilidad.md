---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/03-enfoques-y-axiomas/05-propiedades-de-la-probabilidad/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #propiedades #regla_aditiva #complemento

>[!informacion] Vinculación
>A partir de los tres axiomas fundamentales de Kolmogorov: [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/03_Enfoques y axiomas/04-Enfoque axiomático (Kolmogorov)\|04-Enfoque axiomático (Kolmogorov)]], se inicia la construcción de toda la teoría para el cálculo de probabilidades. Las siguientes propiedades son **teoremas demostrables** que derivan directamente de esos axiomas y son nuestras herramientas matemáticas principales para resolver problemas.

---
# 1. Probabilidad del suceso imposible
Si $\emptyset$ representa el conjunto vacío (suceso imposible), entonces su probabilidad es cero:
$$
P(\emptyset)=0
$$
*Interpretación:* A los eventos simples que no tienen ninguna posibilidad física de ocurrir dentro del experimento se les asigna una probabilidad nula.

#### Demostración
Consideramos el espacio muestral completo $\ohm$ y el conjunto vacío $\emptyset$. Si unimos todo lo que puede pasar con la nada misma, seguimos teniendo lo que puede pasar:
$$\ohm\cup\emptyset=\ohm$$
Evidentemente, $\ohm$ y $\emptyset$ son mutuamente excluyentes, porque el conjunto vacío no tiene elementos. Aplicamos la probabilidad a la ecuación del paso 1 y usamos el **Axioma 3**:
$$
P(\ohm)+P(\emptyset)=P(\ohm)
$$
Por el **Axioma 1**, sabemos que $P(\ohm)=1$. Reemplazamos en ambos lados y tenemos:
$$1+P(\emptyset)=1$$
Pasamos el 1 restando al otro lado:
$$P(\emptyset)=1-1 \ \ \ \ \to \ \ \ \ P(\emptyset)=0$$
>[!done] Demostrado

---
## 2. Probabilidad del suceso complementario
Para cualquier evento $A$, la probabilidad de que no ocurra (su complemento $A'$ o $A^c$) es igual a 1 menos la probabilidad de que sí ocurra:
$$
P(A^c)=1-P(A)
$$
>[!tip] Tip de práctica
>Esta regla es vital en la práctica. A menudo es mucho más fácil calcular la probabilidad de que un evento no ocurra, para luego deducir la probabilidad de que sí ocurra. Es especialmente útil cuando los problemas de confiabilidad o calidad incluyen la frase "por lo menos uno".

#### Demostración
Sabemos por teoría de conjuntos que un suceso $A$ y su complemento $A^c$ abarcan todo el espacio muestral disponible. Al unirlos, tenemos el total:
$$A\cup A^c=\ohm$$
También sabemos por lógica que no pueden ocurrir al mismo tiempo: es decir, son mutuamente excluyentes.
$$
A\cap A^c=\emptyset
$$
Aplicamos la función de probabilidad a ambos lados de la ecuación del primer paso:
$$
P(A\cup A^c)=P(\ohm)
$$
Por el Axioma 1, sabemos que $P(\ohm)=1$. Reemplazamos:
$$
P(A\cup A^c)=1
$$
Como probamos en el paso 2 que son excluyentes, podemos aplicar el Axioma 3 para separar la unión en una suma:
$$P(A)+P(A^c)=1$$
Despejamos $P(A^c)$:
$$
P(A^c)=1-P(A)
$$
>[!done] Demostrado

---
## 3. Monotonía (subconjuntos)
Si un evento $A$ está completamente contenido dentro de un evento $B$ (es decir, $A\subset B$), entonces la probabilidad de $A$ nunca puede superar a la de $B$:
$$
P(A)\leq P(B)
$$
*Interpretación:* Si la ocurrencia del defecto $A$ implica obligatoriamente la ocurrencia del defecto $B$, el defecto $B$ tiene que ser al menos igual o más probable que el $A$.

#### Demostración
Como $A$ está dentro de $B$, podemos expresar el conjunto $B$ grande como la unión de dos pedazos que no se toca: el círculo $A$ por un lado, y todo lo que está en $B$ pero afuera de $A$ por otro. Matemáticamente, esto es:
$$B=A\cup (B\cap A^c)$$
Sabemos que el pedazo $A$ y el pedazo $(B\cap A^c)$ son mutuamente excluyentes (no tienen intersección). Por lo tanto, podemos aplicar el Axioma 3 (regla de la adición para sucesos mutuamente excluyentes):
$$P(B)=P(A)+P(B\cap A^c)$$
Ahora entra en juego el Axioma 1 (no negatividad). Sabemos que la probabilidad de cualquier suceso, por más raro que sea, siempre es mayor o igual a cero. Entonces, la probabilidad de esa "corteza" $(B\cap A^c)$ tiene que cumplir que:
$$
P(B\cap A^c)\leq0
$$
Si miramos la ecuación del segundo paso, $P(B)$ es igual a $P(A)$ sumándole "algo" que sabemos que es positivo o cero. Por lo tanto, obligatoriamente $P(B)$ tiene que ser mayor o igual a $P(A)$
$$P(A)\leq P(B)$$
>[!done] Demostrado

---
## 4. Regla de la cota superior
Si cualquier evento $A$ es un subconjunto del espacio muestral ($A\subset \ohm$), entonces su probabilidad no puede ser mayor que 1. Al combinar esto con el Axioma 1 de no negatividad, obtenemos el rango absoluto de la probabilidad:
$$0\leq P(A)\leq1$$
*Interpretación:* La probabilidad siempre será un número fraccionario (o porcentaje) acotado entre la imposibilidad absoluta (0) y la certeza absoluta (1).

#### Demostración
Por definición fundamental, cualquier suceso o evento $A$ que estemos estudiando pertenece a nuestro experimento. Por lo tanto, todos los elementos de $A$ están contenidos dentro de nuestro espacio muestral total $\ohm$. Matemáticamente:
$$A\subset \ohm$$
Como acabamos de demostrar la propiedad de monotonía (propiedad 3), si un conjunto está dentro de otro, su probabilidad debe ser menor o igual. Aplicamos eso directo a nuestro caso:
$$P(A)\leq P(\ohm)$$
Finalmente, usamos el axioma 2, que decreta como verdad absoluta que la probabilidad del espacio muestral completo es 1 ($P(\ohm)=1$). Reemplazamos esto en la igualdad del paso anterior:
$$P(A)\leq1$$
>[!done] Demostrado

---
## 5. Regla aditiva general
*(Para sucesos no excluyentes)* El Axioma 3 de Kolmogorov nos enseñó que si dos eventos son mutuamente excluyentes (no tienen intersección), sus probabilidades se suman directamente. Pero, ¿Qué pasa si dos eventos si pueden ocurrir al mismo tiempo?

Aquí utilizamos la propiedad de la Regla Aditiva General:
$$
P(A\cup B)=P(A)+P(B)-P(A\cap B)
$$
*Interpretación:* $P(A\cup B)$ es la probabilidad de que ocurra $A$, ocurra $B$, o ambos. Al sumar $P(A)$ y $P(B)$, estamos sumando las probabilidades de la intersección ($A\cap B$) dos veces (un "doble conteo"). Para obtener el resultado correcto, debemos corregir esto restando la intersección una vez.

#### Demostración
![Pasted image 20260424144437.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260424144437.png)

Descomponemos el suceso $A\cup B$ en dos fragmentos que sean mutuamente excluyentes (para poder usar el Axioma 3). Imaginemos los dos círculos de Venn; la unión total es igual a todo el círculo A, más el pedacito de $B$ que "sobra" por fuera de $A$:
$$A\cup B=A\cup (B\cap A^c)$$
Aplicamos probabilidad. Como $A$ y el fragmento $(B\cap A^c)$ no se tocan, usamos el Axioma 3:
$$
P(A\cup B)=P(A)+P(B\cap A^c)
$$
Ahora nuestro problema es encontrar cuánto vale esa pieza extraña $P(B\cap A^c)$. Para eso, analizamos el círculo $B$. El círculo $B$ se descompone del centro compartido y el pedacito que sobra:
$$B=(A\cap B)\cup(B\cap A^c)$$
Como esas dos partes de $B$ son mutuamente excluyentes, les aplicamos probabilidad con el Axioma 3:
$$
P(B)=P(A\cap B)+P(B\cap A^c)
$$
De esta última ecuación, despejamos la pieza extraña $P(B\cap A^c)$ pasando la intersección restando:
$$
P(B\cap A^c)=P(B)-P(A\cap B)
$$
Finalmente, metemos este reemplazo en la ecuación que dejamos en espera en el paso 2:
$$
P(A\cup B)=P(A)+[P(B)-P(A\cap B)]
$$
$$P(A\cup B)=P(A)+P(B)-P(A\cap B)$$
>[!done] Demostrado

---
## 6. Ejemplo de aplicación
En una encuesta de respuestas no excluyentes se ha encontrado que se consumen dos tipos de mezclas: marcas $A$ y $B$. e ha registrado que:
- El 30% consume por lo menos $A\to P(A)=0.3$.
- El 60% consume por lo menos $B\to P(B)=0.6$.
- El 5% consume los dos tipos $P(A\cap B)=0.05$.

Si se elige un formulario al azar, ¿cuál es la probabilidad de...

**1. ... que indique el consumo de alguno de los dos tipos?**
Esto es "A o B". Aplicamos la propiedad de la regla aditiva general:
$$P(A\cup B)=P(A)+P(B)-P(A\cap B)$$
$$
P(A\cup B)=0.3+0.6-0.05=0.85\to(85\%)
$$

**2. ... que consuma sólo A?**
Consumir "sólo A" significa que consume $A$ pero no $B$. Matemáticamente, es la diferencia $A-B$, o bien, la probabilidad de $A$ menos la porción de $A$ que comparte con $B$:
$$P(A-B)=P(A)-P(A\cap B)$$
$$P(A-B)=0.3-0.05=0.25\to(25\%)$$

**3. ... que no consuma ningún tipo?**
Esto significa que no consume ni A ni B. Es el complemento exacto de "consumir alguno de los dos tipos" $(A\cup B)$. Aplicamos la propiedad de la regla del complemento y las Leyes de De Morgan:
$$
P(A^c\cap B^c)=P((A\cup B)^c)=1-P(A\cup B)
$$
$$
P((A\cup B)^c)=1-0.85=0.15 \to (15\%)
$$
