---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/01-ley-de-coulomb-y-campo-electrico/02-campo-electrico/03-calculo-de-campo-en-distribuciones/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #campo_eléctrico #dipolo #anillo

>[!abstract] Resumen
>En el mundo real, las cargas rara vez son "puntuales". Generalmente están distribuidas a lo largo de cables, superficies o volúmenes. Para calcular su campo eléctrico, debemos dividir el cuerpo en infinitas cargas puntuales ($dq$), calcular el campo infinitesimal ($dE$) de cada una usando la Ley de Coulomb, y sumar todo mediante integrales.

---
## 1. Método de integración
Cuando no podemos usar la elegancia geométrica del *Teorema de Gauss*, recurrimos a la integración. El campo resultante en un punto $P$ se obtiene sumando vectorialmente los campos creados por cada segmento $dx$ (que contiene una carga $dq$) del objeto.
$$
dE=\frac{1}{4\pi\epsilon_0}\frac{dq}{r^2}
$$

![Pasted image 20260502134014.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502134014.png)

>[!warning] Cuidado con los vectores
>Como el campo es un vector, no se puede integrar los módulos directamente. Primero hay que descomponer $dE$ en sus componentes rectangulares ($dE_x=dE\cdot\cos(\theta)$ y $dE_y=dE\cdot\sin(\theta)$) e integrar cada eje por separado.

---
## 2. Dipolo eléctrico
Un dipolo eléctrico está formado por dos cargas iguales pero de signos opuestos ($+q$ y $-q$) separadas por una distancia $L$. Es una configuración importantísima (muchas moléculas en dieléctricos se comportan así).
![Pasted image 20260502134122.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502134122.png)

- **Momento eléctrico del dipolo ($p$):** Se define como $p=q\cdot L$.
- **Campo sobre su eje (Punto $P$ a una distancia $r$):**  $$E_p=\frac{1}{4\pi\epsilon_0}\frac{2p}{r^3}$$
  (*Para distanciar $r$ muy grandes frente a $L$*).


- **Campo sobre su plano ecuatorial (Punto $Q$):**
  $$E_Q=\frac{1}{4\pi\epsilon_0}\frac{p}{r^3}$$
  ![Pasted image 20260502134331.png\|230](/img/user/IM%C3%81GENES/Pasted%20image%2020260502134331.png)

>[!dato] Detalle fino
>Notemos que el campo de un dipolo decae rapidísimo, con el cubo de la distancia ($1/r^3$), mientras que el de una carga sola decae con el cuadrado ($1/r^2$).

---
## 3. Anillo cargado (sobre su eje)
Imaginemos un anillo de radio $a$ con una carga total $q$ distribuida uniformemente. Queremos saber el campo en un punto $P$ sobre su eje central, a una distancia $b$ de su centro. Por simetría, todas las componentes perpendiculares al eje se anulan entre sí (se compensan la de arriba con la de abajo, etc.) y solo sobreviven las componentes paralelas al eje.

![Pasted image 20260502134650.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502134650.png)

La integración da como resultado:
$$E=\frac{1}{4\pi\epsilon_0}\frac{q\cdot b}{(a^2+b^2)^{3/2}}$$
- Si evaluamos exactamente en el centro del anillo $(b=0)$, el campo es nulo $(E=0)$, lo cual tiene sentido geométrico.

---
## 4. Distribuciones de alta simetría
**1. Hilo infinito / Cilindro:**
$$E=\frac{1}{2\pi\epsilon_0}\frac{\lambda}{r}$$
Donde $\lambda$ es la densidad lineal de carga.


**2. Láminas paralelas con cargas opuestas:**
El campo exterior es despreciable y el campo interior es uniforme.
$$E=\frac{\sigma}{\epsilon_0}$$
Donde $\sigma$ es la densidad superficial de carga.

>[!informacion] Conexión
>Esta es la base matemática para armar un Capacitor.


**3. Esfera:**
Se comporta en el exterior como si toda su carga estuviera concentrada en un punto en su centro. En su interior, el campo es nulo.

---

>[!example] Ejemplos con analogías
>- **Integración vs. Gauss:** Calcular el campo dividiéndolo en infinitos pedacitos $dq$ (integración) es como analiza la telemetría de Colapinto micro-sector por micro-sector sumando las frenadas de cada metro de pista. Usar el Teorema de Gauss es como mirar directamente el tiempo de vuelta final del cronómetro: si la pista es perfectamente simétrica (como un óvalo), te dice exactamente el rendimiento del auto sin tener que calcular punto por punto.
>- **El Dipolo y el $1/r^3$:** Imaginemos dos monoplazas luchando rueda a rueda (un dipolo). Uno genera turbulencia que empuja el aire hacia afuera ($+q$) y el otro deja succión o "rebufo" que atrae el aire hacia adentro ($-q$). Vistos desde muy lejos, los efectos aerodinámicos de ambos chocan y se cancelan casi por completo mutuamente, por eso la perturbación (el campo del dipolo) "muere" rapidísimo en la distancia ($1/r^3$), mucho más rápido que si hubiera un solo auto en pista.





