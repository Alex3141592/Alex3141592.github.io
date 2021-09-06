---
layout: default
title: 2021 01 29 Ejercicio conjuntos inductivos.
nav_order: 2021-01-18
description: "Página de la materia"
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Demostraciones sobre conjuntos inductivos y&nbsp;<span class="deg-sitio deg-sitio-texto">\\(\mathbb{N}\\)</span>
{:.fs-9}

29 de enero de 2021.
{:.fs-6 .fw-300}

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">3.5.1</span>

1. \\(\mathbb{N}\\) es inductivo.
2. Si \\(A\\) es inductivo,  \\(\mathbb{N}\subset A\\).

#### Demostración 1

La expresión \\(\left(\forall x\in U:p(x)\implies q(x)\right)\implies \left(\forall x\in U:p(x)\implies\forall x\in U: q(x)\right)\\) es tautología.

Sea \\(I\\) el conjunto de todos los conjuntos inductivos. El siguiente razonamiento es válido, tomando como premisas la tautología anterior y, que para todo número real \\(x\\), si \\(x\\) es elemento de un conjunto inductivo, \\(x+1\\) también es un elemento de dicho conjunto inductivo:

$$
\begin{align*}
\forall x\in \mathbb{R}:&\left(\forall A\in I:x\in A\implies x+1\in A\right)\\
\forall x\in \mathbb{R}:&\left(\forall A\in I:x\in A\implies x+1\in A\right)\\
&\implies \left(\forall A\in I:x\in A\implies\forall A\in I: x+1\in A\right)\\
\hline
\forall x\in \mathbb{R}:&\:\forall A\in I:x\in A\implies\forall A\in I: x+1\in A
\end{align*}
$$
{:.math}

La conclusión nos dice que para todo número real \\(x\\), si \\(x\\) pertenece a cualquier conjunto inductivo, entonces \\(x+1\\) pertenece a cualquier conjunto inductivo.

Sea \\(\mathbb{N}\\) la intersección de todos los conjuntos inductivos. Por definición, \\(\mathbb{N}=\\{x\in R\|\forall A\in I: x\in A\\}\\).

En el siguiente razonamiento, si tomamos como premisas la definición del conjunto \\(\mathbb{N}\\) y que el número 1 pertenece a cualquier conjunto inductivo, concluimos que 1 pertenece al conjunto \\(\mathbb{N}\\): 

$$
\begin{align*}
\forall x\in \mathbb{R}:&\forall A\in I:x\in A\iff x\in \mathbb{N} \\
\forall A\in I:&\:1\in A\\
\hline
1\in \mathbb{N}
\end{align*}
$$
{:.math}

Finalmente, dado que hemos demostrado que \\(\forall x\in \mathbb{R}:\forall A\in I:x\in A\implies\forall A\in I: x+1\in A\\), entonces podemos utilizar esta proposición como premisa, junto a la definición del conjunto \\(\mathbb{N}\\):

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\iff \forall A\in I:x\in A\\
\forall x\in \mathbb{R}:&&\forall A\in I:x\in A&\implies\forall A\in I: x+1\in A\\
\forall x\in \mathbb{R}:&&\forall A\in I:x+1\in A&\iff x+1\in \mathbb{N}\\
\hline
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\implies x+1\in \mathbb{N}
\end{align*}
$$
{:.math}

Todo lo anterior demuestra que \\(\mathbb{N}\\) es un conjunto inductivo.

Nota: *Dado que \\(\mathbb{N}\\) es inductivo, tenemos que \\(n\in\mathbb{N}\implies n+1\in\mathbb{N}\\). Por lo tanto, si en algún momento se tiene que la proposición \\(n\in\mathbb{N}\\) es verdadera, entonces la proposición \\(n+1\in\mathbb{N}\\) es verdadera. Es decir:*

$$
\begin{align*}
n\in\mathbb{N}&\\
n\in\mathbb{N}&\implies n+1\in\mathbb{N}\\
\hline
n+1\in\mathbb{N}
\end{align*}
$$
{:.math}

#### Demostración 2

En el siguiente razonamiento, la primera premisa es la definición del conjunto de los números naturales, la segunda premisa indica que si el la expresión del cuantificador es verdadera, entonces lo es para cualquier elemento.

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\iff \forall A\in I:x\in A\\
\forall x\in \mathbb{R}:&&(\forall A\in I:x\in A)&\implies x\in A\\
\hline
\forall x\in \mathbb{R}:&&x\in\mathbb{N}&\implies x\in A
\end{align*}
$$
{:.math}

Dado que \\(\forall x\in \mathbb{R}: \\: x\in\mathbb{N}\implies x\in A\\) \\(\equiv \mathbb{N}\subset A\\), concluimos la demostración.

### Corolario&nbsp;<span class="deg-sitio deg-sitio-texto">3.5.2</span>

\\(\forall n\in \mathbb{N}: n\ge1\\).

#### Demostración

Sea \\(A=\\{x\in \mathbb{R}\|x\ge 1\\}\\).

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in &\iff x\ge1 \\
1\ge 1\\
\hline
1\in A&&
\end{align*}
$$
{:.math}

Además:

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in A&\iff x\ge 1 \\
\forall x\in \mathbb{R}:&&x\ge 1&\implies x\ge 1 \land 1>0\\
\forall x\in \mathbb{R}:&&x\ge 1\land 1>0&\implies x>0\\
\forall x\in \mathbb{R}:&&x>0&\implies x+1>0+1\\
\forall x\in \mathbb{R}:&&x+1>0+1&\implies x+1>1\\
\forall x\in \mathbb{R}:&&x+1>1&\implies x+1 \in A\\
\hline
\forall x\in \mathbb{R}:&&x\in A&\implies x+1\in A
\end{align*}
$$
{:.math}

