---
{"dg-publish":true,"permalink":"/primer-ano/fisica-i/02-cinematica/02-conceptos/03-movimiento-rectilineo-uniformemente-variado-mruv/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

## Un cuerpo posee movimiento rectilíneo uniformemente variado cuando cumple las siguientes condiciones:

**A)** La trayectoria que recorre es una línea recta.
**B)** La velocidad cambia, permaneciendo constante el valor de la aceleración.

>[!observacion]
>1. Si la velocidad del móvil aumenta, la velocidad y la aceleración tienen el mismo sentido.
>2. Si la velocidad del móvil disminuye, la velocidad y la aceleración tienen sentidos contrarios.

## FÓRMULAS DE MRUV

#### 1. $V_f=V_i+a \cdot t$
#### 2. $a=\frac{V_f-V_i}{t}$
#### 3. $X_f=X_i+V_i \cdot t + \frac{1}{2} \cdot a \cdot t^2$
#### 4. $V_f^2=V_i^2+2 \cdot a \cdot (X_f-X_i)$

La fórmula general de **MRUV** es la expresión $(3):\ \ X_f=X_i+v_i\cdot t+\frac{1}{2}\cdot a\cdot t^2$

**¿Cómo se deduce esta fórmula?**
Primero, partiendo que la aceleración es constante, sabemos que la aceleración media va ser igual a la aceleración instantánea, por lo tanto:
$$\frac{v_f-v_i}{t_f-t_i}=\frac{dv}{dt}$$
Pero podemos relacionar $dv$ en función de la aceleración y el tiempo, teniendo en cuenta que $i$ hace referencia al inicio, por lo que $t_i=0$.
$$\to \ \ \ a=\frac{dv}{dt} \ \ \ \to \ \ \ a\cdot dt=dv$$
$$\int_0^ta\cdot dt=\int_{v_o}^{v_f}dv$$
$$a\cdot t=v_f-v_o$$
Obteniendo así, la primer fórmula de la lista:
$$v_f=v_o+a\cdot t \ \ \ (A)$$
Gráficamente lo que representa es:
![Pasted image 20250720192514.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250720192514.png)
>[!informacion]
>El área debajo la curva representa justamente el desplazamiento total $\Delta x$.

Ahora, para deducir la ecuación en función de $x-t$, sabemos que:
$$v_{med}=\frac{\Delta x}{\Delta t}=\frac{X_f-X_i}{t}$$
Como la aceleración es constante y $t_1=0$, entonces, adicionalmente la velocidad media es lo mismo que:
$$v_{med}=\frac{v_f+v_o}{2} \ \ \ (B)$$
>[!informacion]
>La fórmula $v_{med}=\frac{v_f+v_o}{2}$ sale de sumar las áreas del triángulo rectángulo y el área del rectángulo.

>[!cuidado]
>Cuando la aceleración es constante, la velocidad cambia de manera lineal. En este caso, expresado en el gráfico anterior, como la curva es una línea recta, el promedio entre $v_o$ y $v_f$ es el valor "medio" real de la velocidad durante este intervalo. Por eso es válida la ecuación anterior y, ÚNICAMENTE puede usarse en estos casos.

Habiendo obtenido las expresiones $(A)$ y $(B)$, reemplazando una en la otra obtenemos:
$$v_{med}=\frac{(v_o+a\cdot t)+v_o}{2}$$
Recordando también que $v_{med}=\frac{X_f-X_i}{t}$:
$$\frac{X_f-X_i}{t}=\frac{1}{2}\cdot(2v_o+a\cdot t)$$
$$\frac{X_f-X_i}{t}=v_o+\frac{1}{2}\cdot a\cdot t$$
$$X_f-X_i=v_o\cdot t + \frac{1}{2}\cdot a\cdot t^2$$
$$X_f=X_i+v_o\cdot t+\frac{1}{2}\cdot a\cdot t^2$$
Y así obtuvimos la principal expresión de MRUV.