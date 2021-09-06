---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: 2021 02 09 Propiedad 2 pag. 20 Libro de álgebra.
nav_order: 2021-01-18
description: "Los ejercicios de la sección de inducción del libro."
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Demostración sobre&nbsp;<span class="deg-sitio deg-sitio-texto">sumatorias</span>
{:.fs-9}

29 de enero de 2021.
{:.fs-6 .fw-300}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

Demuestre que \\(\displaystyle\forall n\in\mathbb{N}:\sum^n_{i=0}a_i=\sum^{n+1}\_{i=1}a_{i-1}\\).

#### Demostración
Sea \\(\displaystyle p(n)\equiv\sum^n_{i=0}a_i=\sum^{n+1}\_{i=1}a_{i-1}\\).

Vemos que:

$$\begin{align*}
p(1)&\iff\sum^1_{i=0}a_i=\sum^{1+1}_{i=1}a_{i-1}\\
&\iff a_0+\sum^1_{i=1}a_i=\sum^{1}_{i=1}a_{i-1} + a_1\\
&\iff a_0+a_1=a_0+a_1\\
\hline
p(1)
\end{align*}
$${:.math}

Ahora, en el caso general:

$$\begin{align*}
\forall n\in\mathbb{N}:&&p(n)&\iff\sum^n_{i=0}a_i=\sum^{n+1}_{i=1}a_{i-1}\\
&&&\implies \left(\sum^n_{i=0}a_i\right)+a_{n+1}=\left(\sum^{n+1}_{i=1}a_{i-1}\right)+a_{(n+2)-1}\\
&&&\implies \left(a_0+\sum^n_{i=1}a_i\right)+a_{n+1}=\sum^{n+2}_{i=1}a_{i-1}\\
&&&\implies a_0+\left(\left(\sum^n_{i=1}a_i\right)+a_{n+1}\right)=\sum^{n+2}_{i=1}a_{i-1}\\
&&&\implies a_0+\left(\sum^{n+1}_{i=1}a_i\right)=\sum^{n+2}_{i=1}a_{i-1}\\
&&&\implies \sum^{n+1}_{i=0}a_i=\sum^{n+2}_{i=1}a_{i-1}\\
&&&\iff p(n+1)\\
\hline
\forall n\in\mathbb{N}:&&p(n)&\implies p(n+1)
\end{align*}
$${:.math}

Por lo tanto, \\(\forall n\in\mathbb{N}:\displaystyle\sum^n_{i=0}a_i=\displaystyle\sum^{n+1}\_{i=1}a_{i-1}\\).

#### Demostración

* Para \\(n=1\\) 
  
  $$\begin{align*}
    \sum^1_{𝑖=0} a_i&=a_0+a_1\\[0.5em]
    \sum^{1+1}_{i=1}a_{i-1}&=\sum^2_{i=1}a_{i-1}\\
    &=a_{1−1}+a_{2−1}\\
    &=a_0+a_1\\
    \hline
    \sum^1_{𝑖=0} a_i&=\sum^{1+1}{i=1}a_{i-1}
  \end{align*}$$

* Para \\(n\ge1\\)
  
  **Hipótesis de inducción**

  $$\sum^n_{i=0}a_i=\sum^{n+1}_{i=1}a_{i-1}$${:.math}

  Entonces... **P.D.**

  $$\sum^{n+1}_{i=0}a_i=\sum^{n+2}_{i=1}a_{i-1}$${:.math}
  
  Partiendo del primer miembro… 
  
  $$\begin{align*}
  \sum^{n+1}_{i=0}a_i&=\sum^{n}_{i=0}a_i+a_{n+1}&\text{Por propiedad de sumatorias: }\sum^{n+1}_{i=1}a_i&=\sum^{n}_{i=1}a_i+a_{n+1}\\[0.5em]
  \sum^{n}_{i=0}a_i+a_{n+1}&=\sum^{n+1}_{i=1}a_{i-1}+a_{n+1}&\text{Por hipótesis: }\sum^n_{i=0}a_i&=\sum^{n+1}_{i=1}a_{i-1}\\
  \end{align*}
  $${:math}
  
  Obsérvese que el último elemento de la suma \\(\displaystyle\sum^{n+1}\_{i=1}a\_{i-1}\\) es \\(a\_{(𝑛+1)−1}=a\_n\\) y su sucesor se puede incorporar a la suma cuando \\(\displaystyle\sum^{n+2}\_{i=1}a\_{i-1}\\), ya que su último elemento será  \\(a\_{(n+2)−1}=a\_{n+1}\\), bajo esta premisa tenemos entonces que... 

  $$\begin{align*}
  \sum^{n+1}_{i=1}a_{i-1}+a_{n+1}&=\sum^{n+2}_{i=1}a_{i-1}&\text{Por propiedad de sumatorias: }\sum^{n+1}_{i=1}a_i&=\sum^{n}_{i=1}a_i+a_{n+1}\\[0.5em]
  \sum^{n+1}_{i=1}a_{i-1}+a_{n+1}&=\sum^{n+2}_{i=1}a_{i-1}
  \end{align*}
  $${:math}

***Quod erat demonstrandum.***