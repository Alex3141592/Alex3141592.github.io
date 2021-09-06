---
layout: default
title: 2021 01 21 Producto de tangentes de rectas y perpendiculares.
nav_order: 2021-01-18
description: "Página de la materia"
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Geometría Analítica
parent: Ejercicios Geometría Analítica
---

# Demostración producto de tangentes igual a -1 implica&nbsp;<span class="deg-sitio deg-sitio-texto">perpendicularidad.</span>
{:.fs-9}

25 de enero de 2021.
{:.fs-6 .fw-300}

Sean \\(\ell_1\\) y \\(\ell_2\\) dos rectas del plano no perpendiculares a los ejes. Sean \\(P_1=(x_1,y_1)=\ell_1\cap\ell_2\\), \\(P_2=(x_2,y_2)\in\ell_1\\) y \\(P_3=(x_2,y_3)\in\ell_2\\) tres puntos distintos. Dado que sus tangentes \\(m_1\\) y \\(m_2\\), respectivamente, cumplen que \\(m_1m_2=-1\\), y \\(-1\ne 0\\), se tiene que \\(m_1\ne 0 \land m_2\ne 0\\). De esto también se concluye, dado que \\(m_1=\frac{y_2-y_1}{x_2-x_1}\\) y \\(m_2=\frac{y_3-y_1}{x_2-x_1}\\), que los números \\(y_2-y_1\\), \\(y_3-y_1\\) y \\(x_2-x_1\\) son distintos de cero.

A través del siguiente razonamiento se demuestra que \\(m_1m_2=-1\implies\\) \\((y_1-y_3)(y_2-y_1)=(x_2-x_1)^2\\)

$$
\begin{align*}
m_1m_2=-1&\implies \frac{y_2-y_1}{x_2-x_1}\cdot\frac{y_3-y_1}{x_2-x_1}=-1\\

&\implies \frac{(y_2-y_1)(y_3-y_1)}{(x_2-x_1)^2}=-1\\

&\implies \frac{(y_3-y_1)(y_2-y_1)}{(x_2-x_1)^2}=-1\\

&\implies \frac{(y_3-y_1)(y_2-y_1)}{(x_2-x_1)^2}(x_2-x_1)^2=-(x_2-x_1)^2\\

&\implies (y_3-y_1)(y_2-y_1)=-1(x_2-x_1)^2\\

&\implies (y_3-y_1)(y_2-y_1)(-1)=-1(x_2-x_1)^2(-1)\\

&\implies (y_3-y_1)(-1)(y_2-y_1)=-1(-1)(x_2-x_1)^2\\

&\implies (y_1-y_3)(y_2-y_1)=1(x_2-x_1)^2\\

&\implies (y_1-y_3)(y_2-y_1)=(x_2-x_1)^2\\

\hline
m_1m_2=-1&\implies (y_1-y_3)(y_2-y_1)=(x_2-x_1)^2
\end{align*}
$$
{:.math}

Entonces, con el siguiente razonamiento:

$$
\begin{align*}
m_1m_2=-1&\implies \frac{y_2-y_1}{x_2-x_1}\cdot\frac{y_3-y_1}{x_2-x_1}=-1\\

&\implies \frac{(y_2-y_1)(y_3-y_1)}{(x_2-x_1)^2}=-1\\

&\implies \frac{(y_3-y_1)(y_2-y_1)}{(x_2-x_1)^2}=-1\\

&\implies \frac{(y_3-y_1)(y_2-y_1)}{(x_2-x_1)^2}(x_2-x_1)^2=-(x_2-x_1)^2\\

&\implies (y_3-y_1)(y_2-y_1)=-1\cdot(x_2-x_1)^2\\

&\implies  (y_3-y_1)(y_2-y_1)-(y_2-y_1)^2=-(x_2-x_1)^2-(y_2-y_1)^2\\

&\implies (y_3-y_1)(y_2-y_1)-(y_2-y_1)^2=-|P_1P_2|^2\\

&\implies -(y_2-y_1)^2+(y_3-y_1)(y_2-y_1)=-|P_1P_2|^2\\

&\implies -(y_2-y_1)^2-(y_1-y_3)(y_2-y_1)=-|P_1P_2|^2\\

&\implies -(y_2-y_1)^2-(y_1-y_3)(y_2-y_1)-(y_1-y_3)(y_2-y_1)+(y_1-y_3)\\
&\phantom{\implies =}\,(y_2-y_1)-(y_1-y_3)^2+(y_1-y_3)^2\\
&\phantom{\implies}=-|P_1P_2|^2-(y_1-y_3)(y_2-y_1)+(y_1-y_3)(y_2-y_1)\\
&\phantom{\implies =}-(y_1-y_3)^2+(y_1-y_3)^2\\

&\implies -(y_2-y_1)^2-2(y_1-y_3)(y_2-y_1)+(y_1-y_3)(y_2-y_1)\\
&\phantom{\implies =}-(y_1-y_3)^2+(y_1-y_3)^2\\
&\phantom{\implies}=-|P_1P_2|^2+0+0\\

&\implies -(y_2-y_1)^2-2(y_1-y_3)(y_2-y_1)-(y_1-y_3)^2\\
&\phantom{\implies =}+(y_1-y_3)(y_2-y_1)+(y_1-y_3)^2\\
&\phantom{\implies}=-|P_1P_2|^2\\

&\implies -((y_2-y_1)^2+2(y_1-y_3)(y_2-y_1)+(y_1-y_3)^2)\\
&\phantom{\implies =}+(y_1-y_3)(y_2-y_1)+(y_1-y_3)^2\\
&\phantom{\implies}=-|P_1P_2|^2\\

&\implies -(y_2-y_3)^2 +(y_1-y_3)(y_2-y_1)+(y_1-y_3)^2\\
&\phantom{\implies}=-|P_1P_2|^2\\

&\implies -|P_2P_3|^2+(y_1-y_3)(y_2-y_1)+(y_1-y_3)^2=-|P_1P_2|^2\\

&\implies -|P_2P_3|^2+(x_2-x_1)^2+(y_1-y_3)^2=-|P_1P_2|^2\\

&\implies -|P_2P_3|^2+(x_2-x_1)^2+(y_3-y_1)^2=-|P_1P_2|^2\\

&\implies -|P_2P_3|^2+|P_1P_3|^2=-|P_1P_2|^2\\

&\implies |P_1P_3|^2-|P_2P_3|^2=-|P_1P_2|^2\\

&\implies |P_1P_3|^2-|P_2P_3|^2+|P_2P_3|^2+|P_1P_2|^2=-|P_1P_2|^2+|P_1P_2|^2+|P_2P_3|^2\\

&\implies |P_1P_3|^2+0+|P_1P_2|^2=0+|P_2P_3|^2\\

&\implies |P_1P_3|^2+|P_1P_2|^2=|P_2P_3|^2\\

&\implies P_1P_2\perp P_1P_3\\

&\implies \ell_1\perp \ell_2\\

\hline

m_1m_2=-1&\implies \ell_1\perp \ell_2
\end{align*}
$$
{:.math}

Queda demostrado que, si dos rectas tienen tangentes \\(m_1\\) y \\(m_2\\) tales que \\(m_1m_2=-1\\), son perpendiculares. Nótese que la penúltima implicación es el recíproco del Teorema de pitágoras.

Dudas: ¿Es posible cambiar la implicación por doble implicación?


