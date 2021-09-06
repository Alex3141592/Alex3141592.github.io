---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 05 14 Polinomios
nav_order: 2021-04-30
description: "Polinomios"
last_modified_date: 2021-04-30T18:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Ejercicios&nbsp;<span class="deg-sitio deg-sitio-texto">Polinomios</span>
{:.fs-9}

Álgebra superior, Cárdenas, p. 287.

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

¿Cuáles son las raíces del polinomio \\(x^4-1\\)?

#### Solución 

Sea \\(f(x)=x^4-1\\). \\(a\\) es raíz de \\(f\\) sí y sólo sí \\(f(a)=0\\). Vemos que

$$\begin{align*}
f(a)=0&\implies a^4-1=0\\
&\implies (a^2+1)(a^2-1)=0\\
&\implies a^2+1=0\lor a^2-1=0\\
&\implies a^2-(-1)=0\lor (a+1)(a-1)=0\\
&\implies a^2-i^2=0\lor (a+1=0\lor a-1=0)\\
&\implies (a+i=0\lor a-i=0)\lor (a+1=0\lor a-1=0)\\
&\implies a+i=0\lor a-i=0\lor a+1=0\lor a-1=0\\
&\implies a=-i\lor a=i\lor a=-1\lor a=1\\
\hline
f(a)=0&\implies a=-i\lor a=i\lor a=-1\lor a=1
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

Exprésese \\(x^3-1\\) como producto de polinomios de grado 1.

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

Resuélvase la ecuación \\(x^3-1=0\\).
#### Solución 

Basta con encontrar las raíces de \\(f(x)=x^3-1\\), ya que \\(a\\) es raíz de \\(f\\) sí y sólo sí \\(x-a\|f(x)\\) sí y sólo sí existe \\(h(x)\\) tal que \\(f(x)=(x-a)h(x)\\). Es decir, el polinomio de grado 1 \\(x-a\\) es un factor de \\(f\\) sí y sólo sí \\(a\\) es raíz de \\(f\\).

$$\begin{align*}
f(a)=0&\implies a^3-1=0\\
&\implies (a-1)(a^2+a+1)=0\\
&\implies a-1=0\lor a^2+a+1=0\\
&\implies a=1\lor \left(a=\frac{-1+\sqrt{1-4(1)(1)}}{2(1)}\lor a=\frac{-1-\sqrt{1-4(1)(1)}}{2(1)}\right)\\
&\implies a=1\lor a=-\frac{1}{2}+\frac{\sqrt{3}}{2}i\lor a=-\frac{1}{2}-\frac{\sqrt{3}}{2}i\\
\hline
f(a)=0&\implies a=1\lor a=-\frac{1}{2}+\frac{\sqrt{3}}{2}i\lor a=-\frac{1}{2}-\frac{\sqrt{3}}{2}i
\end{align*}
$${:.math}

Finalmente, vemos que \\(f(x)=(x-1)\left(x+\frac{1}{2}-\frac{\sqrt{3}}{2}i\right)\left(x+\frac{1}{2}+\frac{\sqrt{3}}{2}i\right)\\), que es lo requerido.

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">4</span>

¿Cuáles son los polinomios que no tienen ninguna raíz?

#### Solución

El teorema "todo polinomio de grado mayor a 0 tiene al menos una raíz compleja" nos indica que el polinomio \\(f\\) que no tiene raíces tiene grado 0.

Luego \\(f(x)=a_0\\) para algún complejo \\(a_0\\). \\(a_0=0\\) implica \\(f(x)=0\\) para todo complejo \\(x\\), entonces cualquier número complejo es una raíz de \\(f\\), lo cual es una contradicción, pues \\(f\\) no tiene raíces.

Veamos que todo polinomio de la forma \\(f(x)=a_0\\) con \\(a_0\ne 0\\) no tiene raíces. Basta verificar que \\(f(a)=a_0\ne 0\\) para todo complejo \\(a\\).

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">5</span>

Dése un polinomio que tenga una infinidad de raíces.

#### Solución

\\(f(x)=0\\).