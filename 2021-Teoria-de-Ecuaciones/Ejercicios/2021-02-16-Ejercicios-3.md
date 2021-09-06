---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: 2021 02 09 Ejercicios 3 Libro de Álgebra.
nav_order: 2021-01-18
description: "Los ejercicios de la sección de inducción del libro."
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Ejercicios&nbsp;<span class="deg-sitio deg-sitio-texto">3</span>
{:.fs-9}

18 de febrero de 2021.
{:.fs-6 .fw-300}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">4</span> Desigualdad de Bernoulli

\\(\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:(1+\alpha)^n>1+n\alpha\\).

#### Solución

$$
\begin{align*}
\forall \alpha\in\mathbb{R}:&&\alpha>-1&\implies 1+\alpha>0\\
&&\alpha>-1&\\
\hline
&&1+\alpha>0 
\end{align*}
$${:.math}

Ahora. para \\(n=2\\), se tiene que, como \\(\alpha\ne 0\\):

$$\begin{align*}
(1+\alpha)^2=1+2\alpha+\alpha^2\land\alpha^2>0&\implies(1+\alpha)^2=1+2\alpha+\alpha^2\land 1+2\alpha+\alpha^2>1+2\alpha\\
\hline
(1+\alpha)^2&>1+2\alpha
\end{align*}
$${:.math}

Veamos el caso general:

$$\begin{align*}
\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:&&(1+\alpha)^n>1+n\alpha&\implies(1+\alpha)^{n+1}>(1+n\alpha)(1+\alpha)\\
&&&\land n\alpha^2 >0\\
&&&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha+n\alpha^2\\
&&&\land n\alpha^2 >0\\
&&&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha\\
\hline
\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:&&(1+\alpha)^n>1+n\alpha&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha
\end{align*}
$${:.math}

Por lo tanto, \\(\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:(1+\alpha)>1+n\alpha)\\).

**Nota importante:** *La expresión anterior puede ser cambiada a \\(\forall n \in\mathbb{N}: \forall\alpha\in\mathbb{R}\land\alpha>-1:(1+\alpha)\ge1+n\alpha\\), dado que el caso \\(n=1\\) es trivial por la definición de exponenciación y de neutro multiplicativo (se da la igualdad), y en el caso \\(\alpha=0\\), la igualdad se cumple, pues ya se ha demostrado que \\(1^n=1\\) para todo número natural. En tal caso, el razonamiento cambia ligeramente*

$$\begin{align*}
\forall n\in\mathbb{N}: \forall\alpha\in\mathbb{R}\land \alpha>-1:&&(1+\alpha)^n\ge 1+n\alpha&\implies(1+\alpha)^{n+1}\ge (1+n\alpha)(1+\alpha)\\
&&&\land n\alpha^2\ge 0\\
&&&\implies(1+\alpha)^{n+1}\ge1+(n+1)\alpha+n\alpha^2\\
&&&\land n\alpha^2\ge 0\\
&&&\implies(1+\alpha)^{n+1}\ge1+(n+1)\alpha\\
\hline
\forall n\in\mathbb{N}: \forall\alpha\in\mathbb{R}\land \alpha>-1:&&(1+\alpha)^n>1+n\alpha&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha
\end{align*}
$${:.math}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

\\(\forall n\in\mathbb{N}: (1+\frac{1}{n})^n\ge 2\\).

#### Solución 1

Dado que \\(\frac{1}{n}>0>-1\\), por la **Desigualdad de Bernoulli** (que incluye el caso de igualdad), se tiene que \\(\forall n\in\mathbb{N}: (1+\frac{1}{n})^n\ge 1+n\left(\frac{1}{n}\right)=2\\).

#### Solución 2

En esta solución, quiero demostrar que \\(\forall n\in\mathbb{N}: (1+\frac{1}{n+1})^{n+1}>(1+\frac{1}{n})^n\\).

Para ello, demostraremos la siguiente proposición:

$$\forall n\in\mathbb{N}:\frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}>1$${:.math}

$$\begin{align*}
\forall n\in\mathbb{N}:n>0&\iff n+1>1\\

&\iff (n+1)^2>1\\

&\iff 1>\frac{1}{(n+1)^2}\\

&\iff -\frac{1}{(n+1)^2}>-1\\

&\iff \left(1-\frac{1}{(n+1)^2}\right)^n
\ge\left(1-\frac{n}{(n+1)^2}\right)\\

&\iff \left(\frac{n(n+2)}{(n+1)^2}\right)^n\\
&\phantom{\iff}\ge\left(1-\frac{n}{(n+1)^2}\right)\\

&\iff \frac{(n(n+2))^n}{((n+1)^2)^n}\frac{n+2}{n+1}\\
&\phantom{\iff}\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}\\

&\iff \frac{(n(n+2))^n(n+2)}{((n+1)(n+1))^n(n+1)}\\
&\phantom{\iff}\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}\\

&\iff \frac{n^n(n+2)^n(n+2)}{(n+1)^n(n+1)^n(n+1)}\\
&\phantom{\iff}\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}\\

&\iff \frac{n^n(n+2)^{n+1}}{(n+1)^n(n+1)^{n+1}}\\
&\phantom{\iff}\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}\\


