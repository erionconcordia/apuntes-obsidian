---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/05-teoremas-fundamentales/01-ley-de-la-probabilidad-total/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #teorema_probabilidad_total #partición

>[!informacion] Vinculación
>Este teorema es la culminación de la [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/04_Prob. condicional e independencia/01-Probabilidad condicional\|01-Probabilidad condicional]]. Nos permite resolver problemas complejos dividiéndolos en partes más pequeñas y manejables.
>

---
## El requisito previo: Participación de un espacio muestral
Para poder aplicar la **Ley de la Probabilidad Total** (o el **Teorema de Bayes** más adelante), primero debemos entender cómo dividir nuestro espacio muestral $\ohm$ de forma correcta.

Se dice que un conjunto de eventos $\{B_1,B_2,...,B_n\}$ constituye una partición del espacio muestral si cumplen dos reglas estrictas:
1. **Son mutuamente excluyentes:** No pueden ocurrir al mismo tiempo.
2. **Son exhaustivos:** Entre todos cubren la totalidad de los resultados posibles del experimento (su unión es igual a $\ohm$).

---
# Teorema de la Probabilidad Total

>[!definicion] Teorema: Probabilidad Total (Regla de eliminación)
>Sea $\{B_1,B_2,...,B_n\}$ una partición de $\ohm$. Si $A$ es un evento cualquiera, su probabilidad total se calcula ponderando (multiplicando) la probabilidad de que ocurra cada escenario $B_i$ por la probabilidad de que $A$ ocurra en ese escenario, y luego sumando todo:
>$$
>P(A)=\sum_{i=1}^nP(B_i)\cdot P(A/B_i)
>$$

**Ejemplo:** Una planta de ensamble recibe productos provenientes de tres fabricantes A, B y C. El 50% del total se compra a A, mientras que a B y C se le compran el resto en partes iguales. El porcentaje de productos defectuosos para A, B y C, es de 5, 10 y 12% respectivamente. Determine la probabilidad de que una unidad ensamblada tenga un componente malo.

- $P(A)=0.5$
- $P(B)=0.25$
- $P(C)=0.25$
- $P(D/A)=0.05$
- $P(D/B)=0.1$
- $P(D/C)=0.12$

Aplicando el teorema:
$$P(D)=P(A)\cdot P(D/A)+P(B)\cdot P(D/B)+ P(C)\cdot P(D/C)$$
$$P(D)=(0.5\cdot 0.05)+(0.25\cdot0.1)+(0.25\cdot0.12)$$
$$
P(D)=0.025+0.025+0.030=0.08\to (8\%)
$$
#### Demostración
Supongamos una partición $\{ B_1,B_2,B_3,...,B_n \}$ del espacio muestral $\ohm$ y un evento $A\subset\ohm$, tal como en la figura:
![Pasted image 20260507134754.png](/img/user/Pasted%20image%2020260507134754.png)

El evento $A$ estará definido por:
$$A=A\cap B_1+A\cap B_2+A\cap B_3+...+A\cap B_n$$
Si le aplicamos la función probabilidad a ambos miembros:
$$P(A)=P(A\cap B_1)+P(A\cap B_2)+P(A\cap B_3)+...+P(A\cap B_n)$$
Ahora, si recordamos la definición de probabilidad condicional, tenemos que:
$$P(X/Y)=\frac{P(X\cap Y)}{P(Y)} \ \ \ \ \to \ \ \ \ P(X\cap Y)=P(Y)\cdot P(X/Y)$$
Por ende, si reemplazamos esta última expresión en cada probabilidad de la intersección, conseguimos demostrar:
$$P(A)=P(B_1)\cdot P(A/B_1)+P(B_2)\cdot P(A/B_2)+...+P(B_n)\cdot P(A/B_n)$$
>[!success] Demostrado

