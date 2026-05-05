---
{"dg-publish":true,"permalink":"/primer-ano/fisica-i/07-estatica-y-dinamica-de-fluidos/07-leyes-y-principios/04-ecuacion-de-continuidad/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

**La masa de un fluido en movimiento no cambia al fluir**. Esto conduce a una relación cuantitativa importante llamada **ecuación de continuidad**.

>[!informacion]
>Que algo sea **cuantitativo** se refiere a la capacidad de medir o expresar algo en términos numéricos. Se relaciona con la cantidad, el tamaño, la magnitud o la frecuencia de un fenómeno o variable.

![Pasted image 20250715163855.png](/img/user/IM%C3%81GENES/Pasted%20image%2020250715163855.png)

**Deducción de la ecuación de continuidad**
Consideramos **siempre** un [[PRIMER AÑO/FÍSICA I/07_Estática_y_Dinámica_de_Fluidos/07_Conceptos/01-Fluído ideal\|01-Fluído ideal]], entonces:
$$v_1=\frac{dx_1}{dt} \ \ \ \ \ \ \ \ \ \ \land \ \ \ \ \ \ \ \ \ \ v_2=\frac{dx_2}{dt}$$
$$(1) \ \ \ dx_1=v_1dt \ \ \ \ \ \ \ \ \ \ \land \ \ \ \ \ \ \ \ \ \ dx_2=v_2dt \ \ \ (2)$$
Teniendo las expresiones $(1)$ y $(2)$, procedemos a relacionarlas con la fórmula del volumen:
$$dV_1=A_1\cdot dx_1 \ \ \ \ \ \ \ \ \ \ \land \ \ \ \ \ \ \ \ \ \ dV_2=A_2\cdot dx_2$$
$$dV_1=A_1\cdot(v_1\cdot dt) \ \ \ \ \ \ \ \ \ \ \land \ \ \ \ \ \ \ \ \ \ dV_2=A_2\cdot(v_2\cdot dt)$$
$$\frac{dm_1}{\rho_1}=A_1\cdot(v_1\cdot dt) \ \ \ \ \ \ \ \ \ \ \land \ \ \ \ \ \ \ \ \ \ \frac{dm_2}{\rho_2}=A_2\cdot(v_2\cdot dt)$$
$$dm_1=\rho_1\cdot A_1\cdot v_1\cdot dt \ \ \ \ \ \ \ \ \ \ \land \ \ \ \ \ \ \ \ \ \ dm_2=\rho_2\cdot A_2\cdot v_2\cdot dt$$
Como el flujo es constante y no hay acumulación ni pérdidas de masa dentro del volumen de control, **la masa que entra tiene que ser igual a la masa que sale**, por lo tanto podemos igualar las expresiones y obtener:
$$\rho_1 \cdot A_1\cdot v_1\cdot dt=\rho_2\cdot A_2\cdot v_2\cdot dt$$
$$A_1\cdot v_1=A_2\cdot v_2 \ \ \ \ \text{(ecuación de continuidad)}$$

Entonces:
- $A\cdot v=\text{Área}\cdot \text{Velocidad}$
- $A\cdot v = Q = Caudal = \text{Flujo de volumen}$
- $[\frac{m^3}{s}]=[\frac{volumen}{tiempo}]$
