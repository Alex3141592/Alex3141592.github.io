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

# Examen de&nbsp;<span class="deg-sitio deg-sitio-texto">Inducción</span>
{:.fs-9}

**<span class="deg-sitio deg-sitio-texto">Alumno:</span>** Alexis Jonathan Dorantes Vázquez
{:.fs-6 .fw-300}

**<span class="deg-sitio deg-sitio-texto">Materia:</span>** Teoría de Ecuaciones
{:.fs-6 .fw-300}

**<span class="deg-sitio deg-sitio-texto">Matrícula:</span>** 202081434
{:.fs-6 .fw-300}


20 de febrero de 2021.
{:.fs-6 .fw-300}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Dados \\(a,b\in\mathbb{R}\\). Demostrar que \\((ab)^n=a^nb^n\\) para todo \\(n\in\mathbb{N}\\).

#### Demostración

La proposición planteada es equivalente a \\(\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}:(ab)^n=a^nb^n\\).

Analicemos el caso \\(n=1\\):

$$(ab)^1=ab=a^1b^1$${:.math}

El cual se cumple por las igualdades anteriores.

En el caso general:

$$
\begin{align*}
\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}:&&(ab)^n=a^nb^n&\implies (ab)^n(ab)=a^nb^n(ab)\\
&&&\implies (ab)^{n+1}=a^n(ab)b^n\\
&&&\implies (ab)^{n+1}=(a^na)bb^n\\
&&&\implies (ab)^{n+1}=a^{n+1}b^{n+1}\\
\hline
\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}:&&(ab)^n=a^nb^n&\implies (ab)^{n+1}=a^{n+1}b^{n+1}\\
\end{align*}
$$
{:.math}

Por lo tanto, \\(\forall n\in\mathbb{N}:\forall a,b\in\mathbb{R}:(ab)^n=a^nb^n\\).

<div> </div>
{:.salto .no-mostrar}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

Demuestre que \\(n^4<4^n\\) para todo \\(n\ge 5\\).

#### Demostración

La proposición a demostrar es equivalente a \\(\forall n\in\mathbb{N}: n\ge 5\implies n^4<4^n\\).

Si \\(n<5\\), la implicación es verdadera. Por lo tanto, sólo resta demostrar que \\(n^4<4^n\\) cuando \\(n\ge 5\\)

Si \\(n=5\\):

$$5^4=625<1024=4^5$${:.math}

Por lo tanto, la proposición se cumple cuando \\(n=5\\).

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

Es decir: \\(\forall n\in\mathbb{N}: n\ge 5\implies n^4<4^n\\).

<div> </div>
{:.salto .no-mostrar}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

Encontrar \\(n\in\mathbb{N}\\) tal que

$$3\binom{n}{4}=5\binom{n-1}{5}$${:.math}

#### Demostración

Nótese que \\(\forall n,m\in\mathbb{N}:n-m>0\iff n>m\\) (Pues \\(\mathbb{N}\subset\mathbb{R}\\)). Esto será de utilidad en las operaciones que se realicen más adelante.

Además, \\(\binom{n-1}{5}\\) está definido cuando \\(n-1\ge5\\), es decir, cuando \\(n\ge 6\\) (con el otro coeficiente binomial, tenemos \\(n\ge 4\\), pero \\(n\ge 6\implies n\ge 4\\)). 

Podemos realizar el siguiente razonamiento:

$$
\begin{align*}
n\ge 6\land 3\binom{n}{4}=5\binom{n-1}{5}\\[1em]
n\ge 6\land 3\binom{n}{4}=5\binom{n-1}{5}&\iff n\ge 6\land 3\frac{n!}{4!(n-4)!}=5\frac{(n-1)!}{5!(n-1-5)!}\\
&\iff n\ge 6\land \frac{3}{4!}\frac{n!}{(n-4)!}=\frac{5}{5!}\frac{(n-1)!}{(n-1-5)!}\\[1em]
&\iff n\ge 6\land \frac{3}{4!}\frac{\prod^n_{i=1}i}{\prod^{n-4}_{i=1}i}=\frac{5}{5!}\frac{\prod^{n-1}_{i=1}i}{\prod^{n-6}_{i=1}i}\\[1em]
&\iff n\ge 6\land \frac{3}{4!}\left(\prod^n_{i=(n-4)+1}i\right)=\frac{5}{5!}\left(\prod^{n-1}_{i=(n-6)+1}i\right)\\[1em]
&\iff n\ge 6\land \frac{3}{4!}\left(\prod^n_{i=n-3}i\right)=\frac{5}{5!}\left(\prod^{n-1}_{i=n-5}i\right)\\[1em]
&\iff n\ge 6\land\\[1em]
&\phantom{\iff}\frac{3}{4!}(n-3)(n-2)(n-1)n=\frac{5}{5!}(n-5)(n-4)(n-3)(n-2)(n-1)\\
&\iff n\ge 6\land \frac{3}{4!}n=\frac{5}{5!}(n-5)(n-4)\\[1em]
&\iff n\ge 6\land \frac{3n}{4!}=\frac{5(n-5)(n-4)}{5(4!)}\\[1em]
&\iff n\ge 6\land \frac{3n}{4!}4!=\frac{(n-5)(n-4)}{4!}4!\\[1em]
\end{align*}
$${:.math .fs-3}

