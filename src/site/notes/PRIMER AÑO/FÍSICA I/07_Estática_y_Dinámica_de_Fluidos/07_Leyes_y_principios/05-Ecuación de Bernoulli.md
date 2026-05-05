---
{"dg-publish":true,"permalink":"/primer-ano/fisica-i/07-estatica-y-dinamica-de-fluidos/07-leyes-y-principios/05-ecuacion-de-bernoulli/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Según la [[PRIMER AÑO/FÍSICA I/07_Estática_y_Dinámica_de_Fluidos/07_Leyes_y_principios/04-Ecuación de continuidad\|04-Ecuación de continuidad]], la rapidez de flujo de un fluido puede variar a lo largo de las trayectorias del fluido. Podemos deducir una relación importante, llamada **ecuación de Bernoulli**, que relaciona la presión, la rapidez de flujo y la altura para el flujo de un fluido ideal.
![Pasted image 20250715172212.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250715172212.png)
Para deducir la ecuación de Bernoulli, debemos aplicar el [[PRIMER AÑO/FÍSICA I/04_Trabajo_y_Energía/04_Leyes_y_teoremas/02-Teorema trabajo-energía\|02-Teorema trabajo-energía]] al fluido de una sección de un tubo de flujo, como el de la figura de arriba. Se aplica este teorema porque Bernoulli describe cómo se transforma la energía dentro de un fluido en movimiento, cuando no hay pérdidas por fricción ni fuerzas externas adicionales.

Por ende, procederemos a armar la expresión $(1)$:
$$P=\frac{\vec{F}}{A}$$
$$\vec{F}_1=P_1\cdot A_1 \ \ \ \ \ \land \ \ \ \ \ \vec{F}_2=P_2\cdot A_2$$
$$dW=F_1\cdot ds_1-F_2\cdot ds_2$$
$$dW=P_1\cdot A_1 \cdot ds_1 - P_2\cdot A_2 \cdot ds_2$$
$$dW=P_1\cdot dV - P_2\cdot dV$$
$$dW=(P_1-P_2)dV \ \ \ (1)$$
Habiendo obtenido la primer expresión, que es el diferencial del trabajo mecánico, procedemos a armar la la expresión ($2$):
$$dV=A_1\cdot ds_1 \ \ \ \ \ \land \ \ \ \ \ dV=A_2\cdot ds_2$$
$$\frac{dm_1}{\rho}=A_1\cdot ds_1 \ \ \ \ \ \land \ \ \ \ \ \frac{dm_1}{\rho}=A_2\cdot ds_2$$
$$dm_1=\rho\cdot A_1\cdot ds_1 \ \ \ \ \ \land \ \ \ \ \ dV=\rho \cdot A_2\cdot ds_2$$
$$K_1=\frac{1}{2}\cdot m_1 \cdot v_1^2=\frac{1}{2}\cdot\rho\cdot A_1\cdot ds_1\cdot v_1^2$$
$$K_2=\frac{1}{2}\cdot m_2 \cdot v_2^2=\frac{1}{2}\cdot\rho\cdot A_2\cdot ds_2\cdot v_2^2$$
$$dK=K_2-K_1$$
$$dK=\frac{1}{2}\cdot\rho\cdot A_2\cdot ds_2\cdot v_2^2-\frac{1}{2}\cdot\rho\cdot A_1\cdot ds_1\cdot v_1^2$$
$$dK=\frac{1}{2}\cdot\rho\cdot dV\cdot v_2^2-\frac{1}{2}\cdot\rho\cdot dV\cdot v_2^2$$
$$dK=(\frac{1}{2}\cdot\rho\cdot v_2^2 - \frac{1}{2}\cdot\rho\cdot v_1^2)dV$$
$$dK=\frac{1}{2}\cdot \rho \cdot dV \cdot (v_2^2-v_1^2) \ \ \ (2)$$
Conseguimos la segunda expresión, que corresponde al diferencial de energía cinética. Procedemos a armar la última ecuación:
$$U_{g_1}=\rho\cdot dV\cdot g\cdot y_1 \ \ \ \ \ \land \ \ \ \ \ U_{g_2}=\rho\cdot dV\cdot g\cdot y_2$$
$$dU_g=\rho \cdot dV\cdot (y_2-y_1) \ \ \ (3)$$
La tercer expresión corresponde al diferencial de energía potencial gravitatoria. Por lo tanto podemos llegar a la siguiente conclusión: Como trabajo es igual a la variación de energía mecánica, o sea:
$$\text{Trabajo y energía} \to W_{otras}=\Delta E$$
Podemos escribir, con las expresiones $(1)$, $(2)$ y $(3)$, lo siguiente:
$$dW=dK+dU_g$$
$$(P_1-P_2)\cdot dV=\frac{1}{2}\cdot\rho\cdot dV\cdot(v_2^2-v_1^2)+\rho\cdot dV\cdot g\cdot (y_2-y_1)$$
$$P_1-P_2=\frac{1}{2}\cdot\rho\cdot(v_2^2-v_1^2)+\rho\cdot g\cdot (y_2-y_1)$$
$$P_1+\frac{1}{2}\rho v_1^2+\rho g y_1=P_2+\frac{1}{2} \rho v_2^2+\rho g y_2$$
De esta forma conseguimos la ecuación de Bernoulli.

>[!cuidado]
>La ecuación de Bernoulli se deduce considerando un fluido ideal y un flujo estable.

>[!informacion]
>La ecuación de Bernoulli no es otra cosa que una **conservación de la energía aplicada al flujo de un fluido ideal**.
>Decimos que la ecuación de Bernoulli **aplica el principio de conservación de la energía**, porque establece que **la energía total se conserva** mientras el fluido se mueve por una tubería o canal sin perder energía por fricción, calor u otras formas de disipación.

