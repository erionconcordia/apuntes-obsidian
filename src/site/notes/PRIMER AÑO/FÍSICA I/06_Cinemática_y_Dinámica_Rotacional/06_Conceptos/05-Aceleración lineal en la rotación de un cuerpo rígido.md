---
{"dg-publish":true,"permalink":"/primer-ano/fisica-i/06-cinematica-y-dinamica-rotacional/06-conceptos/05-aceleracion-lineal-en-la-rotacion-de-un-cuerpo-rigido/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

>[!cuidado]
>Aceleración lineal y aceleración tangencial no es lo mismo. La aceleración lineal es el vector que se obtiene de componer la aceleración radial (centrípeta) con la aceleración tangencial.

![Pasted image 20250713214104.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250713214104.png)
$$\vec{a}_{lineal}=\vec{a}=\vec{a}_{tan}+\vec{a}_{cen}$$
$$||\vec{a}||=\sqrt{(a_T)^2+(a_C)^2}$$
## ¿Cómo se escribe la aceleración tangencial en un movimiento circular?
Partimos de lo siguiente, la aceleración tangencial la conocemos usualmente como $$a_{tan_{media}}=\frac{v_2-v_1}{t_2-t_1} \ \ \ \land \ \ \ a_{tan_{instantánea}}=\frac{dv}{dt}$$
Por ende, sabiendo que la velocidad tangencial es $v_{tan}=\omega\cdot R$, podemos decir lo siguiente:
$$a_{tan}=\frac{dv}{dt}$$
$$a_{tan}=\frac{d(\omega R)}{dt}$$
$$a_{tan}=R\cdot\frac{d\omega}{dt}$$
$$a_{tan}=R\cdot\alpha=\alpha\cdot R$$
## ¿Qué hay de la aceleración centrípeta?
La aceleración centrípeta es la aceleración responsable de mantener a un cuerpo en su trayectoria angular. Ésta siempre apunta hacia el centro de la curva o del círculo en el que se mueve la partícula.

**Deducción matemática de su fórmula a través del siguiente gráfico:**
![Pasted image 20250713223426.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250713223426.png)
Por el **Teorema de Tales** (similitud de triángulos), entonces obtenemos esta proporción:
$$\frac{\Delta V}{V}=\frac{\Delta S}{R}$$
$$\Delta V=\frac{V}{R} \cdot \Delta S$$
$$\frac{\Delta V}{\Delta t}=\frac{V}{R}\cdot \frac{\Delta S}{\Delta t}$$
$$\vec{a}_{cen}=\frac{V}{R}\cdot V$$
$$\vec{a}_{cen}=\frac{V^2}{R}$$
