---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: 2021 02 19 ¿Se puede considerar a \(\mathbb{R}^2\) campo con operaciones par a par?
nav_order: 2021-02-10
description: "Página de la materia"
last_modified_date: 2021-02-19T14:00:00+0000
grand_parent: Problemas de Matemáticas Básicas
parent: Apuntes Problemas de Matemáticas Básicas
---

# ¿Se puede considerar a&nbsp;<span class="deg-sitio deg-sitio-texto">\\(\mathbb{R}^2\\)</span> campo con operaciones par a par?
{:.fs-9}

19 de febrero de 2021.
\\(\def\Real{\mathbb{R}} \def\Vec#1{\boldsymbol{#1}}\\)
{:.fs-6 .fw-300}

Sean \\(\Vec{u},\Vec{v}\in\Real^2\\), tales que \\(\Vec{u}=(x_0,y_0)\\) y \\(\Vec{v}=(x_1,y_1)\\).

Por definición de \\(\Real^2\\), \\(\Vec{u}\in\Real^2\iff x_0,y_0\in\Real\\).

### Definiciones

* Igualdad: \\(\Vec{u}=\Vec{v}\iff x_0=x_1\land y_0=y_1\\)
* Suma \\(\Vec{u}+\Vec{w}=(x_0+x_1,y_0+y_1)\\),
* Producto \\(\Vec{u}\Vec{v}=(x_0x_1,y_0y_1)\\) y
* \\(\Vec{1}=(1,1)\\) y \\(\Vec{0}=(0,0)\\).

### ¿Este conjunto, con las operaciones definidas, satisface los axiomas de campo?

Sean \\(\Vec{u},\Vec{v},\Vec{w}\in\Real^2\\), tales que \\(\Vec{u}=(x_0,y_0)\\), \\(\Vec{v}=(x_1,y_1)\\) y \\(\Vec{w}=(x_2,y_2)\\).

* Ley de cerradura
  
  \\(\Vec{u+v}\in\Real^2\iff x_0+x_1,y_0+y_1\in\Real\\).

  \\(\Vec{uv}\in\Real^2\iff x_0x_1,y_0y_1\in\Real\\).
* Leyes conmutativas
  
  \\(\Vec{u}+\Vec{v}=\Vec{v}+\Vec{u}\iff x_0+x_1=x_1+x_0\land y_0+y_1=y_1+y_0\\).

  \\(\Vec{uv}=\Vec{vu}\iff x_0x_1=x_1x_0\land y_0y_1=y_1y_0\\).
* Leyes asociativas
  
  \\(\Vec{u}+(\Vec{v}+\Vec{w})=(\Vec{u}+\Vec{v})+\Vec{w}\iff x_0+(x_1+x_2)=(x_0+x_1)+x_2\land y_0+(y_1+y_2)=(y_0+y_1)+y_2\\).

  \\(\Vec{u}(\Vec{vw})=(\Vec{uv})\Vec{w}\iff x_0(x_1x_2)=(x_0x_1)x_2\land y_0(y_1y_2)=(y_0y_1)y_2\\).

* Ley distributiva
  
  \\(\Vec{u}(\Vec{v}+\Vec{w})=\Vec{u}\Vec{v}+\Vec{u}\Vec{w}\iff x_0(x_1+x_2)=x_0x_1+x_0x_2\land y_0(y_1+y_2)=y_0y_1+y_0y_2\\).

* Existencia de neutro aditivo y multiplicativo
  
  \\(\exists\Vec{0},\Vec{1}\in\Real^2:\Vec{0}\ne\Vec{1}\land\forall \Vec{u}\in\Real^2:\Vec{u}+\Vec{0}=\Vec{u}\land\Vec{u}(\Vec{1})=\Vec{u}\\).

  Esto es cierto, pues siendo \\(\Vec{u}=(x,y)\\), \\(\Vec{0}=(0,0)\\) y \\(\Vec{1}=(1,1)\\), se tiene que \\(\Vec{u}+\Vec{0}=\Vec{u}\iff x+0=x\land y+0=y\\) y \\(\Vec{u}\\:\Vec{1}=\Vec{u}\iff x(1)=x\land y(1)=y\\). Además, \\(0,1\in\Real\\) y \\(\Vec{0}=\Vec{1}\iff 0=1\\).

* Existencia de inversos aditivos y multiplicativos
  
  Si \\(\Vec{u}\in\Real^2\\) y \\(u=(x,y)\\), existe \\(\Vec{u_1}\in\Real^2\\) tal que \\(\Vec{u}+\Vec{u_1}=\Vec{0}\\) y si \\(\Vec{u}\ne\Vec{0}\\), existe \\(u_2\\) tal que \\(\Vec{uu_2}=\Vec{1}\\).

  Eso no es cierto. Si bien \\(\Vec{u_1}=(-x,-y)\\) satisface la condición planteada, \\(x\ne y\land x=0\lor y=0 \implies (x,y)\ne\Vec{0}\land\forall(a,b)\in\Real:\Vec{u}(a,b)=(0,yb)\lor\Vec{u}(a,b)=(xa,0)\\) \\(\implies (x,y)\ne\Vec{0}\land\forall(a,b)\in\Real:\Vec{u}(a,b)\ne\Vec{1}\\). Es decir, existen infinitos elementos de \\(\Real^2\\) distintos al neutro aditivo tales que no tienen inverso multiplicativo.


