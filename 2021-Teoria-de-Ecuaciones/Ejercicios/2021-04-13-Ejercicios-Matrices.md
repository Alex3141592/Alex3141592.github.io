---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 04 13 Ejercicios Matrices
nav_order: 2021-01-18
description: "Inducción"
last_modified_date: 2021-03-20T18:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Problemas de&nbsp;<span class="deg-sitio deg-sitio-texto">Matrices</span>
{:.fs-9}



# Ejercicios&nbsp;<span class="deg-sitio deg-sitio-texto">Matrices</span>
{:.fs-9}

En los ejercicios se utilizará la propiedad de asociatividad. Sea \\(M\\) el conjunto de matrices \\(2\times 2\\).

$$\forall A,B,C\in M: (A\times B)\times C=A\times(B\times C)$${:.math}

Se tiene que la matriz identidad es \\(I=\begin{pmatrix}1&0\\\\0&1\end{pmatrix}\\)

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

Sea \\(A,B\in M\\). Demuestre que 

$$|AB|=|A|\:|B|$${:.math}

#### Solución

Sean

$$A=\begin{pmatrix}
    a_{11}&a_{12}\\
    a_{21}&a_{22}
\end{pmatrix},\;B=\begin{pmatrix}
    b_{11}&b_{12}\\
    b_{21}&b_{22}
\end{pmatrix}$$

Entonces

$$A\times B=\begin{pmatrix}
    a_{11}b_{11}+a_{12}b_{21}&a_{11}b_{12}+a_{12}b_{22}\\
    a_{21}b_{11}+a_{22}b_{21}&a_{21}b_{12}+a_{22}b_{22}
\end{pmatrix}$${:.math}

Finalmente:

$$\begin{align*}
|A\times B|&=\begin{vmatrix}
    a_{11}b_{11}+a_{12}b_{21}&a_{11}b_{12}+a_{12}b_{22}\\
    a_{21}b_{11}+a_{22}b_{21}&a_{21}b_{12}+a_{22}b_{22}
\end{vmatrix}\\[1em]
&=a_{11}a_{21}b_{11}b_{12}+a_{11}a_{22}b_{11}b_{22}+a_{12}a_{21}b_{21}b_{12}+a_{12}a_{22}b_{21}b_{22}
-a_{21}a_{11}b_{11}b_{12}-a_{21}a_{12}b_{11}b_{22}-a_{22}a_{11}b_{12}b_{21}-a_{22}a_{12}b_{12}b_{22}\\[1em]
&=a_{11}a_{22}b_{11}b_{22}+a_{12}a_{21}b_{21}b_{12}-a_{21}a_{12}b_{11}b_{22}-a_{22}a_{11}b_{12}b_{21}\\[1em]
&=(a_{11}a_{22}-a_{12}a_{21})(b_{11}b_{22}-b_{12}b_{21})\\[1em]
&=|A|\:|B|
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

Sea \\(A\in M\\) tal que \\(\|A\|\ne 0\\). Demuestre que 

$$A=(A^{-1})^{-1}$${:.math}

#### Solución

Primero, como \\(\|A\|\ne 0\\),

$$\exists!A^{-1}\in M: A\times A^{-1}=I$${:.math}

es decir, existe una matriz inversa a \\(A\\) y es única. Ahora, como \\(\|A\|\ne 0\\), \\(\|A\|^{-1}=\|A^{-1}\|\ne 0\\). Por tanto, \\(A^{-1}\\) tiene inversa.

Se cumple que

$$A^{-1}\times(A^{-1})^{-1}=(A^{-1})^{-1}\times A^{-1}=I$${:.math}

$$A^{-1}\times A=A\times A^{-1}=I$${:.math}

Luego, como la inversa de \\(A^{-1}\\) es única, \\((A^{-1})^{-1}=A\\).

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">3</span>


#### Solución

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">4</span>


#### Solución

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">5</span>

#### Solución

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">6</span>


#### Solución

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">7</span>

#### Solución