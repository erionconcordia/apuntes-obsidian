---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/02-relaciones-matematicas/02-gradiente-de-potencial/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #campo_eléctrico #gradiente #derivadas

## 1. El gradiente en una dirección arbitraria
Partamos de la fórmula diferencial de la diferencia de potencial:
$$dV=-E\cdot\cos(\phi)\cdot ds$$
Si despejamos matemáticamente, obtenemos:
$$E\cdot\cos(\phi)=-\frac{dV}{ds}$$
>[!important] Importante
>La razón $\frac{dV}{ds}$, es decir, la derivada del potencial respecto a la distancia en una dirección determinada, se denomina gradiente de potencial. Como el término $E\cdot\cos(\phi)$ es la componente del campo eléctrico en la dirección de $ds$, concluimos que: La componente de la intensidad del campo eléctrico en una dirección cualquiera es igual al gradiente de potencial en dicha dirección, cambiado de signo.

Si nos movemos exactamente en la misma dirección que apunta el campo eléctrico ($\phi=0°$, por lo que $\cos(0°)=1$), la ecuación se reduce a:
$$E=-\frac{dV}{ds}$$
El signo negativo nos recuerda que el **campo eléctrico siempre apunta hacia donde el potencial disminuye**.

>[!informacion] Equivalencia de unidades
>Al ver que $E=dV/ds$, nos damos cuenta de que las unidades del campo eléctrico también pueden expresarse como Voltios por metro ($V/m$). Esta unidad es exactamente equivalente a ($N/C$). De hecho, en la práctica de la ingeniería es mucho más común usar $V/m$, o incluso $V/cm$ o $V/mm$.

---
## 2. Expresión tridimensional (Derivadas parciales)
En el mundo real, el campo que rodea a las cargas es tridimensional, por lo que el potencial $V$ es una función de las coordenadas espaciales ($x,y,z$). Para encontrar el vector campo eléctrico completo $E$, aplicamos el gradiente en cada uno de los tres ejes cartesianos usando derivadas parciales:
$$E_x=-\frac{\partial V}{\partial x}, \ \ \ \ \ \ E_y=-\frac{\partial V}{\partial y}, \ \ \ \ \ \ E_z=-\frac{\partial V}{\partial z}$$
El vector campo eléctrico resultante se arma sumando vectorialmente estas tres componentes:
$$E=E_xi+E_yj+E_zk$$
![Pasted image 20260502165748.png\|380](/img/user/IM%C3%81GENES/Pasted%20image%2020260502165748.png)

---
## 3. Zonas equipotenciales y atajo matemático
**1. El campo interior de los conductores**
*¿Qué pasa si en una región del espacio el potencial es exactamente el mismo en todos los puntos ($V=cte$)?* Si el voltaje no cambia, sus derivadas parciales son nulas. Por lo tanto, las tres componentes de $E$ son cero. Esto demuestra matemáticamente lo que ya sabíamos: como dentro de un conductor en equilibrio el campo es nulo, todo su volumen interior es, obligatoriamente, una región equipotencial.

**2. El "atajo"**
Una de las mayores utilidades del gradiente es que nos ahorra muchísimo tiempo en los cálculos. Es muchísimo más sencillo calcular primero la expresión del potencial $V$ en un punto (ya que es una suma escalar y algebraica de las cargas) y luego derivar esa función espacial para obtener el vector Campo Eléctrico ($E$), que intentar calcular $E$ directamente sumando vectores complicados con la Ley de Coulomb.
