---
layout: default
title: 2021 02 03 El plano y las rectas.
nav_order: 2021-01-18
description: "Página de la materia"
last_modified_date: 2021-02-03T21:00:00+0000
grand_parent: Geometría Analítica
parent: Apuntes Geometría Analítica
---

# El plano y las&nbsp;<span class="deg-sitio deg-sitio-texto">rectas</span>
{:.fs-9}

3 de febrero de 2021.
{:.fs-6 .fw-300}

## Coordenadas cartesianas

Sea \\(\mathbb{R}^2=\\{(a,b)\|a,b\in\mathbb{R}\\}\\), es decir, \\(\mathbb{R}^2\\) es el conjunto de todas las parejas ordenadas de números reales \\((a,b)\\). Esto puede interpretarse de la siguiente manera:

Tómense dos rectas reales perpendiculares \\(X\\) y \\(Y\\), a las cuales podemos referirnos como ejes (coordenados). Cualquier punto \\(P\\) en el plano se corresponde a una pareja de números reales \\((a,b)\\), los cuales serán las coordenadas de dicho punto. A la primera coordenada se le llama *coordenada \\(x\\)* o *abcisa*, y a la segunda, *coordenada \\(y\\)* u *ordenada*. 

El punto \\(P\\) es representado como la intersección de la recta \\(\ell_1\\) (que es paralela a \\(Y\\) e intersecta a \\(X\\) en el punto \\(a\\)), con la recta \\(\ell_2\\), (que es paralela a \\(X\\) e intersecta a \\(Y\\) en el punto \\(b\\)).

Se define al punto de intersección de \\(X\\) y \\(Y\\) como el punto \\((0,0)\\).

### Propiedad&nbsp;<span>1</span>{:.deg-sitio .deg-sitio-texto} Igualdad

Para cualesquiera \\((x_1,y_1),(x_2,y_2)\in\mathbb{R}^2\\), \\((x_1,y_1)=(x_2,y_2)\iff\\) \\(x_1=x_2\land y_1=y_2\\).

## Distancia

Sean \\(P_1=(x_1,y_1)\\) y \\(P_2=(x_2,y_2)\\) dos puntos en el plano. La distancia entre \\(P_1\\) y \\(P_2\\), denotada como \\(\|P_1P_2\|\\), satisface la siguiente igualdad:

$$|P_1P_2|=\sqrt{(x_1-x_2)^2+(y_1-y_2)^2}$${:.math}

## Rectas

Las rectas, entendidas como conjuntos de puntos, son subconjuntos de \\(\mathbb{R}^2\\) que cumplen las siguientes propiedades:

### Propiedad&nbsp;<span>2</span>{:.deg-sitio .deg-sitio-texto} Axioma de geometría euclídea

Por cualesquiera dos puntos pasa una única recta.

### Propiedad&nbsp;<span>3</span>{:.deg-sitio .deg-sitio-texto} Rectas paralelas a \\(X\\) o \\(Y\\)

Una recta \\(\ell\\) es paralela al eje \\(X\\) sí y sólo sí todos los puntos que la conforman tienen la misma abcisa: \\(\ell\parallel X\iff \exists x_0\in\mathbb{R}:\forall (x,y)\in\ell:x=x_0\\)

Una recta \\(\ell\\) es paralela al eje \\(Y\\) sí y sólo sí todos los puntos que la conforman tienen la misma ordenada: \\(\ell\parallel X\iff \exists y_0\in\mathbb{R}:\forall (x,y)\in\ell:y=y_0\\).

### Propiedad&nbsp;<span>4</span>{:.deg-sitio .deg-sitio-texto} Pendiente

Toda recta \\(\ell\\) no paralela al eje \\(X\\) satisface que, para cualesquiera \\((x_1,y_1),(x_2,y_2)\in\ell:(x_1,y_1)\ne(x_2,y_2)\\) sí y sólo sí existe un único número real \\(m\\) tal que \\(\frac{y_1-y_2}{x_1-x_2}=m\\). Este número se define como **la pendiente de la recta \\(\ell\\)**.

$$\begin{align*}
\forall(x_1,y_1),(x_2,y_2)\in\ell:&\:(x_1,y_1)\ne(x_2,y_2)\iff\\
&\;\;\left(\forall m,n\in\mathbb{R}:\left(\frac{y_1-y_2}{x_1-x_2}=m\land\frac{y_1-y_2}{x_1-x_2}=n\right)\implies m=n\right)\end{align*}$${:.math}

Dicho de otra manera:

$$\forall(x_1,y_1),(x_2,y_2)\in\ell:(x_1,y_1)\ne(x_2,y_2)\iff\left(\exists! m\in\mathbb{R}:\frac{y_1-y_2}{x_1-x_2}=m\right)$${:.math}

Donde \\(\exists!\\) es el cuantificador existencial único.

