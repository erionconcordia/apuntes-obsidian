---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/04-analisis-de-redes/01-conexiones-en-serie-y-paralelo/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #circuitos #resistencias #redes

## 1. Conexión en serie (recorrido único)
Se dice que cualquier número de elementos (resistencias, motores, etc.) están conectados en serie entre dos puntos si ofrecen un **recorrido único** para el paso de las cargas.

![Pasted image 20250911154926.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250911154926.png)

- **Corriente ($i$):** Como hay un solo camino, la intensidad i que pasa por todas las resistencias es exactamente la misma.
- **Voltaje ($V$):** La diferencia de potencial total es la suma de las caídas de potencial en cada resistencia individual ($V_{ab}​=V1​+V2​+V3$​).

A partir de la Ley de Ohm ($V=i\cdot R$), se deduce que la **resistencia equivalente** a un número cualquiera de resistencias en serie es simplemente la **suma algebraica** de dichas resistencias:
$$Req​=R1​+R2​+R3​+...$$

---
## 2. Conexión en Paralelo (Recorridos múltiples)

Se dice que los elementos están conectados en paralelo cuando todos se conectan cruzados exactamente entre los mismos dos nodos o puntos del circuito.

![Pasted image 20260502201853.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502201853.png)

- **Voltaje ($V$):** Como los bornes de todas las resistencias están conectados a los mismos dos puntos generales, la diferencia de potencial entre los bornes de cada una ha de ser exactamente la misma ($V_{ab}$​).
- **Corriente ($i$):** La corriente total que llega al nudo se divide y se reparte entre las distintas ramas ($i=i_1​+i_2​+i_3$​).

Aplicando la Ley de Ohm a la suma de las corrientes, se deduce que para un número cualquiera de resistencias en paralelo, la **inversa de la resistencia equivalente** es igual a la suma de las inversas de cada una de las resistencias individuales:
$$\frac{1}{R_{eq}}=\frac{1}{R_1}+\frac{1}{R_2}+\frac{1}{R_3}+...$$

>[!informacion] El atajo matemático para dos resistencias
>Si tenemos solamente **dos** resistencias conectadas en paralelo, podemos evitar lidiar con las fracciones usando esta fórmula simplificada directa:
>$$R_{eq}=\frac{R_1\cdot R_2}{R_1+R_2}$$

---
## 3. ¿Qué significa "equivalente"?

El método para hallar una resistencia equivalente consiste en suponer una diferencia de potencial entre los bornes de la red, calcular la corriente total que entraría, y hallar la razón de una a la otra ($R=V/i$). Físicamente, significa que si sacas toda la maraña de cables y resistencias de tu circuito y pones en su lugar una sola cajita con el valor de la $R_{eq}$​, a la batería le va a dar exactamente lo mismo: va a entregar la misma corriente total y va a sentir el mismo "esfuerzo".