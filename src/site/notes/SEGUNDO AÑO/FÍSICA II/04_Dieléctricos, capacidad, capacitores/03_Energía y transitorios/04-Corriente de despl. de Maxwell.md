---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/04-dielectricos-capacidad-capacitores/03-energia-y-transitorios/04-corriente-de-despl-de-maxwell/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #maxwell #electromagnetismo #capacitores 

## 1. Circuito "abierto"
Tradicionalmente, definimos la corriente como un flujo de carga y establecemos que su intensidad debe ser la misma en todas las secciones transversales de un circuito en serie. Sin embargo, si el circuito incluye un condensador, el dieléctrico entre sus láminas es un aislador.

Esto significa que:
- En los cables, hay una corriente de conducción ($i$) real.
- En el espacio entre las placas, la corriente de conducción es estrictamente nula porque no puede saltar electrones a través del aislante.
Como resultado de la corriente, los electrones entran en una armadura y obligan a otros a salir de la armadura opuesta, pero nada cruza físicamente el medio.

## 2. Definición matemática
Para resolver esta inconsistencia y poder decir que la corriente es la misma en todo el circuito (incluyendo el dieléctrico), Maxwell generalizó la definición.

Si representamos por $q$ la carga del condensador en un instante dado, la corriente en los cables es $i=dq/dt$. Sabemos que el desplazamiento eléctrico ($D$) en el dieléctrico es igual a la densidad de carga de las placas ($D=q/A$), por lo que la carga se puede expresar como $q=D\cdot A$.

Sustituyendo esto en la derivada, Maxwell propuso denominar corriente de desplazamiento ($i_D$) a la expresión:
$$i_D=A\cdot\frac{dD}{dt}$$
Donde:
- $A$ es el área de las armaduras del capacitor.
- $dD/dt$ es la rapidez con la que cambia el desplazamiento (y por ende campo eléctrico) en el tiempo.

---
## 3. Interpretación física
La corriente de desplazamiento tiene las mismas dimensiones que la corriente de conducción. Gracias a este concepto, podemos afirmar que la corriente es la misma en todas las secciones del circuito, incluidas las que cortan el dieléctrico.

Físicamente, esto implica que un campo eléctrico que cambia con el tiempo ($dD/dt$) produce los mismos efectos magnéticos que una corriente eléctrica real circulando por un cable. Así, todos los circuitos pueden considerarse como "cerrados" aunque una parte de ellos sea un aislador.