&\iff 1\frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}\\
&\phantom{\iff}\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}\\

\hline
\forall n\in\mathbb{N}:\frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}&\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}
\end{align*}
$${:.math}

$$\begin{align}
\forall n\in\mathbb{N}:\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}>1
 
&\iff \frac{n^2+n+1}{n^2+2n+1}\frac{n+2}{n+1}>1\\

&\iff \frac{n^3+3n^2+3m+2}{n^3+3n^2+3n+1}>1\\

&\iff n^3+3n^2+3m+2>n^3+3n^2+3n+1\\

&\iff 1>0\\
\hline
\forall n\in\mathbb{N}:\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}>1
\end{align}
$${:.math}

$$\begin{align}
\forall n\in\mathbb{N}:&\frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}\ge\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}\\
\forall n\in\mathbb{N}:&\left(1-\frac{n}{(n+1)^2}\right)\frac{n+2}{n+1}>1\\
\hline
\forall n\in\mathbb{N}:&\frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}>1
\end{align}
$${:.math}

Es decir,

$$\begin{align*}
\forall n\in\mathbb{N}:&\left(1+\frac{1}{n+1}\right)^{n+1}>\left(1+\frac{1}{n}\right)^n\\
&\iff \left(1+\frac{1}{n}\right)^n \frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}>\left(1+\frac{1}{n}\right)^n\\
&\iff \frac{n^n}{(n+1)^n}\frac{(n+2)^{n+1}}{(n+1)^{n+1}}>1\\
\hline
\forall n\in\mathbb{N}:&\left(1+\frac{1}{n+1}\right)^{n+1}>\left(1+\frac{1}{n}\right)^n\\
\end{align*}
$${:.math}

Finalmente, la solución se deduce a partir de lo que ya se ha demostrado:

Para \\(n=1\\), se tiene que

$$\left(1+\frac{1}{1}\right)^1=1+1=2\ge 2$${:.math}

Por lo que sólo queda analizar el caso general. 

$$\begin{align*}
\forall n\in\mathbb{N}:&&\left(1+\frac{1}{n}\right)^{n}\ge 2&\implies \left(1+\frac{1}{n+1}\right)^{n+1}>\left(1+\frac{1}{n}\right)^n\land\left(1+\frac{1}{n}\right)^{n}\ge 2\\
&&&\implies \left(1+\frac{1}{n+1}\right)^{n+1}>2\\
&&&\implies \left(1+\frac{1}{n+1}\right)^{n+1}>2\lor\left(1+\frac{1}{n+1}\right)^{n+1}=2\\
&&&\iff \left(1+\frac{1}{n+1}\right)^{n+1}\ge 2\\
\hline
\forall n\in\mathbb{N}:&&\left(1+\frac{1}{n}\right)^{n}\ge 2&\implies \left(1+\frac{1}{n+1}\right)^{n+1}\ge 2\\
\end{align*}
$${:.math}

Por lo tanto, \\(\forall n\in\mathbb{N}: (1+\frac{1}{n})^n\ge 2\\).

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">5</span>

\\(\forall n\ge 2\in\mathbb{N}:\forall a,b\in\mathbb{R}\land a+b>0\land a\ne b:\frac{a^n+b^n}{2}>\left(\frac{a+b}{2}\right)^n\\).

#### Solución

Haremos tres casos:

* Si \\(a=0\\):
  
  Primero:

  $$\begin{align*}
  2>1\\
  1^n=1\\
  1>\frac{1}{2}\\
  \forall n\in\mathbb{N}:1^n>\frac{1}{2}^n\\
  \hline
  \forall n\in\mathbb{N}:2>\frac{1}{2}^n\\
  \end{align*}
  $${:.math}
  
  $$\begin{align*}
  \neg(\forall a,b\in\mathbb{R}\land a+b>0\land a\ne b:a=0\implies b\ne 0\land b>0)
  &\iff \exists a,b\in\mathbb{R}\land a+b>0\land a\ne b:\neg(a=0\implies b\ne 0\land b>0)\\
  &\iff \exists a,b\in\mathbb{R}\land a+b>0\land a\ne b:a=0\land \neg(b\ne 0\land b>0)
  &\iff \exists a,b\in\mathbb{R}\land a+b>0\land a\ne b:a=0\land(b=0\lor b\le 0)
  &\iff \exists a,b\in\mathbb{R}\land a+b>0\land a\ne b:(a=0\land b=0)\lor (a=0\land b\le 0)
  &\iff \exists a,b\in\mathbb{R}\land a+b>0\land a\ne b:(a=b)\lor (a+b\le 0)
  \hline
  \forall a,b\in\mathbb{R}\land a+b>0\land a\ne b:a=0\implies b\ne 0\land b>0
  \end{align*}
  $${:.math}
  
  $$\begin{align*}
  \forall a,b\in\mathbb{R}\land a+b>0\land a\ne b:a=0
  &\implies b>0\\
  &\implies b^n>0
  \hline
  \forall a,b\in\mathbb{R}\land a+b>0\land a\ne b:a=0&\implies b^n> 0
  \end{align*}
  $${:.math}



  Por lo que





Entonces tenemos