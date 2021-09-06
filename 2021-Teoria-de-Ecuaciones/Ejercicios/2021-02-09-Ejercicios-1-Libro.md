---
layout: default
title: 2021 02 09 Ejercicios 1. Libro de álgebra.
nav_order: 2021-01-18
description: "Los ejercicios de la sección de inducción del libro."
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Demostraciones de los Ejercicios de Inducción Matemática del libro de&nbsp;<span class="deg-sitio deg-sitio-texto">Álgebra</span>
{:.fs-9}

29 de enero de 2021.
{:.fs-6 .fw-300}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

Demuestre que \\(\forall n\in\mathbb{N}:a>1\implies a^n>1\\).

#### Demostración
Sea \\(p(n)\equiv a^n>1\\).
Cuando \\(a\le 1\\), \\(\forall n\in\mathbb{N}:a>1\implies a^n>1\\) es verdadera \\(\forall n\in\mathbb{N}\\). Luego, sólo falta demostrar que \\(p(n)\\) es verdadera para todo número natural \\(n\\), asumiendo que \\(a>1\\). 

En tal caso, \\(1>0\\) y por transitividad \\(a>0\\).

$$
\begin{align*}
a>1&\implies a^1=a\land a>1 \\
&\implies a^1>1\\
\hline
p(1)
\end{align*}
$$
{:.math}

Para finalizar:

$$
\begin{align*}
p(n)&\iff a^n>1\\
&\implies a^n\cdot a>1\cdot a \land a>1\\
&\implies a^{n+1}> a \land a>1\\
&\iff p(n+1)\\
\hline
p(n)&\implies p(n+1)
\end{align*}
$$
{:.math}

Concluimos que \\(\forall n\in\mathbb{N}:a>1\implies a^n>1\\).

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Demuestre que \\(\forall n\in\mathbb{N}: n<2^n\\).

#### Demostración

Por el **Problema [2](#problema2)**, se tiene que:

$$
\begin{align*}
\forall n\in\mathbb{N}:&\: a>1\implies a^n>1 \\
&2>1\\
\hline
2^n>1
\end{align*}
$$
{:.math}

Ahora, sea \\(p(n)\equiv n<2^n\\). Vemos que 

$$
\begin{align*}
2^1=2\\
2>1\\
\hline
p(1)
\end{align*}
$$
{:.math}

Por lo tanto, \\(p(1)\\) es verdadera.

$$
\begin{align*}
\forall n\in\mathbb{N}:&&p(n)&\iff n<2^n\\
\forall n\in\mathbb{N}:&&n<2^n&\implies n+1<2^n+2^n\\
\forall n\in\mathbb{N}:&&n+1<2^n+2^n&\implies n+1<2(2^n)\\
\forall n\in\mathbb{N}:&&n+1<2(2^n)&\implies n+1<2^{n+1}\\
\forall n\in\mathbb{N}:&&n+1<2^{n+1}&\iff p(n+1)\\
\hline
\forall n\in\mathbb{N}:&&p(n)&\implies p(n+1)
\end{align*}
$$
{:.math}

Por lo tanto, \\(\forall n\in\mathbb{N}:n<2^n\\).

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">6</span>

Demuestre que \\(\forall n\in\mathbb{N}: 3^n\ge 1+2^n\\).

#### Demostración

Sea \\(p(n)\equiv 3^n\ge 1+2^n\\)

Por el **Problema [2](#problema2)**, se tiene que:

$$
\begin{align*}
\forall n\in\mathbb{N}:&\: a>1\implies a^n>1 \\
&3>1\\
&1>0\\
\hline
3^n>0
\end{align*}
$$
{:.math}

Luego:

$$
\begin{align*}
3>2\\
3^n>0\\
\hline
3^{n+1}>2\cdot 3^n
\end{align*}
$$
{:.math}

Además

Luego:

$$
\begin{align*}
2>1\\
\hline
2+2^{n+1}>1+2^{n+1}
\end{align*}
$$
{:.math}

Finalmente:

$$3^1=3\land 3=1+2 \land 2=2^1\implies 3^1=1+2^1$${:.math}

Es decir, \\(p(1)\\) es verdadera.

$$
\begin{align*}
\forall n\in\mathbb{N}:p(n)&\iff 3^n\ge 1+2^n\\
&\implies 3^{n+1}>2\cdot 3^n\land \\
&\phantom{\implies}3^n\cdot 2\ge 2+2^{n+1}\land 2+2^{n+1}>1+2^{n+1}\\
&\implies 3^{n+1}>1+2^{n+1}\\
&\iff p(n+1)\\
\hline
\forall n\in\mathbb{N}:p(n)&\implies p(n+1)
\end{align*}
$$
{:.math}

Por lo tanto, \\(\forall n\in\mathbb{N}: 3^n\ge 1+2^n\\).

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">6</span>

Demuestre que \\(\forall n\in\mathbb{N}: n\ge 5\implies n^4<4^n\\).

#### Demostración

Si \\(n<5\\), la implicación es verdadera. Por lo tanto, sólo resta demostrar que \\(n^4<4^n\\) cuando \\(n\ge 5\\)

Si \\(n=5\\):

$$5^4=625<1024=4^5$${:.math}

Por lo tanto \\(p(5)\\) es verdadera.

Además:

$$
\begin{align*}
\forall n\in\mathbb{N}:&&n\ge 5&\implies n-1>3\\
\forall n\in\mathbb{N}:&&&\iff (n-1)^2>9\\
\forall n\in\mathbb{N}:&&&\implies (n-1)^2>2\\
\forall n\in\mathbb{N}:&&&\iff n^2-2n-1>0\\
\forall n\in\mathbb{N}:&&&\iff n^2>2n+1\\
\forall n\in\mathbb{N}:&&&\iff 2n^2>(n+1)^2\\
\forall n\in\mathbb{N}:&&&\iff 4n^4>(n+1)^4\\
\hline
\forall n\in\mathbb{N}:&&n\ge 5&\implies4n^4>(n+1)^4
\end{align*}
$$
{:.math}

Es necesario enfatizar que \\(n\ge 5\implies n-1\in\mathbb{N}\\), además, \\(2n^2,(n+1)\in\mathbb{N}\\). Por tanto, todos son mayores por cero, y ello nos permite utilizar la siguiente propiedad: \\(\forall a,b\in\mathbb{R}:a>0\land b>0\implies (a>b\iff a^2>b^2)\\).

Para terminar:

$$
\begin{align*}
\forall n\in\mathbb{N}:&&n\ge 5\land 4^n>n^4&\implies 4^{n+1}>4n^4\land 4n^4>(n+1)^4\\
\forall n\in\mathbb{N}:&& 4^{n+1}>4n^4\land 4n^4>(n+1)^4&\implies 4^{n+1}>(n+1)^4\\
\hline
\forall n\in\mathbb{N}:&&n\ge 5\land 4^n>n^4&\implies 4^{n+1}>(n+1)^4\\
\end{align*}
$$
{:.math}

Es decir: \\(\forall n\in\mathbb{N}: n\ge 5\implies n^4<4^n\\)