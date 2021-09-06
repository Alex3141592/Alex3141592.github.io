---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 02 20 Examen de Inducción
nav_order: 2021-01-18
description: "¡Primer examen parcial!"
last_modified_date: 2021-02-20T20:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Resolución de sistemas de ecuaciones por&nbsp;<span class="deg-sitio deg-sitio-texto">determinantes.</span>
{:.fs-9}

2 de marzo de 2021.
{:.fs-6 .fw-300}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

$$\begin{cases}
\frac{-5}{3}x+\frac{2}{9}y = \frac{1}{4}\\
\frac{4}{7}x+\frac{-5}{8}y = \frac{2}{3}
\end{cases}$$
{:.math}

#### Solución

$$
\begin{align*}
\Delta
&=\left|\begin{matrix} -\frac{5}{3} & \frac{2}{9} \\ \frac{4}{7}&\frac{-5}{8}\end{matrix}\right|\\[1em]
&=\left(\frac{-5}{3}\right)\left(\frac{-5}{8}\right)-\left(\frac{4}{7}\right)\left(\frac{2}{9}\right)\\[1em]
&=\frac{25}{24}-\frac{8}{63}\\[1em]
&=\frac{1575-192}{24(63)}\\[1em]
&=\frac{1383}{24(63)}\\[1em]
&=\frac{461}{8(63)}
\end{align*}
$$
{:.math}

$$
\begin{align*}
\Delta_x
&=\left|\begin{matrix} \frac{1}{4} & \frac{2}{9} \\ \frac{2}{3}&\frac{-5}{8}\end{matrix}\right|\\[1em]
&=\left(\frac{1}{4}\right)\left(\frac{-5}{8}\right)-\left(\frac{2}{3}\right)\left(\frac{2}{9}\right)\\[1em]
&=\frac{-5}{32}-\frac{4}{27}\\[1em]
&=\frac{-135-128}{32(27)}\\[1em]
&=\frac{-263}{32(27)}
\end{align*}
$$
{:.math}

$$
\begin{align*}
\Delta_y
&=\left|\begin{matrix} -\frac{5}{3} & \frac{1}{4} \\ \frac{4}{7}&\frac{2}{3}\end{matrix}\right|\\[1em]
&=\left(\frac{-5}{3}\right)\left(\frac{2}{3}\right)-\left(\frac{4}{7}\right)\left(\frac{1}{4}\right)\\[1em]
&=\frac{-10}{9}-\frac{1}{7}\\[1em]
&=\frac{-70-9}{63}\\[1em]
&=\frac{-79}{63}
\end{align*}
$$
{:.math}

Finalmente, como \\(\Delta\ne 0\\),

$$
\begin{align*}
x&=\frac{\Delta_x}{\Delta}\\[1em]
&=\frac{-263}{32(27)}\left(\frac{8(63)}{461}\right)\\[1em]
&=\frac{-263(7)}{3(4)(461)}\\[1em]
&=\frac{-1841}{5532}
\end{align*}
$$
{:.math}

$$
\begin{align*}
y&=\frac{\Delta_y}{\Delta}\\[1em]
&=\frac{-79}{63}\left(\frac{8(63)}{461}\right)\\[1em]
&=\frac{-79(8)}{461}\\[1em]
&=\frac{-632}{461}
\end{align*}
$$
{:.math}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

$$\begin{cases}
\frac{3}{5}x-\frac{6}{7}y = \frac{2}{3}\\
\frac{-9}{10}x+\frac{5}{8}y = \frac{3}{7}
\end{cases}$$
{:.math}

#### Solución

$$
\begin{align*}
\Delta
&=\left|\begin{matrix} \frac{3}{5} & \frac{-6}{7} \\ \frac{-9}{10}&\frac{5}{8}\end{matrix}\right|\\[1em]
&=\left(\frac{3}{5}\right)\left(\frac{5}{8}\right)-\left(\frac{-9}{10}\right)\left(\frac{-6}{7}\right)\\[1em]
&=\frac{3}{8}-\frac{9(3)}{5(7)}\\[1em]
&=\frac{105-216}{8(5)(7)}\\[1em]
&=\frac{-111}{8(5)(7)}
\end{align*}
$$
{:.math}

$$
\begin{align*}
\Delta_x
&=\left|\begin{matrix} \frac{2}{3} & \frac{-6}{7} \\ \frac{3}{7}&\frac{5}{8}\end{matrix}\right|\\[1em]
&=\left(\frac{2}{3}\right)\left(\frac{5}{8}\right)-\left(\frac{3}{7}\right)\left(\frac{-6}{7}\right)\\[1em]
&=\frac{2(5)}{3(8)}+\frac{18}{49}\\[1em]
&=\frac{490+432}{3(8)(49)}\\[1em]
&=\frac{245+216}{3(4)(49)}
\end{align*}
$$
{:.math}

$$
\begin{align*}
\Delta_y
&=\left|\begin{matrix} \frac{3}{5} & \frac{2}{3} \\ \frac{-9}{10}&\frac{3}{7}\end{matrix}\right|\\[1em]
&=\left(\frac{3}{5}\right)\left(\frac{3}{7}\right)-\left(\frac{-9}{10}\right)\left(\frac{2}{3}\right)\\[1em]
&=\frac{9}{5(7)}+\frac{3}{5}\\[1em]
&=\frac{9+21}{5(7)}\\[1em]
&=\frac{30}{5(7)}
\end{align*}
$$
{:.math}

Finalmente, como \\(\Delta\ne 0\\),

$$
\begin{align*}
x&=\frac{\Delta_x}{\Delta}\\[1em]
&=\frac{461}{3(4)(49)}\left(\frac{8(5)(7)}{-111}\right)\\[1em]
&=-\frac{461(10)}{3(7)(111)}\\[1em]
&=\frac{-4610}{2331}
\end{align*}
$$
{:.math}

$$
\begin{align*}
y&=\frac{\Delta_y}{\Delta}\\[1em]
&=\frac{30}{5(7)}\left(\frac{8(5)(7)}{3(37)}\right)\\[1em]
&=-\frac{10(8)}{37}\\[1em]
&=-\frac{80}{37}
\end{align*}
$$
{:.math}

$$
\begin{align*}

\left(\begin{matrix} 
\frac{1}{5} & \frac{1}{6} & 9\\ 
\frac{3}{10}&\frac{3}{7}
\end{matrix}\right)\\

\end{align*}
$$
{:.math}

