---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/01-ley-de-coulomb-y-campo-electrico/03-leyes-y-teoremas/02-teorema-de-gauss/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electroestática #leyes #teorema_de_gauss #flujo #flujo_eléctrico

>[!abstract] Resumen: Teorema de Gauss
>Es una ley fundamental que relaciona la cantidad de campo eléctrico que atraviesa una superficie cerrada con la carga neta que se encuentra en su interior. Mientras que la Ley de Coulomb calcula fuerzas interaccionando punto por punto, el Teorema de Gauss usa la geometría y la asimetría para resolver problemas complejos de una forma mucho más directa y global.

---
## 1. Las líneas de fuerza y el flujo
Para representar los campos eléctricos, *Michael Faraday* introdujo el concepto de líneas de fuerza. Estas son líneas imaginarias trazadas de modo que su dirección en cada punto coincida con la dirección del campo eléctrico en ese punto.

La intensidad de un campo eléctrico puede visualizarse según qué tan "apretadas" estén estas líneas. Matemáticamente, el número total de líneas de fuerza $(N)$ que atraviesan una superficie (lo que comúnmente llamamos "flujo") se calcula integrando la componente normal del campo sobre toda el área.
$$
N=\int\epsilon_0\cdot E\cdot \cos(\theta)\cdot dA
$$
Donde $\theta$ es el ángulo entre el campo eléctrico $E$ y la recta normal (perpendicular) al elemento de área $dA$. 

*Nota:* En la práctica nos solemos referir a $N$ como $\Phi$ (flujo eléctrico)

---
## 2. Enunciado del Teorema de Gauss
Si imaginamos una superficie cerrada de cualquier forma (a la que llamaremos "superficie gaussiana"), el teorema establece:

>[!definicion] Teorema de Gauss
>El número neto de líneas de fuerza que cruzan una superficie cerrada hacia afuera es exactamente igual a la carga neta positiva encerrada dentro de dicha superficie, independientemente de cómo estén distribuidas las cargas en su interior.
>
>La expresión matemática, extendiendo la integral a toda la superficie cerrada, es:
>$$\oint\epsilon_0\cdot E\cdot\cos(\theta)\cdot dA=q$$

En la expresión matemática, $q$ es la carga neta positiva encerrada. Si no hay carga en el interior, el número neto de líneas que la atraviesan es cero (las líneas que entran son iguales a las que salen).

---
## 3. Aplicaciones y demostraciones
La verdadera magia del Teorema de Gauss aparece cuando lo aplicamos a cuerpos con formas geométricas muy simétricas (esferas, cilindros, planos).

**Ejemplo demostrativo:** Campo de un hilo conductor infinitamente largo
Si quisiéramos calcular el campo de un cable largo con carga uniforme usando Coulomb, tendríamos que hacer un integración compleja sumando el aporte de infinitos puntos. Con Gauss, es casi instantáneo:

1. Imaginemos una superficie gaussiana en forma de cilindro (de radio $r$ y largo $b$) concéntrico al cable.
2. Por simetría, el campo $E$ es constante en toda la superficie curva del cilindro y paralelo a su normal $(\cos(0°)=1)$. Las tapas planas no son atravesadas por líneas de fuerza.
3. La carga encerrada es $q=\lambda\cdot b$ (donde $\lambda$ es la carga por unidad de longitud).
4. Aplicamos Gauss:
$$\epsilon_0\cdot E\cdot(2\pi\cdot r\cdot b)=\lambda\cdot b$$
   Despejando $E$, obtenemos la intensidad del campo:
   $$E=\frac{1}{2\pi\epsilon_0}\cdot\frac{\lambda}{r}$$
   Y así, el campo eléctrico decae inversamente proporcional a la distancia $r$ del cable.


