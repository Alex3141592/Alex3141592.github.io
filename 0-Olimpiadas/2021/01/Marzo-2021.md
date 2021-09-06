---
layout: default
title: Marzo 2021
nav_order: 2021-03
description: "Trabajo olímpico del mes de Marzo"
last_modified_date: 2020-09-28T13:00:00+0000
grand_parent: Olimpiadas
parent: Olimpiadas 2021
---

# <span class="deg-sitio deg-sitio-texto">Marzo 2021</span><i class="jpa-anim-rel-fire jpa-2em"></i>
{:.fs-9 .no-toc}

¡Comencemos!
{:.fs-6 .fw-300}

---

## <span class="deg-sitio deg-sitio-texto">Álgebra</span>

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2021 03 13 A1</span> <span>2016 HMMT (The Harvard-MIT Mathematics Tournament) [Foro HMMT](https://artofproblemsolving.com/community/c129_hmmt)</span>{:.no-imprimir}

Sea \\(x_i\\) una secuencia de números reales para todo \\(i\in\mathbb{N}\\). Si \\(x_1=x_3=1\\), \\(x_{98}=x_{99}\\) y

$$x_{n+3}=x_{n+2}-2x_{n+1}+x_n,$${:.math}

Encuentra el valor de

$$x_1+x_2+...+x_{100}$${:.math}

[AoPS](https://artofproblemsolving.com/community/c1266408h2482669_recursion_with_ngt0)

[AoPS](https://artofproblemsolving.com/community/c129h1359316p7444569)
#### Solución

$$\begin{aligned}
\sum^n_{i=1}x_{i+3}&=\left(\sum^n_{i=1}x_{i+2}\right)+\left(\sum^n_{i=1}-2x_{i+1}\right)+\left(\sum^n_{i=1}x_{i}\right)\\
&=\left(\sum^{n+2}_{i=3}x_{i}\right)-2\left(\sum^{n+1}_{i=2}x_{i}\right)+\left(\sum^n_{i=1}x_{i}\right)\\
&=\left(\sum^{n+2}_{i=3}x_{i}\right)-\left(\sum^{n+1}_{i=2}x_{i}\right)-\left(\left(\sum^{n+1}_{i=2}x_{i}\right)-\left(\sum^n_{i=1}x_{i}\right)\right)\\
&=\left(x_{n+2}+\sum^{n+1}_{i=3}x_{i}\right)-\left(x_2+\sum^{n+1}_{i=3}x_{i}\right)-\left(\left(x_{n+1}+\sum^{n}_{i=2}x_{i}\right)-\left(x_1+\sum^n_{i=2}x_{i}\right)\right)\\
&= x_{n+2}-x_2-x_{n-1}+x_1\\
&=x_{n+2}-x_{n+1}-x_2+x_1
\end{aligned}$${:.math}

Finalmente:

$$\begin{aligned}
\sum^{100}_{i=1}x_{i}&=\left(\sum^3_{i=1}x_{i}\right)+\left(\sum^{100}_{i=4}x_{i}\right)\\
&=x_1+x_2+x_3+\sum^{97}_{i=1}x_{i+3}\\
&=x_1+x_2+x_3+x_{97+2}-x_{97+1}-x_2+x_1\\
&=2x_1+x_3\\
&=3
\end{aligned}$${:.math}

Podemos generalizar el problema de la siguiente manera:

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2021 03 13 A1.1</span>

Sea \\(x_i\\) una secuencia de números reales para todo \\(i\in\mathbb{N}\\). Si \\(k>3\\), \\(x_{k-1}=x_{k-2}\\) y

$$x_{n+3}=x_{n+2}-2x_{n+1}+x_n$${:.math}

Se cumple que

$$\begin{aligned}
\sum^{k}_{i=1}x_{i}&=\left(\sum^3_{i=1}x_{i}\right)+\left(\sum^{k}_{i=4}x_{i}\right)\\
&=x_1+x_2+x_3+\sum^{k-3}_{i=1}x_{i+3}\\
&=x_1+x_2+x_3+x_{k-3+2}-x_{k-3+1}-x_2+x_1\\
&=2x_1+x_3\\
\end{aligned}$${:.math}

Para cualesquiera valores de \\(x_1\\) y \\(x_3\\).

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2021 03 13 A2</span> <span>Latvian TST 2021, D1 P2 (Letonia)</span>{:.no-imprimir}
Sean \\(x\\), \\(y\\), \\(z\\) y \\(a\\) que satisfacen las siguientes igualdades: 

$$ x+y+z = a$${:.math}

$$\frac{1}{x}+\frac{1}{y}+\frac{1}{z}= \frac{1}{a}$${:.math}

Demuestre que al menos uno de los números \\(x\\), \\(y\\) y \\(z\\) es igual a \\(a\\).

[AoPS](https://artofproblemsolving.com/community/c6h2485838p20899251){:no-imprimir}

#### Solución

Sea

$$P(X)=(X+x)(X+y)(X+z)=X^3+aX^2+\frac{p}{a}X+p$${:.math}

donde \\(p=xyz\\).

\\(P(-a)=0\\), lo es decir, \\(-a\\) es una de las raíces de \\(P\\) (las cuales son \\(-x\\), \\(-y\\) y \\(-z\\)), lo que implica lo que se quería demostrar.

#### Solución equivalente
Sea

$$P(X)=(X-x)(X-y)(X-z)=X^3-aX^2+\frac{p}{a}X-p$${:.math}

donde \\(p=xyz\\).

\\(P(a)=0\\), lo es decir, \\(a\\) es una de las raíces de \\(P\\) (las cuales son \\(x\\), \\(y\\) y \\(z\\)), lo que implica lo que se quería demostrar.


## <span class="deg-sitio deg-sitio-texto">Combinatoria</span>

## <span class="deg-sitio deg-sitio-texto">Geometría</span>

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2021 03 13 G1</span>
{: .no_toc}


Dado cualquier vértice \\(V\\) de un prisma rectangular, las diagonales de las tres caras que coinciden en dicho vértice tienen longitudes \\(\sqrt{19}\\), \\(\sqrt{23}\\) y \\(\sqrt{30}\\). Encuentra la longitud del segmento que une a \\(V\\) con el único vértice \\(V^\prime\\) tal que ninguna cara del prisma tiene como vértices a \\(V\\) y \\(V^\prime\\) a la vez.

Escrito de otro modo:

Sean \\(ABCD\\) y \\(EFGH\\) dos caras opuestas del prisma rectangular \\(ABCDEFGH\\), el cual tiene a los segmentos \\(AE\\), \\(BF\\), \\(CG\\) y \\(DH\\) como aristas. Las longitudes de \\(AC\\), \\(CF\\) y \\(FA\\) son \\(\sqrt{19}\\), \\(\sqrt{23}\\) y \\(\sqrt{30}\\), respectivamente. Encuentra la longitud del segmento \\(AG\\).

[AoPS](https://artofproblemsolving.com/community/c1266408h2483226_interesting_algebra__geometry_problem)

#### Solución

Sea tiene que

$$
\begin{align*}
   AG^2&=AE^2+EG^2\\
   &=BF^2+AC^2\\
   &=BA^2+BC^2+BF^2\\
   &=\frac{BA^2+BC^2}{2}+\frac{BC^2+BF^2}{2}+\frac{BF^2+BA^2}{2}\\
   &=\frac{AC^2}{2}+\frac{CF^2}{2}+\frac{FA^2}{2}\\
\end{align*}
$${:.math}

Como las longitudes de \\(AC\\), \\(CF\\) y \\(FA\\) son \\(\sqrt{19}\\), \\(\sqrt{23}\\) y \\(\sqrt{30}\\), respectivamente, por lo que \\(AG^2=36\\), es decir, \\(AG=6\\).

## <span class="deg-sitio deg-sitio-texto">Teoría de números</span>

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2021 03 13 N1</span> <span>2003 AIME I, P1</span>{:.no-imprimir}
{: .no_toc}

Si

$$\frac{((3!)!)!}{3!}=k\cdot n!,$$

donde \\(k\\) y \\(n\\) son números naturales, y \\(n\\) es el mayor natural que satisface la igualdad, encuentra \\(k+n\\).

[AoPS](https://artofproblemsolving.com/wiki/index.php/2003_AIME_I_Problems/Problem_1){:.no-imprimir}

#### Solución

Como 

$$k^\prime\cdot 720!\ge 720!>120\cdot 719!=k\cdot n!$${:.math}

para todo \\(k^\prime\in\mathbb{N}\\), se tiene que \\(n< 720\\). Luego, como \\(n=719\\) es el máximo valor posible, \\(k=120\\) y \\(m+n=839\\)

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2020 12 28 N2</span>

#### Solución 1



## <span class="deg-sitio deg-sitio-texto">Especiales</span>



### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">4</span>
{: .no_toc}


### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">5</span>
{: .no_toc}



### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">6</span>
{: .no_toc}



### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">7</span>
{: .no_toc}
