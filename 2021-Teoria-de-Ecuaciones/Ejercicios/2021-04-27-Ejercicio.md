---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 04 22 Números complejos
nav_order: 2021-01-18
description: "Inducción"
last_modified_date: 2021-03-20T18:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Problemas de&nbsp;<span class="deg-sitio deg-sitio-texto">\\(\mathbb{C}\\)</span>
{:.fs-9}


### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">10</span>

>**a.** Si \\(w^3=1\\) y \\(w\ne 1\\), entonces \\(w^2+w+1=0\\)
>
>**b.** Encuentre todas las soluciones de la ecuación \\(w^3=1\\)

#### Solución 

Para la parte **a.**

$$\begin{align*}
w^3=1\land w\ne 1&\implies w^3-1=0 \land w\ne 1\\
&\implies \left(w-1\right)\left(w^2+w+1\right)=0\land w\ne 1\\
&\implies \left(w-1=0\lor w^2+w+1=0\right)\land w\ne 1\\
&\implies \left(w=1\lor w^2+w+1=0\right)\land w\ne 1\\
&\implies \left(w=1\land w\ne 1\right)\lor \left(w^2+w+1=0\land w\ne 1\right)\\
&\implies w^2+w+1=0\land w\ne 1\\
&\implies w^2+w+1=0\\
\hline
w^3=1\land w\ne 1&\implies w^2+w+1=0
\end{align*}
$${:.math}

Para la parte **b.**, utilizaremos la siguiente propiedad.

> Sea \\(r\in\mathbb{R}\\). \\(r^3=1\iff r=1\\).

Entonces, sea \\(w=\left(a,b\right)\\):

$$\begin{align*}
w^3=1&\implies |w^3|=|1|\\
&\implies |ww^2|=1\\
&\implies |w|\:|w^2|=1\\
&\implies |w|\:|ww|=1\\
&\implies |w|\:|w|\:|w|=1\\
&\implies |w|^3=1\\
&\implies |w|=1\\
\hline
w^3=1&\implies|w|=1
\end{align*}
$${:.math}

Si \\(w^3=1\\), entonces \\(ww^2=1\\), es decir, \\(w^2\\) es el inverso multiplicativo de \\(w\\). Como el inverso multiplicativo es único, se cumple que:

$$\begin{align*}
w^3=1&\implies|w|=1\\
w^3=1&\implies w^2=w^{-1}\\
&\implies w^2=|w|^{-1}\bar w\\
&\implies w^2=1^{-1} \bar w\\
&\implies w^2= \bar w\\
&\implies \left(a,b\right)^2=\left(a,-b\right)\\
&\implies \left(a^2-b^2,2ab\right)= \left(a,-b\right)\\
&\implies a^2-b^2=a \land 2ab=-b\\
&\implies a^2-b^2=a \land 2ab=-b\\
&\implies a^2-b^2=a \land \left(2a+1\right)b=0\\
&\implies a^2-b^2=a \land \left(2a+1=0\lor b=0\right)\\
&\implies \left(a^2-b^2=a \land 2a+1=0\right)\lor \left(a^2-b^2=a\land b=0\right)\\
&\implies \left(a^2-b^2=a \land a=-\frac{1}{2}\right)\lor \left(a^2=a\land b=0\right)\\
&\implies \left(a^2-b^2=a \land a=-\frac{1}{2}\right)\lor \left(a\left(a-1\right)=0\land b=0\right)\\
&\implies \left(b^2=\frac{3}{4} \land a=-\frac{1}{2}\right)\lor \left(\left(a=0\lor a-1=0\right)\land b=0\right)\\
&\implies \left(\left(b=\frac{\sqrt{3}}{2}\lor b=-\frac{\sqrt{3}}{2}\right) \land a=-\frac{1}{2}\right)\lor \left(\left(a=0\land b=0\right)\lor\left(a-1=0\land b=0\right)\right)\\
&\implies \left(\left(b=\frac{\sqrt{3}}{2}\land a=-\frac{1}{2}\right)\lor\left(b=-\frac{\sqrt{3}}{2}\land a=-\frac{1}{2}\right)\right)\lor \left(\left(a=0\land b=0\right)\lor\left(a=1\land b=0\right)\right)\\
&\implies w=\left(-\frac{1}{2},\frac{\sqrt{3}}{2}\right)\lor w=\left(-\frac{1}{2},-\frac{\sqrt{3}}{2}\right)\lor w=\left(0,0\right)\lor w=\left(1,0\right)\\
\hline
w^3=1&\implies w=\left(-\frac{1}{2},\frac{\sqrt{3}}{2}\right)\lor w=\left(-\frac{1}{2},-\frac{\sqrt{3}}{2}\right)\lor w=\left(1,0\right)\\
\end{align*}
$${:.math}