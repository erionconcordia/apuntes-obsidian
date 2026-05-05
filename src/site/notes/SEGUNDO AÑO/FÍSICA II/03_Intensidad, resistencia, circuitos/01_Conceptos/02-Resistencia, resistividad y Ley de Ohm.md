---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/01-conceptos/02-resistencia-resistividad-y-ley-de-ohm/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #resistencia #ohm

>[!abstract] Resumen y relación
>Así como en la mecánica existe el rozamiento, en la electrodinámica existe una oposición al libre flujo de los electrones. Esta oposición depende intrínsecamente del material (resistividad) y de su geometría (resistencia). La famosísima Ley de Ohm relaciona esta resistencia con la corriente y el voltaje, aunque sorpresivamente, descubriremos que no es una ley universal de la naturaleza, sino un comportamiento particular de ciertos materiales. Esta última parte se relaciona bastante con temas dados en la cátedra de *ELECTROTECNIA I*, específicamente con [[SEGUNDO AÑO/ELECTROTECNIA I/01_Introducción/01_Leyes y teoremas/03-Ley de Ohm\|03-Ley de Ohm]]. 

---
## 1. Conductibilidad ($\sigma$) y Resistividad ($\rho$)
Para mantener una corriente en un conductor, necesitamos un campo eléctrico ($E$). Las sustancias difieren entre sí respecto a qué tanta densidad de corriente ($J$) permiten fluir para un mismo campo aplicado.
- **Conductibilidad ($\sigma$):** Es la razón entre la densidad de corriente y el campo eléctrico ($\sigma=J/E$). Cuanto mayor es $\sigma$, mejor conductor es el material.
- **Resistividad ($\rho$):** En la practica, es mucho más común usar la inversa de la conductibilidad, a la cual llamamos resistividad ($\rho=1/\sigma$).

Los materiales con alta resistividad son aisladores (o dieléctricos), y los de baja resistividad son buenos conductores (como la plata, el cobre o el oro).

---
## 2. Cálculo de la resistencia
Si consideramos un cable de sección transversal uniforme ($A$) y una longitud ($L$), podemos calcular su resistencia total ($R$) a partir de su resistividad mediante la siguiente fórmula:
$$R=\frac{\rho\cdot L}{A}$$
*Deducción lógica:* La resistencia al paso de la corriente es directamente proporcional a la longitud (más largo el cable, más colisiones sufren los electrones) e inversamente proporcional a la sección (un cable más grueso ofrece un "pasillo" más ancho para que los electrones fluyan, disminuyendo la resistencia).

![Pasted image 20260502191656.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502191656.png)

La resistencia se mide en Voltios por Amper ($V/A$), unidad bautizada como Ohm $(\ohm)$.

---
## 3. La Ley de Ohm
Si reemplazamos el campo y la densidad de corriente por variables macroscópicas y medibles (como la diferencia de potencial $V_{ab}$ y la intensidad $i$), llegamos a la siguiente ecuación:
$$V_{ab}=R\cdot i, \ \ \ \ \ \text{o bien} \ \ \ \ \ \ i=\frac{V_{ab}}{R}$$
>[!warning] Gran trampa
>Se suele creer que $V=I\cdot R$ es una ley absoluta del universo como la de la Gravedad, pero no es así. Para llegar a ella se supuso matemáticamente que la resistividad $\rho$ (y por ende, la resistencia $R$) era una constante.
>- **La verdadera Ley de Ohm establece que:** Para ciertas sustancias (los metales), la diferencia de potencial es una función lineal de la corriente, porque su resistencia $R$ se mantiene constante.
>- A los materiales que cumplen esto se los llama conductores lineales. Hay muchos materiales e instrumentos que no la obedecen (conductores no lineales). Es una característica particular, no una ley general de la materia.

---
## 4. El efecto de la temperatura
La resistividad de todas las sustancias conductoras varía con la temperatura. Para la mayoría de los metales, si la temperatura aumenta, la amplitud de vibración de los átomos fijos del metal también aumenta, provocando que los electrones libres choquen más veces y se frenen. Por ende, en los metales, a mayor temperatura, mayor resistencia.

La ecuación que rige esto (para variaciones no tan grandes de temperatura) es una aproximación lineal:
$$R=R_0(1+\alpha\cdot t)$$
Donde $R_0$ es la resistencia a $0°C$, $t$ es la temperatura en grados Celsius, y $\alpha$ es el "coeficiente de temperatura", medido en $°C^{-1}$.

![Pasted image 20260502192426.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502192426.png)

>[!dato] Dato curioso
>Los aisladores, semiconductores y electrolitos funcionan al revés. Su $\alpha$ es negativo, lo que significa que al calentarse se vuelven **mejores conductores**.

