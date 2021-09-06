---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 04 30 Ejercicios Números Complejos
nav_order: 2021-04-30
description: "Inducción"
last_modified_date: 2021-04-30T18:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Ejercicios&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>
{:.fs-9}


### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Si \\(z\\), \\(w\in\mathbb{C}\\) y \\(w\ne 0\\), \\(\left\|\frac{z}{w}\right\|=\frac{\|z\|}{\|w\|}\\)

#### Solución 

Como \\(w\ne 0\\), existe su inverso multiplicativo. Por tanto:

$$\begin{align*}
\left|\frac{z}{w}\right|&=\left|z\:\frac{1}{w}\right|\\
&=\left|z\right|\:\left|\frac{1}{w}\right|\\
&=\left|z\right|\:\left|w\right|^{-1}\\
&=\frac{\left|z\right|}{\left|w\right|}\\
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

$$\forall z,w\in\mathbb{C}: \left|\left|z\right|-\left|w\right|\right|\le \left|z-w\right|$$

#### Solución 

Dado que \\(\forall c\in\mathbb{C}\\), se cumple que \\(\|c\|\in\mathbb{R}\land\|c\|\ge 0\\), y, para todo \\(r\in\mathbb{R}\\), \\(\|(x,0)\|=\|x\|\\), podemos utilizar las propiedades del valor absoluto en alguna parte, ya que este coincide con el módulo cuando se aplica a un número real.

Primero

$$\begin{align*}
|z-w+w|&\le |z-w|+|w|\\
|z|&\le |z-w|+|w|\\
|z|-|w|&\le |z-w|
\end{align*}
$${:.math}

Después

$$\begin{align*}
|w-z+z|&\le |w-z|+|z|\\
|w|&\le |z-w|+|z|\\
|w|-|z|&\le |z-w|
\end{align*}
$${:.math}

Como

$$|z|-|w|\le |z-w|\land |w|-|z|\le |z-w|$$

Se cumple que \\(\left\|\left\|z\right\|-\left\|w\right\|\right\|\le \left\|z-w\right\|\\).

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

Sean \\(z,w \in\mathbb{C}\\).  Demuestre que

>**a.** \\(\|z+w\|^2+\|z-w\|^2=2(\|z\|^2+\|w\|^2)\\)
>
>**b.** 

$$|z+w|^2=|z|^2+|w|^2\iff \Im\left(\frac{iz}{w}\right)=0\iff |z+w|=|z-w|$${:.math}

#### Solución a

$$\begin{align*}
|z+w|^2+|z-w|^2&=(z+w)\overline{z+w}+(z-w)\overline{z-w}\\
&=(z+w)(\bar{z}+\bar{w})+(z-w)(\bar{z}-\bar{w})\\
&=z\bar{z}+z\bar{w}+w\bar{z}+w\bar{w}+z\bar{z}-z\bar{w}-w\bar{z}+w\bar{w}\\
&=2(z\bar{z}+w\bar{w})\\
&=2(|z|^2+|w|^2)
\end{align*}
$${:.math}

#### Solución b

Primero, verificaremos la equivalencia \\(\|z+w\|^2=\|z\|^2+\|w\|^2\iff\Im\left(\frac{iz}{w}\right)=0\\).

Comenzamos con la implicación \\(\|z+w\|^2=\|z\|^2+\|w\|^2\implies\Im\left(\frac{iz}{w}\right)=0\\), utilizando la propiedad de la parte **a.** Nótese que \\(i=(0,1)\\), por tanto, \\(\bar{i}=\overline{(0,1)}=-i\\)

$$\begin{align*}
|z+w|^2=|z|^2+|w|^2&\implies(z+w)\overline{z+w}=|z|^2+|w|^2\\
&\implies (z+w)(\bar{z}+\bar{w})=|z|^2+|w|^2\\
&\implies z\bar{z}+z\bar{w}+w\bar{z}+w\bar{w}=|z|^2+|w|^2\\
&\implies |z|^2+z\bar{w}+w\bar{z}+|w|^2=|z|^2+|w|^2\\
&\implies z\bar{w}+w\bar{z}=0\\
&\implies z\bar{w}=-w\bar{z}\\
&\implies z\bar{w}=-\frac{i}{i}w\bar{z}\\[1em]
&\implies iz\bar{w}=-i\overline{\bar{w}}\bar{z}\\
&\implies iz\bar{w}=-i\overline{z\bar{w}}\\
&\implies iz\bar{w}=\overline{iz\bar{w}}\\
&\implies iz\bar{w}\in\mathbb{R}\\
\end{align*}
$${:.math}

Duda: ¿\\(w\ne 0\\)?

