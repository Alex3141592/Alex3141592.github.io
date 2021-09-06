---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 03 20 Problema de Inducción
nav_order: 2021-01-18
description: "Inducción"
last_modified_date: 2021-03-20T18:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Problema de&nbsp;<span class="deg-sitio deg-sitio-texto">Inducción</span>
{:.fs-9}

**<span class="deg-sitio deg-sitio-texto">Alumno:</span>** Alexis Jonathan Dorantes Vázquez
{:.fs-6 .fw-300}

**<span class="deg-sitio deg-sitio-texto">Materia:</span>** Teoría de Ecuaciones
{:.fs-6 .fw-300}

**<span class="deg-sitio deg-sitio-texto">Matrícula:</span>** 202081434
{:.fs-6 .fw-300}


20 de marzo de 2021.
{:.fs-6 .fw-300}

<div> </div>
{:.salto .no-mostrar}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Dados \\(a,b\in\mathbb{R}\\) con \\(b\ne 0\\). Demostrar que

$$\left(\frac{a}{b}\right)^n=\frac{a^n}{b^n}$${:.math} 

para todo \\(n\in\mathbb{N}\\).

#### Demostración

El problema es equivalente a demostrar que:

$$\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}\land b\ne 0:\left(\frac{a}{b}\right)^n=\frac{a^n}{b^n}$${:.math} 

Dado que \\(a,b\in\mathbb{R}\land b\ne 0\\), existe el inverso multiplicativo de \\(b\\), y por el axioma de cerradura, \\(\frac{a}{b}\\) es un número real.

Por definición de las potencias naturales de un número real: 

$$\forall r\in\mathbb{R}:r^1=r\land (\forall n\in\mathbb{N}:r^{n+1}=r^n\cdot r)$${:.math}

Luego, podemos realizar lo siguiente para demostrar la hipótesis de inducción, con \\(n=1\\) (dado que la propiedad debe cumplirse para todo número natural):

$$\begin{align*}
\forall r\in\mathbb{R}:&&r^1=r&\land (\forall n\in\mathbb{N}:r^{n+1}=r^n\cdot r)\\[1em]
\forall a,b\in\mathbb{R}\land b\ne 0:&& \frac{a}{b}\in\mathbb{R}\\[1em]
\forall a,b\in\mathbb{R}\land b\ne 0:&& \frac{a}{b}\in\mathbb{R}&\implies \left(\frac{a}{b}\right)^1=\frac{a}{b}\land\frac{a}{b}=\frac{a^1}{b^1}
&&\text{Dado que }\\
&&&&&r^1=r\text{ por definición}\\[1em]

&&&\implies \left(\frac{a}{b}\right)^1=\frac{a^1}{b^1}
&&\text{Por transitividad}\\[1em]
\hline
\forall a,b\in\mathbb{R}\land b\ne 0:&&\left(\frac{a}{b}\right)^1&=\frac{a^1}{b^1}
\end{align*}$$
{:.math .fs-3}

Analicemos el caso general:

$$\begin{align*}
\forall r\in\mathbb{R}:&&r^1=r&\land (\forall n\in\mathbb{N}:r^{n+1}=r^n\cdot r)\\[1em]
\forall a,b\in\mathbb{R}\land b\ne 0:&& \frac{a}{b}\in\mathbb{R}\\[1em]
\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}\land b\ne 0:&& \left(\frac{a}{b}\right)^n=\frac{a^n}{b^n}&\implies \left(\frac{a}{b}\right)^n\cdot\frac{a}{b}=\frac{a^n}{b^n}\cdot\frac{a}{b}
&&\text{Por la propiedad de la igualdad}\\[1em]

&&&\implies  \left(\frac{a}{b}\right)^{n+1}=\frac{a^n\cdot a}{b^n\cdot b}
&&\text{Por definición de potencias}\\
&&&&&\text{y multiplicación de fracciones}\\[1em]

&&&\implies  \left(\frac{a}{b}\right)^{n+1}=\frac{a^{n+1}}{b^{n+1}}
&&\text{Por definición de potencias}\\[1em]
\hline
\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}\land b\ne 0:&&\left(\frac{a}{b}\right)^n=\frac{a^n}{b^n}&\implies \left(\frac{a}{b}\right)^{n+1}=\frac{a^{n+1}}{b^{n+1}}
\end{align*}$$
{:.math .fs-2}

Dado que se cumple la implicación, por el **Principio de Inducción Matemática**, 

$$\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}\land b\ne 0:\left(\frac{a}{b}\right)^n=\frac{a^n}{b^n}$${:.math} 

Nota: *La existencia del inverso multiplicativo de \\(b^n\\) (utilizada en la primera parte de la implicación y en la multiplicación de fracciones), se da porque \\(\forall n\in\mathbb{N}:\forall b\in\mathbb{R}\land b\ne0:b^n\ne 0\\). Para demostrarlo, basta con notar que \\(b^1=b\ne0\\) para toda \\(b\in\mathbb{R}\land b\ne0\\), por lo que la hipótesis de inducción con \\(n=1\\) es verdadera. Para el caso general:*

$$\begin{align*}
\forall r\in\mathbb{R}:&&r^1=r&\land (\forall n\in\mathbb{N}:r^{n+1}=r^n\cdot r)\\[1em]
\forall n\in\mathbb{N}:\forall b\in\mathbb{R}\land b\ne 0:&& b^n\ne 0&\implies b^n\ne0\land b\ne 0\\[1em]
&&&\iff \neg(b^n=0\lor b= 0)
&&\text{Leyes de D' Morgan}\\[1em]
&&&\iff \neg(b^n\cdot b= 0)\\[1em]
&&&\iff \neg(b^{n+1}= 0)
&&\text{Definición de potencias}\\[1em]
&&&\iff b^{n+1}\ne 0\\
\hline
\forall n\in\mathbb{N}:\forall b\in\mathbb{R}\land b\ne 0:&& b^n\ne 0&\implies b^{n+1}\ne 0
\end{align*}$$
{:.math .fs-2}

*Y por el **Principio de Inducción Matemática**, se concluye que \\(\forall n\in\mathbb{N}:\forall b\in\mathbb{R}\land b\ne0:b^n\ne 0\\).*