---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/04-prob-condicional-e-independencia/02-sucesos-independientes/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #sucesos_independientes #independencia_mutua

>[!informacion] Vinculación
>Con $P(A/B)$ nos permite actualizar la probabilidad de $A$ si sabemos que $B$ ya ocurrió, pero ¿Qué sucede si la ocurrencia de $B$ no altera en absoluto la probabilidad de $A$? Ese es el núcleo de la independencia estocástica.

## 1. Concepto intuitivo y definición
Intuitivamente se dice que un evento es independiente de otro cuando la ocurrencia de uno no influye en la ocurrencia del otro.

Matemáticamente, esto significa que saber que el evento $B$ ha ocurrido no aporta ninguna información nueva que modifique la probabilidad original de $A$. Por lo tanto, la probabilidad condicional es exactamente igual a la probabilidad incondicional:
$$P(A/B)=P(A)$$
$$P(B/A)=P(B)$$
*Siempre que $P(A)>0$ y $P(B)>0$.*

Si estas desigualdades se cumplen, los eventos $A$ y $B$ son independientes. Si no se cumplen, se dice que son dependientes.

---
## 2. La regla de la multiplicación para independencia
En **probabilidad condicional** vimos la regla del producto general:
$$P(A\cap B)=P(B)\cdot P(A/B)$$
Si sustituimos la definición de independencia en esta ecuación, obtenemos la prueba matemática definitiva para comprobar la independencia estocástica:

>[!important] Condición de Independencia
>Dos eventos $A$ y $B$ son independientes si y sólo si la probabilidad de su intersección es el producto de sus probabilidades individuales:
>$$P(A\cap B)=P(A)\cdot P(B)$$

**Ejemplo:** Dos lanzamientos consecutivos de una moneda legal para observar la cara superior. El resultado del primer lanzamiento no afecta físicamente al segundo, por lo que:
$$P(Cara_1\cap Cara_2)=P(Cara_1)\cdot P(Cara_2)=0.5\cdot 0.5=0.25$$
---
## 3. Independencia mutua (más de 2 sucesos)

>[!definicion] Definición: independencia mutua
>Un conjunto de eventos $A_1,A_2,...,A_n$ son mutuamente independientes si para cualquier subconjunto de estos eventos, la probabilidad de su intersección es igual al producto de sus probabilidades individuales.

Para tres eventos $A,B,C$, la independencia mutua exige que se cumplan todas estas condiciones a la vez:
1. $P(A\cap B)=P(A)\cdot P(B)$
2. $P(A\cap C)=P(A)\cdot P(C)$
3. $P(B\cap C)=P(B)\cdot P(C)$
4. $P(A\cap B\cap C)=P(A)\cdot P(B)\cdot P(C)$

>[!observacion] Nota
>Que los eventos sean independientes "dos a dos", es decir, que cumplan solo las condiciones 1, 2 y 3, no garantiza que cumplan la condición 4. Deben verificarse todas para que sean mutuamente independientes.

---
## 4. Sucesos mutuamente excluyentes vs. independientes
*(Revisar [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/02_Conceptos básicos/03-Sucesos\|03-Sucesos]], ahí se nombran los mutuamente excluyentes)*. Este es uno de los errores conceptuales más comunes en los exámenes de probabilidad. Mutuamente excluyente e independiente NO son sinónimos; de hecho, casi siempre son conceptos opuestos

>[!warning] La trampa teórica
>Si dos sucesos $A$ y $B$ (con probabilidades mayores a cero) son **mutuamente excluyentes**, significa que si ocurre uno, el otro es físicamente imposible:
>$$P(A\cap B)=0$$
>Por lo tanto, si te dicen que $A$ ocurrió, tenemos la certeza absoluta de que $B$ no ocurrió. Esto significa que la ocurrencia de $A$ afecto drásticamente la probabilidad de $B$ (la redujo a cero: $P(B/A)=0$). Como la información de un evento altera la probabilidad del otro, **los eventos mutuamente excluyentes son altamente dependientes**.

---
## 5. Aplicación
La suposición de independencia es la base fundamental para calcular la confiabilidad de sistemas en serie y en paralelo.
- **Sistemas en Serie:** Un sistema de componentes conectados en serie funciona si y sólo si _todos_ los componentes funcionan. Si los componentes operan independientemente, la confiabilidad del sistema es la intersección de los éxitos:

$$
P(\text{Funciona sistema})=P(\text{C1 ​funciona})\cdot P(\text{C2 funciona})
$$