En tal caso, al dividir  \\(iz\bar{w}\\) entre el número real \\(\|w\|^2\\), obtenemos que \\(\frac{iz}{w}\in\mathbb{R}\\), lo que implica \\(\Im\left(\frac{iz}{w}\right)=0\\). 

De manera análoga, si \\(w\ne 0\\), \\(\Im\left(\frac{iz}{w}\right)=0\\), entonces \\(\frac{iz}{w}\in\mathbb{R}\\). Al multiplicar por \\(\|w\|^2\\), por el axioma de cerradura de los números reales, \\(iz\bar{w}\in\mathbb{R}\\).

Luego

$$\begin{align*}
iz\bar{w}\in\mathbb{R}&\implies iz\bar{w}=\overline{iz\bar{w}}\\
&\implies iz\bar{w}=-i\overline{z\bar{w}}\\
&\implies iz\bar{w}=-i\overline{\bar{w}}\bar{z}\\
&\implies z\bar{w}=-\frac{i}{i}w\bar{z}\\[1em]
&\implies z\bar{w}=-w\bar{z}\\
&\implies z\bar{w}+w\bar{z}=0\\
&\implies |z|^2+z\bar{w}+w\bar{z}+|w|^2=|z|^2+|w|^2\\
&\implies z\bar{z}+z\bar{w}+w\bar{z}+w\bar{w}=|z|^2+|w|^2\\
&\implies (z+w)(\bar{z}+\bar{w})=|z|^2+|w|^2\\
&\implies(z+w)\overline{z+w}=|z|^2+|w|^2\\
&\implies |z+w|^2=|z|^2+|w|^2
\end{align*}
$${:.math}

La equivalencia \\(\|z+w\|^2=\|z\|^2+\|w\|^2\iff \|z+w\|=\|z-w\|\\) se da porque, por el inciso **a,** \\(\|z+w\|^2=\|z\|^2+\|w\|^2\iff\|z+w\|^2=\|z-w\|^2\\). Como \\(\|z+w\|,\|z-w\|\in\mathbb{R}\\) y \\(\|z+w\|,\|z-w\|\ge 0\\), se puede aplicar la siguiente propiedad:

$$\forall a,b\in\mathbb{R}:a,b>0\implies (a^2=b^2\iff a=b)$${:.math}

Entonces \\(\|z+w\|^2=\|z-w\|^2\iff \|z+w\|=\|z-w\|\\). Luego, se cumple que \\(\|z+w\|^2=\|z\|^2+\|w\|^2\iff \|z+w\|=\|z-w\|\\).

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

Sean \\(a,b\in\mathbb{C}\\). Si \\(\|z\|=1\\), entonces

$$\left|\frac{az+b}{\overline{b}z+\overline{a}}\right|=1$${:.math}

#### Solución a
Como \\(\|z\|=1\\), \\(\|z\|^2=1\\)

$$\begin{align*}
|z|^2=1&\implies |z|^2\ne 0\\
&\implies z\overline{z}\ne 0\\
&\implies z\ne0\land\overline{z}\ne 0
\end{align*}
$${:.math}

Luego, podemos dividir entre \\(\overline{z}\\).

$$\begin{align*}
|z|^2=1&\implies z\overline{z}=1\\
&\implies z=\frac{1}{\overline{z}}\\
&\implies z=\overline{\frac{1}{z}}\\
\end{align*}
$${:.math}

Entonces:

$$\begin{align*}
\left|\frac{az+b}{\overline{b}z+\overline{a}}\right|&=\left|\frac{az+b}{\overline{b}\overline{\left(\frac{1}{z}\right)}+\overline{a}}\right|\\
&=\left|\frac{az+b}{\overline{\frac{b}{z}}+\overline{a}}\right|\\
&=\left|\frac{az+b}{\overline{\frac{b}{z}+a}}\right|\\
&=\left|\frac{az+b}{\overline{\frac{b+az}{z}}}\right|\\
&=\left|\frac{az+b}{\overline{az+b}\overline{\left(\frac{1}{z}\right)}}\right|\\
&=\left|\frac{az+b}{\overline{az+b}\left(\overline{z}\right)^{-1}}\right|\\
&=\left|\overline{z}\:\frac{az+b}{\overline{az+b}}\right|\\
&=\left|\overline{z}\right|\:\left|\frac{az+b}{\overline{az+b}}\right|\\
&=\left|z\right|\:\left|\frac{az+b}{\overline{az+b}}\right|\\
&=1\:\left|az+b\right|\left|\overline{az+b}\right|^{-1}\\
&=1\:\left|az+b\right|\left|az+b\right|^{-1}\\
&=1
\end{align*}
$${:.math}