$$
\begin{align*}
\phantom{n\ge 6\land 3\binom{n}{4}=5\binom{n-1}{5}}&\phantom{\iff\frac{3}{4!}(n-3)(n-2)(n-1)n=\frac{5}{5!}(n-5)(n-4)(n-3)(n-2)(n-1)}\\

&\iff n\ge 6\land 3n=(n-5)(n-4)\\
&\iff n\ge 6\land 3n=n^2-9n+20\\
&\iff n\ge 6\land 0=n^2-12n+20\\
&\iff n\ge 6\land 0=(n-2)(n-10)\\
&\iff n\ge 6\land (n-2=0\lor n-10=0)\\
&\iff n\ge 6\land (n=2\lor n=10)\\
&\iff (n\ge 6\land n=2)\lor(n\ge 6\land n=10)\\
&\iff n\ge 6\land n=10\\
&\iff n=10\\
\hline
n=10
\end{align*}
$${:.math .fs-3}

Por lo que el único valor de \\(n\in\mathbb{N}\\) que satisface la igualdad es \\(n=10\\).

Nota: *Cuando se realizó la división entre \\((n-3)(n-2)(n-1)\\), se hizo porque \\(n\ge 6\implies n>3\land n>2 \land n>1\\), es decir, \\(n-1\\), \\(n-2\\) y \\(n-3\\) son números mayores a cero, luego sus respectivos inversos multiplicativos existen.*

<div> </div>
{:.salto .no-mostrar}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">4</span>

Sea \\(r\ne 0\\) y \\(a_{n+1}=ra_n\\) para todo \\(n\in\mathbb{N}\\). Demostrar que

$$a_1+a_2+\cdots+a_n=\frac{a_{n+1}−a_1}{r−1}$${:.math}

para todo \\(n\in\mathbb{N}\\).

#### Demostración

Vemos que la proposición a demostrar es equivalente a:

$$\forall n\in\mathbb{N}:\forall r\in\mathbb{R}\backslash 0\land r\ne 1:\sum^n_{i=1}a_i=\frac{a_{n+1}−a_1}{r−1}$${:.math}

Tomando como premisa que

$$\forall n\in\mathbb{N}:\forall r\in\mathbb{R}\backslash 0\land r\ne 1:a_{n+1}=ra_n$${:.math}

Analicemos si la proposición es cierta para \\(n=1\\):

Primero, veamos que:

$$\begin{align*}
\forall n\in\mathbb{N}:\forall r\in\mathbb{R}\backslash 0\land r\ne 1:&a_{n+1}=ra_n\\
1\in\mathbb{N}\\
\hline
a_2=ra_1
\end{align*}
$${:.math}

Por lo que

$$\begin{align*}
\sum^1_{i=1}a_i=\frac{a_{1+1}−a_1}{r−1}&\iff (r-1)\left(\sum^1_{i=1}a_i\right)=\frac{a_{1+1}−a_1}{r−1}(r-1)
&&\text{Dado que }\\
&&&(r-1=0\iff r=1)\land r\ne 1\\[1em]

&\iff (r-1)\left(a_1\right)=a_{1+1}−a_1
&&\text{Propiedad de sumatoria y}\\
&&&\text{de inverso multiplicativo}\\[1em]

&\iff ra_1-a_1=a_{1+1}−a_1
&&\text{Ley distributiva}\\[1em]

&\iff ra_1=a_{1+1}
&&\text{Ley de cancelación}\\[1em]

