---
layout: default
title: Enero 2021
nav_order: 2021-01
description: "Trabajo olímpico del mes de enero"
last_modified_date: 2020-09-28T13:00:00+0000
grand_parent: Olimpiadas
parent: Olimpiadas 2021
---

# <span class="deg-sitio deg-sitio-texto">Enero 2021</span><i class="jpa-anim-rel-fire jpa-2em"></i>
{:.fs-9 .no-toc}

¡Comencemos!
{:.fs-6 .fw-300}

---

## <span class="deg-sitio deg-sitio-texto">Geometría</span>

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2020 12 28 G1</span>
{: .no_toc}

<!--VMO 2021 P7 Vietnam National Olympiad https://artofproblemsolving.com/community/c6h2389840_concyclic_and_collinear_wanted_5_circles_related_starting_with_circumcircle -->


Sea \\(ABC\\) un triángulo inscrito en el círculo \\(\Gamma\\). Sea \\(D\\) la intersección de las dos rectas tangentes a \\(\Gamma\\) en \\(B\\) y \\(C\\). El círculo que pasa por \\(A\\) y es tangente a \\(BC\\) en \\(B\\) intersecta a la mediana del triángulo \\(ABC\\) que pasa por \\(A\\) en \\(G\\). Las rectas \\(BG\\), \\(CG\\) intersectan a \\(CD\\) y \\(BD\\) en \\(E\\) y \\(F\\), respectivamente.

>**a.** La línea que pasa a través de los puntos medios de \\(BE\\) y \\(CF\\) corta a \\(BF\\) y \\(CE\\) en \\(M\\) y \\(N\\), respectivamente. Pruebe que los puntos \\(A\\), \\(D\\), \\(M\\) y \\(N\\) pertenecen al mismo círculo.

>**b.** \\(AD\\) y \\(AG\\) intersectan a los circuncírculos de los triángulos \\(DBC\\) y \\(GBC\\) en \\(H\\) y \\(K\\), respectivamente. Las mediatrices de los segmentos \\(HK\\), \\(HE\\) y \\(HF\\) cortan a \\(BC\\), \\(CA\\) y \\(AB\\) en \\(R\\), \\(P\\) y \\(Q\\), respectivamente. Pruebe que los puntos \\(P\\), \\(Q\\) y \\(R\\) son colineales.