Es decir, \\(A\\) es inductivo, por lo que \\(\mathbb{N}\subset A\\).

Finalmente:

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\implies x\in A \\
\forall x\in \mathbb{R}:&&x\in A&\implies x\ge1\\
\hline
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\implies x\ge 1
\end{align*}
$$
{:.math}

### Corolario&nbsp;<span class="deg-sitio deg-sitio-texto">3.5.3</span> Principio de Inducción Matemática

Si \\(A\subset\mathbb{N}\\) y \\(A\\) es inductivo, entonces \\(A=\mathbb{N}\\).

#### Demostración

$$
\begin{align*}
\forall X\in I:&\:\mathbb{N}\subset X\\
A\subset \mathbb{N}&\land A\in I\\
\hline
A=\mathbb{N}
\end{align*}
$$
{:.math}

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">3.5.4</span>

1. \\(\forall m,n \in \mathbb{N}:m+n\in\mathbb{N}\\).
2. \\(\forall m,n \in \mathbb{N}:mn\in\mathbb{N}\\).

#### Demostración 1

\\(\forall m,n \in \mathbb{N}:m+n\in\mathbb{N}\\) \\(\equiv \forall m\in\mathbb{N}:(\forall n \in \mathbb{N}:m+n\in\mathbb{N})\\).

Sea \\(A=\\{n\in \mathbb{N}\|m+n\in\mathbb{N}\\}\\). Vemos que, dado que:

$$
\begin{align*}
1\in\mathbb{N}&\\
\mathbb{N}\in I&\\
m\in\mathbb{N}&\implies m+1\in\mathbb{N}\\
\hline
1\in A
\end{align*}
$$
{:.math}

Luego:

$$
\begin{align*}
\forall n\in\mathbb{R}:&&n\in A&\implies m+n\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&m+n\in\mathbb{N}&\implies (m+n)+1\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&(m+n)+1\in\mathbb{N}&\implies m+(n+1)\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&m+(n+1)\in\mathbb{N}&\implies n+1\in A\\
\hline
\forall n\in\mathbb{R}:&&n\in A&\implies n+1\in A\\
\end{align*}
$$
{:math}

Finalmente, \\(A\\) es inductivo, y por el **Principio de Inducción Matemática**, \\(A=\mathbb{N}\\).

#### Demostración 2

\\(\forall m,n \in \mathbb{N}:mn\in\mathbb{N}\\) \\(\equiv \forall m\in\mathbb{N}:(\forall n \in \mathbb{N}:mn\in\mathbb{N})\\).

Sea \\(A=\\{n\in \mathbb{N}\|mn\in\mathbb{N}\\}\\). Vemos que, dado que:

$$
\begin{align*}
1\in\mathbb{N}&\\
m\in\mathbb{N}&\implies m(1)\in\mathbb{N}\\
\hline
1\in A
\end{align*}
$$
{:.math}

Luego:

$$
\begin{align*}
\forall n\in\mathbb{R}:&&n\in A&\implies mn\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&mn\in\mathbb{N}&\implies mn+m\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&mn+m\in\mathbb{N}&\implies mn+m(1)\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&mn+m(1)\in\mathbb{N}&\implies m(n+1)\in\mathbb{N}\\
\forall n\in\mathbb{R}:&&m(n+1)\in\mathbb{N}&\implies n+1\in A\\
\hline
\forall n\in\mathbb{R}:&&n\in A&\implies n+1\in A\\
\end{align*}
$$
{:math}

Finalmente, \\(A\\) es inductivo, y por el **Principio de Inducción Matemática**, \\(A=\mathbb{N}\\).

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">3.5.5</span>

Todo número natural diferente de 1 se puede escribir como la suma de 1 más algún número natural.

#### Demostración

Sea \\(A=\\{n\in\mathbb{N}\|n=1\lor \exists m\in\mathbb{N}:1+m=n\\}\\).

$$
\begin{align*}
(n=1\lor \exists m\in\mathbb{N}:1+m=n)&\iff n\in A\\
\hline
1\in A
\end{align*}
$$
{:.math}

Lo anterior indica que \\(1\in A\\).

Ahora supóngase que \\(n\in A\\). Entonces \\(\exists m\in\mathbb{N}:1+m=n\\). Dado que \\(m,n\in\mathbb{N}\\), \\(m+1,n+1\in \mathbb{N}\\).

$$
\begin{align*}
\forall n\in\mathbb{R}:&&n\in A&\iff (\exists m\in\mathbb{N}:1+m=n)\lor 1=n&\\
\forall n\in\mathbb{R}:&&&\iff (\exists m\in\mathbb{N}:1+m+1=n+1)\lor 1+1=n+1\\
\forall n\in\mathbb{R}:&&&\iff (\exists m\in\mathbb{N}:1+(m+1)=n+1)\lor 1+1=n+1\\
\forall n\in\mathbb{R}:&&&\implies n+1\in A\\
\hline
\forall n\in\mathbb{R}:&&n\in A&\implies n+1\in A
\end{align*}
$$
{:.math}

Por tanto, \\(A\\) es inductivo. Por el **Principio de Inducción Matemática**, \\(A=\mathbb{N}\\)

### Corolario&nbsp;<span class="deg-sitio deg-sitio-texto">3.5.6</span>

Todo número natural diferente de 1 se puede escribir como la suma de 1 más algún número natural.









