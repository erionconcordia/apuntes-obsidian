---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/01-fundamentos-matematicos/02-revision-de-teoria-de-conjuntos/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #teoría_de_conjuntos #diagramas_de_venn

>[!attention] Atención: Solo es revisión.

# 1. Conjuntos = Sucesos
En la teoría de la probabilidad moderna, existe una correspondencia directa entre los "sucesos" (o eventos) de un experimento y los "conjuntos" matemáticos. Esta genialidad permite que utilicemos todas las herramientas y propiedades del álgebra de conjuntos para calcular probabilidades complejas.

Para establecer esta correspondencia, definimos dos equivalencias fundamentales:

**Suceso seguro (espacio muestral):** Matemáticamente es el conjunto universal. Los libros suelen denotarlo como $S$, pero en la cátedra de la UTN utilizamos la letra griega $\ohm$.

**Suceso imposible (conjunto vacío):** Se denota con $\emptyset$ y representa un evento que no contiene ningún resultado posible.

#### Operaciones básicas y su significado probabilístico
Cuando operamos con conjuntos, estamos combinando eventos. Aquí tenemos la traducción exacta de lo que significa cada operación matemática en la realidad física de un experimento:

- **Unión** ($A\cup B$): "Que ocurra el suceso A, el suceso B, o ambos" Es decir, que ocurra al menos uno de los dos.
- **Intersección** ($A\cap B$): "Que ocurran simultáneamente A y B".
- **Diferencia** ($A-B$): "Que ocurra A pero no B".
- **Complemento** ($A^c$ o $A'$): "Que NO ocurra A". Son todos los elementos del espacio muestral $\ohm$ que no pertenecen a $A$.
- **Intersección de complementos** ($A^c\cap B^c$): "Que no ocurra A ni B".

---
# 2. Diagramas de Venn
Las relaciones entre los eventos y su espacio muestral correspondiente se ilustran de forma gráfica utilizando los diagramas de Venn.

![Pasted image 20260423132451.png\|259](/img/user/IM%C3%81GENES/Pasted%20image%2020260423132451.png)

**Construcción**
Se traza un rectángulo cuyo interior representa todo el espacio muestral ($\ohm$ o $S$). Cualquier evento $A$ se representa como el interior de una curva cerrada (generalmente un círculo) trazada dentro del rectángulo.

**Utilidad**
Sombrear diferentes regiones de los círculos superpuestos nos permite visualizar rápidamente operaciones complejas, como identificar qué parte de una muestra sufre de un "defecto A" pero no de un "defecto B" ($A-B$).
