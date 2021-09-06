---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: 2021 02 15 
nav_order: 2021-02-15
description: "Página de la materia"
last_modified_date: 2021-02-10T21:00:00+0000
grand_parent: Geometría Analítica
parent: Apuntes Geometría Analítica
---

# Ecuación vectorial de la&#x2000;<span class="deg-sitio deg-sitio-texto">recta</span>
{:.fs-9}

15 de febrero de 2021.
\\(\def\Real{\mathbb{R}} \def\Vec#1{\boldsymbol{#1}}\\)
{:.fs-6 .fw-300}

### Definición&nbsp;<span class="deg-sitio deg-sitio-texto">1</span> Ecuación vectorial de la recta

Sean \\(\Vec{P},\Vec{v}\in\Real^2:\Vec{v}\ne\Vec{0}\\). La línea \\(\ell\\) que pasa por \\(\Vec{P}\\) y tiene dirección \\(\Vec{v}\\). Se define como la colección de todos los puntos de la forma \\(\Vec{P}+t\Vec{v}\\), para alguna \\(t\in\Real\\). De manera simbólica:

$$\ell=\{\Vec{P}+t\Vec{v}:t\in\Real\}$${:.math}

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span> Pertenencia por igualdad y vectores paralelos

Sean \\(\ell_1=\\{\Vec{P}+t\Vec{v}:t\in\Real\\}\\) y \\(\ell_2=\\{\Vec{Q}+t\Vec{w}:t\in\Real\\}\\).

$$\ell_1=\ell_2\iff\Vec{P}\in\ell_2\land\Vec{v}\parallel\Vec{w}$${:.math}

#### Demostración

$$\begin{align*}
\ell_1=\ell_2&\implies(\forall\Vec{u}\in\Real^2:\Vec{u}\in\ell_1\iff\Vec{u}\in\ell_2)\land\Vec{P}\in\ell_1\land\Vec{P+v}\in\ell_1\\
&\implies\Vec{P}\in\ell_2\land\Vec{P+v}\in\ell_2\\
&\implies\Vec{P}\in\ell_2\land\exists t_0\in\Real:\Vec{P}=\Vec{Q}+t_0\Vec{w}\land\exists s_0\in\Real:\Vec{P+v}=\Vec{Q}+s_0\Vec{w}\\
&\implies\Vec{P}\in\ell_2\land\Vec{P-Q}=t_0\Vec{w}\land\Vec{P-Q+v}=s_0\Vec{w}\\
&\implies\Vec{P}\in\ell_2\land t_0\Vec{w}+\Vec{v}=s_0\Vec{w}\\
&\implies\Vec{P}\in\ell_2\land\Vec{v}=(s_0-t_0)\Vec{w}\\
&\implies\Vec{P}\in\ell_2\land\exists r\in\Real:\Vec{v}=r\Vec{w}\\
&\iff\Vec{P}\in\ell_2\land\Vec{v}\parallel\Vec{w}\\
\hline
\ell_1=\ell_2&\implies\Vec{P}\in\ell_2\land\Vec{P}\in\ell_2\land\Vec{v}\parallel\Vec{w}
\end{align*}
$${:.math}

Nota: \\(t_0\ne s_0\\), dado que, en caso contrario, \\(\Vec{P}=\Vec{P+v}\\), lo que implicaría \\(\Vec{v}=\Vec{0}\\), lo cual es imposible, ya que la definición de la ecuación vectorial de la recta exige que \\(\Vec{v}\ne\Vec{0}\\).

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span> Pertenencia por vector diferencia

Si \\(\ell:\Vec{P}+t\Vec{v}\\) y \\(\Vec{Q}\in\Real^2\\), entonces \\(\Vec{Q}\in\ell\\) sí y sólo sí \\(\Vec{Q}-\Vec{P}\perp\Vec{v}^{\perp}\\)

#### Demostración

Si \\(Q\in\ell\\), se cumple que para algún \\(t_0\in\Real\\)

$$Q=\Vec{P}+t_0\Vec{v}$${:.math}

Entonces \\(\Vec{Q}-\Vec{P}=t_0\Vec{v}\\), es decir, \\(\Vec{Q}-\Vec{P}\parallel\Vec{v}\\), y como \\(\Vec{v}\perp\\Vec{v}^{\perp}\\), se sigue que \\(\Vec{Q}-\Vec{P}\perp\\Vec{v}^{\perp}\\)