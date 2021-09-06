---
layout: default
title: 2021 03 25 Presentación de Inducción.
nav_order: 2021-03-05
description: "Página de la materia"
last_modified_date: 2021-03-05T10:00:00+0000
grand_parent: Problemas de Matemáticas Básicas
parent: Ejercicios Problemas de Matemáticas Básicas
---

# Principio del &nbsp;<span class="deg-sitio deg-sitio-texto">Buen Orden</span>
{:.fs-9}

23 de marzo de 2021.
{:.fs-6 .fw-300}


### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Para cualesquiera números naturales \\(m,n\\) tales que \\(m < n\\), existe un número natural \\(k\\) tal que \\(m+k=n\\).

#### Demostración.

Lo anterior es equivalente a:

$$\forall n\in\mathbb{N}:\forall m\in\mathbb{N}: n>m\implies \exists k\in\mathbb{N}:m+k=n$${:.math}

La hipótesis de inducción se demuestra para \\(n=m+1\\), la cual es válida, pues \\(m< n\\) y \\((m)+1=m+1=n\\) (Note que \\(1\in\mathbb{N}\\).

Analicemos el caso general para \\(n> m\\):

$$
\begin{align*}
n>m\\
\forall n\in\mathbb{N}:\forall m\in\mathbb{N}:&&\exists k\in\mathbb{N}:m+k=n&\implies \exists k\in\mathbb{N}:m+k+1=n+1\\
\forall n\in\mathbb{N}:\forall m\in\mathbb{N}:&&&\implies \exists k^\prime\in\mathbb{N}:m+k^\prime=n+1\\
\hline
\forall n\in\mathbb{N}:\forall m\in\mathbb{N}:&&\exists k\in\mathbb{N}:m+k=n&\implies \exists k^\prime\in\mathbb{N}:m+k^\prime=n+1\\
\end{align*}
$$
{:.math}

Nota: *Recuerde que si \\(k\in\mathbb{N}\\), entonces \\(k+1\in\mathbb{N}\\)*

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span> Principio del Buen Orden.

Todo conjunto \\(A\\) tal que \\(A\subset\mathbb{N}\\) y \\(A\ne \emptyset\\), tiene mínimo.

#### Demostración

Ya se había demostrado que \\(\mathbb{N}\subset\\{x\in\mathbb{R}\|x\ge 1\\}\\). Esto significa que

$$\forall x\in\mathbb{R}: x\in A\implies x\ge 1$${:.math}

Es decir, \\(1\\) es cota inferior de \\(A\\), y como \\(A\ne\emptyset\\), tiene ínfimo. 

Sea \\(I_A\\) el ínfimo de \\(A\\). Dado que toda cota inferior de \\(A\\) es menor o igual a \\(I_A\\) (por definicíon de \\(I_A\\)), \\(I_A+1\\) no es cota superior. Esto significa que existe \\(a_0\in A\\) tal que \\(I_A\le a_0< I_A+1\\).

Si \\(I_A=a_0\\), resulta que \\(I_A\in A\\), es decir, \\(I_A=\min(A)\\).

Si \\(I_A< a_0\\), \\(a_0\\) no es cota inferior de \\(A\\). Esto significa que existe \\(a_1\in A\\) tal que \\(I_A\le a_1< a_0\\). Pero dado que \\(A\subset\mathbb{N}\\), podemos utilizar el **Teorema 1** con \\(a_1\\) y \\(a_0\\), es decir, existe un número natural \\(k\\) tal que \\(a_1+k=a_0\\).

Pero

$$a_0=a_1+k\ge a_1+1\ge I_A+1$${:.math}

Lo que no es posible por el axioma de tricotomía, dado que \\(a_0< I_A+1\\).