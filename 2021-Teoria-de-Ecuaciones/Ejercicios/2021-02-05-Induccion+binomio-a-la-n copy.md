---
layout: default
title: 2021 01 29 Ejercicio conjuntos inductivos.
nav_order: 2021-01-18
description: "Página de la materia"
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Demostraciones de&nbsp;<span class="deg-sitio deg-sitio-texto">Inducción Matemática</span>
{:.fs-9}

29 de enero de 2021.
{:.fs-6 .fw-300}

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Demuestre que \\(\forall n\in\mathbb{N}:\forall a\in\mathbb{R}:1^n-a^n=(1-a)(1+s_n)\\).

Donde:

* \\(s_1=0\\)
* \\(s_{n+1}=s_{n}+a^{n}\\).

#### Demostración

Sea \\(p(n)\equiv \forall a\in\mathbb{R}:1^n-a^n=(1-a)(1+s_n)\\).

$$
\begin{align*}
1^1-a^1=1^1-a^1&\implies 1^1-a^1=1-a\\
&\implies (1^1-a^1)(1)=(1-a)(1)\\
&\implies 1^1-a^1=(1-a)(1+0)\\
&\implies 1^1-a^1=(1-a)(1+s_1)\\
\hline
p(1)
\end{align*}
$$
{:.math}

$$
\begin{align*}
p(n)&\equiv 1^n-a^n=(1-a)(1+s_n)\\
&\implies 1^n-a^n+(1-a)(a^n)=(1-a)(1+s_n)+(1-a)a^n\\
&\implies 1^n-a^n+a^n-a^{n+1}=(1-a)(1+s_n)+(1-a)a^n\\
&\implies 1^n\cdot 1+0-a^{n+1}=(1-a)(1+s_n+a^n)\\
&\implies 1^{n+1}-a^{n+1}=(1-a)(1+s_n+a^n)\\
&\implies 1^{n+1}-a^{n+1}=(1-a)(1+s_{n+1})\\
&\equiv p(n+1)\\
\hline
p(n)\implies p(n+1)
\end{align*}
$$
{:.math}

Concluimos que \\(\forall n\in\mathbb{N}:p(n)\\).

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

Demuestre que \\(\forall n\in\mathbb{N}:\forall a\ne 0\in\mathbb{R}:\forall b\in\mathbb{R}:a^n-b^n=(a-b)(a^{n-1}+S_n)\\).

Donde:

* \\(S_1=0\\)
* \\(S_{n+1}=a^{n}\cdot s_{n}+b^n\\).

#### Demostración

Se evalúa el **Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>** con el número real \\(\frac{b}{a}\\). Y se multiplica la igualdad por \\(a^n\\). Nótese que \\(S_{n}=a^{n-1}\cdot s_n\\)



















