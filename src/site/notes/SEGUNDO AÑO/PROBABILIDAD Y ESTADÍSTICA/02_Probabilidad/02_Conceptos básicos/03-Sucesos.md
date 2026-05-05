---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/02-conceptos-basicos/03-sucesos/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #sucesos #eventos #mutuamente_excluyentes #complementarios

>[!informacion] Vinculación matemática
>Todo lo que aplica a los sucesos se rige por las leyes descritas en [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/01_Fundamentos matemáticos/02-Revisión de teoría de conjuntos\|02-Revisión de teoría de conjuntos]]

## 1. Sucesos o eventos
En el contexto de un experimento aleatorio, no siempre estamos interesados en un único resultado específico, sino en sí el resultado cumple con cierta condición o característica.

>[!definicion] Definición: Suceso
>Un evento o suceso es cualquier recopilación o subconjunto de resultados contenidos en el espacio muestral. Es decir, el conjunto $A$ es un evento de $\ohm$ si $A\subset\ohm$.

Dependiendo de la cantidad de resultados que abarquen, se clasifican en:
- **Suceso simple:** Aquel evento que consiste en exactamente un solo resultado posible del espacio muestral.
- **Suceso compuesto:** Aquel que consiste en más de un resultado posible.

*Ejemplo:* Supongamos que probamos tres componentes electrónicos y los clasificamos como Defectuosos (D) o No defectuosos (N). El espacio muestral es: $\ohm=$ {$DDD,DDN,DND,DNN,NDD,NDN,NND,NNN$}
- El evento $E_1=$ "Los tres componentes fallan" es el subconjunto {$DDD$}. Al tener un solo resultado, es un suceso simple.
- El evento $A=$ "Exactamente un componente es defectuoso" es el subconjunto {$DNN,NDN,NND$}. Al contener tres resultados distintos, es un suceso compuesto.

---
## 2. Sucesos mutuamente excluyentes

>[!definicion] Definicion: Sucesos mutuamente excluyentes
>Dos eventos $A$ y $B$ son mutuamente excluyentes o disjuntos si no tienen elementos en común, es decir, si su intersección es el conjunto vacío: $(A\cap B=\emptyset)$.

En la práctica, decir que dos sucesos son mutuamente excluyentes significa que no pueden ocurrir de forma simultánea en un mismo ensayo del experimento.
- *Ejemplo:* Si observamos un vehículo llegar a una intersección, el evento $A$ (el vehículo gira a la izquierda) y el evento $B$ (el vehículo sigue derecho) son mutuamente excluyentes. El vehículo no puede hacer ambas cosas al mismo tiempo.

>[!important] Probabilidad del ejemplo
>  Si nos solicitan la probabilidad de que en el ejemplo anterior ocurran $A$ y $B$ simultáneamente, y sabemos que son sucesos mutuamente excluyentes, esa probabilidad siempre será cero.

---
## 3. Sucesos complementarios

>[!definicion] Definición: Sucesos complementarios
>El complemento de un evento $A$ respecto de $\ohm$ es el subconjunto de todos los elementos (o resultados) de $\ohm$ que no están contenidos en $A$. Generalmente se denota con el símbolo $A'$ o $A^c$.

Todo evento $A$ y su complemento $A'$ siempre son **mutuamente excluyentes** (no podemos tener un componente defectuoso y no defectuoso a la vez) y además, son exhaustivos (entre los dos cubren absolutamente todo el espacio muestral $\ohm$).

**Ejemplo en ingeniería:** Dado el espacio muestral $\ohm=$ {$t|t\geq0$}, donde $t$ es la vida útil en años de cierto componente electrónico. Si definimos el evento $A$ de que el componente falle antes de que finalice el quinto año, es decir $A=$ {$t|0\leq t<5$}, entonces el suceso complementario $A'$ es el evento de que el componente dure 5 años o más, es decir $A'=(t|t\geq 5)$.