[AoPS](https://artofproblemsolving.com/community/c6h2389840_concyclic_and_collinear_wanted_5_circles_related_starting_with_circumcircle){:.no-imprimir}

#### Solución Parte a.



## <span class="deg-sitio deg-sitio-texto">Teoría de números</span>

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2020 12 28 N1</span>
{: .no_toc}
<!-- https://artofproblemsolving.com/community/c6h2116516p15367280 -->

Encuentra el número de pares de números primos \\((p,q)\\) que satisfacen la siguiente desigualdad: 

$$\dfrac {51}{100} <\dfrac {1}{p}+\dfrac {1}{q} <\dfrac {5}{6}$$
{:.math}

[AoPS](https://artofproblemsolving.com/community/c6h2116516p15367280){:.no-imprimir}

#### Solución

Si ambos primos son mayores o iguales a 4, la desigualdad \\(\frac {51}{100} <\frac {1}{p}+\frac {1}{q}\\) no se cumple, pues \\(\frac {1}{p}+\frac{1}{q}\\) \\(<\frac {1}{4}+\frac {1}{4}\\) \\(<\frac{1}{2}<\frac{51}{100}\\). Entonces, **SPG** suponemos que \\(p\le q\\). Esto significa que existen dos casos:

1. \\(p=2\\)
   
   Entonces \\(\frac{1}{100}<\frac{1}{q}<\frac{1}{3}\\), es decir: \\(100>q>3\\). Dado que entre 1 y 100 hay exactamente 25 números primos, \\(q\\) puede tomar 23 valorres distintos (pues se omiten 2 y 3). 
2. \\(p=3\\)
   
   En este caso  \\(\frac{1}{6}\\)\\(<\frac{51}{100}-\frac{1}{3}\\)\\(=\frac{153-100}{300}\\)\\(=\frac{53}{300}\\)\\(<\frac{1}{q}<\frac{1}{2}\\), es decir, \\(6> q\ge 3\\). En este caso \\(q\\) puede tomar dos valores distintos (3 y 5).

Dado que hemos supuesto que \\(p\le q\\), duplicamos los pares \\((p,q)\\) excepto \\((3,3)\\) (para considerar los casos donde \\(p>q\\)), y obtenemos que hay 49 pares que satisfacen la desigualdad.

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2020 12 28 N2</span>
{: .no_toc}

<!-- 2006 Korea National Olympiad #3 https://artofproblemsolving.com/community/c6h1610479p10054906

https://artofproblemsolving.com/community/c629318_2006_korea_national_olympiad -->

Dados tres enteros positivos \\(a\\), \\(b\\) y \\(c\\), si \\(MCD(a,b,c)=1\\) y \\(a^2+b^2+c^2\\)\\(=2(ab+bc+ca)\\), demuestre que \\(a\\), \\(b\\) y \\(c\\) son cuadrados perfectos.

[AoPS](https://artofproblemsolving.com/community/c6h1610479p10054906){:.no-imprimir}

[AoPS](https://artofproblemsolving.com/community/c629318_2006_korea_national_olympiad){:.no-imprimir}

#### Solución 1

Podemos realizar las siguientes factorizaciones:

$$
\begin{align*}
   (a+b-c)^2&= 4ab\\
   (a-b+c)^2&= 4ac\\
   (-a+b+c)^2&= 4bc
\end{align*}
$$
{:.math}

Lo anterior nos lleva a concluir que \\(ab\\), \\(bc\\) y \\(ca\\) son cuadrados perfectos. *SPG*, suponemos que \\(MCD(a,b)>1\\). Esto significa que existe un número primo \\(p\\) que divide a \\(a\\) y \\(b\\), es decir, \\(p\|ab\\), lo que implica \\(p\|(a+b-c)^2\\), es decir, \\(p\|a+b-c\\). Además,\\(p\|a+b\\), por lo que \\(p\|c\\), lo cual implica que \\(p\|MCD(a,b,c)=1\\), una contradicción.

Esto se puede hacer de manera análoga con con cualquier permutación de los tres enteros, por lo que \\(MCD(a,b)\\) \\(=MCD(b,c)\\) \\(=MCD(c,a)=1\\), lo que implica que \\(a\\), \\(b\\) y \\(c\\) son cuadrados perfectos.

#### Solución 2

En las siguientes ecuaciones cuadráticas (respecto a \\(a\\), \\(b\\) y \\(c\\), respectivamente)

$$
\begin{align*}
   a^2-2(b+c)a+(b-c)^2&= 0\\
   b^2-2(c+a)b+(c-a)^2&= 0\\
   c^2-2(a+b)c+(a-b)^2&= 0
\end{align*}
$$
{:.math}

Los determinantes son

$$
\begin{align*}
   4(b+c)^2-4(b-c)^2&= 16bc\\
   4(c+a)^2-4(c-a)^2&= 16ca\\
   4(b+c)^2-4(b-c)^2&= 16bc
\end{align*}
$$
{:.math}

Dado que en las ecuaciones, el coeficiente del término de segundo grado es 1 y el coeficiente del término de primer grado es par, la mitad de la raíz del determinante debe ser entera, es decir, la cuarta parte del determinante debe ser un cuadrado perfecto.

Por ejemplo 

$$
\begin{align*}
   a^2-2(b+c)a+(b-c)^2&= 0\\
   \implies a&=\frac{2(b+c)\pm \sqrt{16bc}}{2}\\
   \implies a&=b+c\pm \sqrt{\frac{16bc}{4}}\\
   &=b+c\pm \sqrt{4bc}
\end{align*}
$$
{:.math}

Dado que \\(a\\), \\(b\\) y \\(c\\) son enteros positivos, \\(4bc\\) debe ser un cuadrado perfecto, por lo tanto, \\(bc\\) es un cuadrado perfecto. De manera análoga, \\(ca\\) y \\(ab\\) son cuadrados perfectos, y se demuestra que \\(a\\), \\(b\\) y \\(c\\) son coprimos par a par como en la solución 1 para concluir.