&\iff a_2=ra_1
&&\\
\hline
\sum^1_{i=1}a_i=\frac{a_{1+1}−a_1}{r−1}
\end{align*}
$${:.math .fs-3}

Es decir, la proposición se cumple cuando \\(n=1\\).

Ahora veamos el caso general

$$\begin{align*}
\forall n\in\mathbb{N}:\forall r\in\mathbb{R}\backslash 0\land r\ne 1:a_{n+1}=ra_n\\[1em]

\forall n\in\mathbb{N}:\forall r\in\mathbb{R}\backslash 0\land r\ne 1:\sum^n_{i=1}a_i=\frac{a_{n+1}−a_1}{r−1}
&\implies \left(\sum^n_{i=1}a_i\right)+a_{n+1}=\frac{a_{n+1}−a_1}{r−1}+a_{n+1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{a_{n+1}−a_1}{r−1}+\frac{a_{n+1}}{1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{(a_{n+1}−a_1)1+(r-1)(a_{n+1})}{(r−1)1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{(a_{n+1}−a_1)+(ra_{n+1}-a_{n+1})}{r−1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{(ra_{n+1}-a_{n+1})+(a_{n+1}−a_1)}{r−1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{a_{n+2}+(-a_{n+1}+a_{n+1})−a_1}{r−1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{a_{n+2}+0−a_1}{r−1}\\[1em]
&\implies \sum^{n+1}_{i=1}a_i=\frac{a_{n+2}−a_1}{r−1}\\[1em]
&\iff \sum^{n+1}_{i=1}a_i=\frac{a_{(n+1)+1}−a_1}{r−1}\\[1em]
\hline
\forall n\in\mathbb{N}:\forall r\in\mathbb{R}\backslash 0\land r\ne 1:\sum^n_{i=1}a_i=\frac{a_{n+1}−a_1}{r−1}&\implies \sum^{n+1}_{i=1}a_i=\frac{a_{(n+1)+1}−a_1}{r−1}
\end{align*}
$${:.math .fs-3}

Lo cual finaliza la demostración.

<div> </div>
{:.salto .no-mostrar}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">5</span> Desigualdad de Bernoulli

Sea \\(\alpha\ne0\\) y \\(\alpha>-1\\). Demostrar que

$$(1+\alpha)^n>1+n\alpha$${:.math}

para todo \\(n\ge2\\).

#### Demostración

La proposición a demostrar es equivalente a 

$$\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:(1+\alpha)^n>1+n\alpha .$${:.math}

El siguiente razonamiento muestra que \\(1+\alpha>0\\), lo cual será necesario para utilizar el axioma de la consistencia de la relación de orden bajo el producto.

$$
\begin{align*}
\forall \alpha\in\mathbb{R}:&&\alpha>-1&\implies 1+\alpha>0\\
&&\alpha>-1&\\
\hline
&&1+\alpha>0 
\end{align*}
$${:.math}

Ahora. para \\(n=2\\), se tiene que, como \\(\alpha\ne 0\\), \\(\alpha^2>0\\):

$$\begin{align*}
(1+\alpha)^2=1+2\alpha+\alpha^2\land\alpha^2>0&\implies(1+\alpha)^2=1+2\alpha+\alpha^2\land 1+2\alpha+\alpha^2>1+2\alpha\\
\hline
(1+\alpha)^2&>1+2\alpha
\end{align*}
$${:.math}

Veamos el caso general:

$$\begin{align*}
\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:(1+\alpha)^n>1+n\alpha&\implies(1+\alpha)^{n+1}>(1+n\alpha)(1+\alpha)\\
&\phantom{\implies}\land n\alpha^2 >0\\
&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha+n\alpha^2\\
&\phantom{\implies}\land n\alpha^2 >0\\
&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha\\
\hline
\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:(1+\alpha)^n>1+n\alpha&\implies(1+\alpha)^{n+1}>1+(n+1)\alpha
\end{align*}
$${:.math .fs-3}

Por lo tanto, \\(\forall n\in\mathbb{N}\land n\ge 2 : \forall\alpha\in\mathbb{R}\backslash 0\land \alpha>-1:(1+\alpha)>1+n\alpha)\\).

Nota: *\\(n\alpha^2>0\\), dado que \\(n\\) es natural y por tanto, mayor a \\(0\\). Además, \\(\alpha^2>0\\).*