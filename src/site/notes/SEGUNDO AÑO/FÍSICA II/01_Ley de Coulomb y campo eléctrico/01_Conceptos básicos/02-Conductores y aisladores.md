---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/01-ley-de-coulomb-y-campo-electrico/01-conceptos-basicos/02-conductores-y-aisladores/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electroestática #conductores #aisladores

>[!abstract] Resumen: Conductores y aisladores
>La diferencia principal entre un conductor y un aislador radica en la movilidad de sus cargas internas. Mientras que los metales poseen electrones libres que fluyen con facilidad, los aisladores tienen sus electrones fuertemente ligados al núcleo. Esta diferencia hace que, bajo la influencia de un campo eléctrico, los conductores anulen el campo en su interior (alcanzando el equilibrio electroestático), mientras que los aisladores simplemente se polarizan.

---
## 1. Modelo microscópico
Todos los átomos contienen protones (positivos) en el núcleo y electrones (negativos) orbitando. La clasificación de los materiales depende de qué tan aferrados estén esos electrones exteriores:

- **Conductores (Ej. cobre, plata, aluminio):** Los átomos de los metales liberan fácilmente uno o más de sus electrones exteriores. El núcleo positivo y el resto de los electrones quedan en posiciones fijas, pero estos electrones libres pueden moverse por todo el volumen del material sin restricciones.
  
- **Aisladores o dieléctricos (Ej. vidrio, goma, seda):** En estas sustancias casi no existen electrones libres. Las cargas están rígidamente ligadas a sus moléculas y no pueden desplazarse indefinidamente a través del material.

![Pasted image 20260501195350.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260501195350.png)

---
## 2. Compartimiento frente a un campo eléctrico exterior
¿Qué pasa si metemos estos materiales dentro de un campo eléctrico exterior?

**En un aislador (polarización)**
Como no hay cargas libres, los electrones y los núcleos solo se "desplazan" microscópicamente de sus posiciones de equilibrio, sin llegar a soltarse. Las moléculas se estiran u orientan en la dirección del campo, formando *dipolos inducidos*. A este fenómeno se lo llama **polarización**.

**En un conductor (equilibrio electrostático)**
Los electrones libres sienten la fuerza del campo y comienzan a moverse (formando una corriente transitorio). Este movimiento continúa hasta que las cargas se reacomodan de tal forma que anulan por completo el campo eléctrico exterior en el interior del conductor. Cuando las cargas dejan de moverse, se dice que el conductor está en *equilibrio electrostático*.

---
## 3. Propiedades de los conductores en equilibrio electrostático
Si las cargas en un conductor están en reposo, se cumplen cuatro condiciones estrictas y demostrables:

**1. El campo eléctrico en el interior del conductor es NULO ($E=0$)**
*¿Por qué?* Porque si $E\neq0$, las cargas libres sentirían una fuerza ($F=q\cdot E$) y se moverían. Si se mueven, no están en reposo, lo cual contradice la premisa de equilibrio. El volumen interior del conductor es un volumen equipotencial (el potencial es constante en todos sus puntos).

**2. Todo exceso de carga reside exclusivamente en su superficie exterior**
Imaginemos una superficie cerrada justo por debajo de la superficie real del conductor. Según el *Teorema de Gauss*:
$$\oint E\cdot dA=\frac{q_encerrada}{\epsilon_0}$$
Como sabemos por el punto 1 que $E=0$ en el interior, la integral da cero, y por ende $q_{encerrada}=0$. La repulsión mutua entre cargas del mismo signo hace que se alejen lo máximo posible, terminando en la frontera (superficie) del material.

**3. El campo eléctrico justo fuera de la superficie es perpendicular a la misma**
*¿Por qué?* Si el vector campo $E$ tuviera un ángulo distinto de $90°$, tendría una componente tangencial ($E_t$) y una componente normal ($E_n$). La componente $E_t$ empujaría a los electrones a lo largo de la superficie del conductor. Como estamos en equilibrio y las cargas no se mueven, forzosamente $E_t=0$, dejando solo la componente perpendicular.
![Pasted image 20260501200840.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260501200840.png)

**4. Efecto Jaula de Faraday (Apantallamiento)**
Como el campo dentro de un conductor cerrado o hueco es nulo, cualquier dispositivo colocado en su interior queda totalmente aislado de las influencias eléctricas externas.

---
>[!example] Conductores vs. Aisladores bajo un campo eléctrico
>Imaginemos que el campo eléctrico es la bandera verde que da inicio en una carrera de F1.
>- En un *conductor*, Lewis Hamilton (el electrón libre) ve la verde, acelera y tiene toda la pita para moverse a su antojo buscando su posición ideal.
>- En un *aislador*, es como si el Alpine de Franco Colapinto estuviera amarrado con lingas en el box haciendo una prueba de motor. Al ver la verde, acelera y el auto se "estira" hacia adelante tensando las lingas (esto es la polarización y los dipolos inducidos), pero por más fuerza que haga el motor, el auto está ligado a su posición y no puede salir a la pista.

