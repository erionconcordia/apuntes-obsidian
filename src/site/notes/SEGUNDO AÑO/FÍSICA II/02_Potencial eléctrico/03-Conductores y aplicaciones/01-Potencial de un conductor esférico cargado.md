---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/03-conductores-y-aplicaciones/01-potencial-de-un-conductor-esferico-cargado/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #conductores #esfera

## 1. Comportamiento en puntos exteriores e interiores
Supongamos un conductor esférico de radio $a$ que posee una carga $q$.
- **En los puntos exteriores ($r\geq a$):** El campo eléctrico fuera del conductor es idéntico al de una carga puntual. Por lo tanto, la fórmula del potencial a una distancia $r$ es la misma que la de una carga puntual:
$$V=\frac{1}{4\pi\epsilon_0}\frac{q}{r}$$
- **En los puntos interiores ($r<a$):** Sabemos que en el interior de un conductor en equilibrio electrostático, la intensidad del campo eléctrico es estrictamente nula ($E=0$). Si derivamos de la relación del gradiente de potencial ($E=-dV/dr$), que la derivada sea cero significa que la función original es una constante. Por lo tanto, el potencial es el mismo en todos los puntos interiores e igual al potencial exacto en la superficie de la esfera:
$$V=\frac{1}{4\phi\epsilon_0}\frac{q}{a}=cte$$

---
## 2. Representación gráfica

![Pasted image 20260502172850.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502172850.png)

De la gráfica se reduce que en un punto exterior infinitamente próximo a la superficie, el campo eléctrico $E$ es máximo y el potencial comienza su curva de descenso. A medida que nos alejamos, el voltaje disminuye proporcionalmente a $1/r$, mientras que el "empujón" del campo decae mucho más rápido, proporcional a $1/r^2$.

---
## 3. Rigidez dieléctrica y las puntas
El aire tiene un límite de "aguante" antes de ionizarse y volverse conductor (rigidez dieléctrica, alrededor de $3*10^6V/m$). Como el campo máximo en la superficie es $E_m$, el potencial máximo ($V_m$) que puede alcanzar la esfera sin descargar chispas al aire es:
$$V_m=E_m\cdot a$$
Esto significa que el *potencial máximo es directamente proporcional al radio de la esfera*.

>[!example] Ejemplo real
>Una pequeña esfera de $1\ cm$ de radio ($0.01\ m$) sólo puede cargarse hasta un potencial de $30.000\ V$ antes de emitir chispas al aire.

