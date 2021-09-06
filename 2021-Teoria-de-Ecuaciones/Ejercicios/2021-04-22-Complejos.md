---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 04 22 Números complejos
nav_order: 2021-01-18
description: "Inducción"
last_modified_date: 2021-03-20T18:00:00+0000
grand_parent: Teoría de Ecuaciones
parent: Ejercicios Teoría de Ecuaciones
---

# Problemas de&nbsp;<span class="deg-sitio deg-sitio-texto">\\(\mathbb{C}\\)</span>
{:.fs-9}

## Introducción a &nbsp;<span class="deg-sitio deg-sitio-texto">\\(\mathbb{C}\\)</span>

* El conjunto de los números complejos se define como el conjunto conformado por pares ordenados de  números reales.

$$\mathbb{C}=\{(x,y)|x,y\in\mathbb{R}\}$${:.math}

* Sean \\((x_1,y_1),\:(x_2,y_2)\in\mathbb{C}\\) y \\(\alpha\in\mathbb{R}\\).  Se define
  * La relación de igualdad:
  
  $$(x_1,y_1)=(x_2,y_2)\iff x_1=x_2\land y_1=y_2$${:.math} 

  * La operación suma:

  $$(x_1,y_1)+(x_2,y_2)=(x_1+x_2,y_1+y_2)$${:.math}

  * La operación producto:

  $$(x_1,y_1)(x_2,y_2)=(x_1x_2-y_1y_2,x_1y_2+x_2y_1)$${:.math}

  * El producto de un número real y un número complejo 
  
  $$\alpha(x_1,y_1)=(\alpha x_1,\alpha y_1)$${:.math}

En los siguientes problemas, se utilizarán \\(z_1,z_2,z_3\in\mathbb{C}\\), donde \\(z_1=(a_1,a_2)\\), \\(z_2=(b_1,b_2)\\) y \\(z_3=(c_1,c_2)\\). Se utilizarán las propiedades de los números reales para demostrar las propiedades de los números complejos.

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">1</span> Leyes de Cerradura

\\(z_1+z_2,z_1z_2\in\mathbb{C}\\).

#### Solución

Primero, la suma de dos complejos 

$$\begin{align*}
z_1,z_2\in\mathbb{C}&\implies a_1,a_2,b_1,b_2\in\mathbb{R}\\
&\implies a_1+b_1, a_2+b_2\in\mathbb{R}\\
&\implies z_1+z_2\in\mathbb{C}
\end{align*}
$${:.math}

Después, el producto de dos complejos.

$$\begin{align*}
z_1,z_2\in\mathbb{C}&\implies a_1,\:a_2,\:b_1,\:b_2\in\mathbb{R}\\
&\implies a_1b_1,\:a_2b_2,\:a_1b_2,\:b_1a_2\in\mathbb{R}\\
&\implies a_1b_1,\:-a_2b_2,\:a_1b_2+b_1a_2\in\mathbb{R}\\
&\implies a_1b_1-a_2b_2,\:a_1b_2+b_1a_2\in\mathbb{R}\\
&\implies z_1z_2\in\mathbb{C}
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">2</span> Leyes conmutativas

\\(z_1+z_2=z_2+z_1, z_1z_2=z_2z_1\\).

#### Solución

Primero, la suma de dos complejos 

$$\begin{align*}
&z_1+z_2=z_2+z_1\\
&\iff (a_1,a_2)+(b_1,b_2)=(b_1,b_2)+(a_1,a_2)\\
&\iff (a_1+b_1,a_2+b_2)=(b_1+a_1,b_2+a_2)\\
&\iff a_1+b_1=b_1+a_1\land a_2+b_2=b_2+a_2\\
\hline
&z_1+z_2=z_2+z_1
\end{align*}
$${:.math}

Después, el producto de dos complejos.

$$\begin{align*}
&z_1z_2=z_2z_1\\
&\iff (a_1,a_2)(b_1,b_2)=(b_1,b_2)(a_1,a_2)\\
&\iff (a_1b_1-a_2b_2,a_1b_2+a_2b_1)=(b_1a_1-b_2a_2,b_1a_2+b_2a_1)\\
&\iff a_1b_1-a_2b_2=b_1a_1-b_2a_2\land a_1b_2+a_2b_1=b_1a_2+b_2a_1\\
&\iff a_1b_1-a_2b_2=a_1b_1-a_2b_2\land a_1b_2+a_2b_1=a_2b_1+a_1b_2\\
&\iff a_1b_1-a_2b_2=a_1b_1-a_2b_2\land a_1b_2+a_2b_1=a_1b_2+a_2b_1\\
\hline
&z_1z_2=z_2z_1
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">3</span> Leyes asociativas

\\((z_1+z_2)+z_3=z_1+(z_2+z_3)\\), \\((z_1z_2)z_3=z_1(z_2z_3)\\)

#### Solución

Primero, la propiedad bajo la suma

$$\begin{align*}
&(z_1+z_2)+z_3=z_1+(z_2+z_3)\\
&\iff ((a_1,a_2)+(b_1,b_2))+(c_1,c_2)=(a_1,a_2)+((b_1,b_2)+(c_1,c_2))\\
&\iff (a_1+b_1,a_2+b_2)+(c_1,c_2)=(a_1,a_2)+(b_1+c_1,b_2+c_2)\\
&\iff ((a_1+b_1)+c_1,(a_2+b_2)+c_2)=(a_1+(b_1+c_1),a_2+(b_2+c_2))\\
&\iff (a_1+b_1)+c_1=a_1+(b_1+c_1)\land (a_2+b_2)+c_2=a_2+(b_2+c_2)\\
\hline
&(z_1+z_2)+z_3=z_1+(z_2+z_3)
\end{align*}
$${:.math}

Después, el producto

$$\begin{align*}
&(z_1z_2)z_3=z_1(z_2z_3)\\
&\iff ((a_1,a_2)(b_1,b_2))(c_1,c_2)=(a_1,a_2)((b_1,b_2)(c_1,c_2))\\
&\iff (a_1b_1-a_2b_2,a_1b_2+a_2b_1)(c_1,c_2)=(a_1,a_2)(b_1c_1-b_2c_2,b_1c_2+b_2c_1)\\[1em]

&\iff ((a_1b_1-a_2b_2)c_1-(a_1b_2+a_2b_1)c_2,(a_1b_1-a_2b_2)c_2+(a_1b_2+a_2b_1)c_1)\\
&\phantom{\iff}=a_1(b_1c_1-b_2c_2)-a_2(b_1c_2+b_2c_1), a_1(b_1c_2+b_2c_1)+a_2(b_1c_1-b_2c_2)\\

&\iff (a_1b_1-a_2b_2)c_1-(a_1b_2+a_2b_1)c_2=a_1(b_1c_1-b_2c_2)-a_2(b_1c_2+b_2c_1)\\
&\phantom{\iff}\land (a_1b_1-a_2b_2)c_2+(a_1b_2+a_2b_1)c_1=a_1(b_1c_2+b_2c_1)+a_2(b_1c_1-b_2c_2)\\

&\iff (a_1b_1c_1-a_2b_2c_1)-(a_1b_2c_2+a_2b_1c_2)=(a_1b_1c_1-a_1b_2c_2)-(a_2b_1c_2+a_2b_2c_1)\\
&\phantom{\iff}\land (a_1b_1c_2-a_2b_2c_2)+(a_1b_2c_1+a_2b_1c_1)=(a_1b_1c_2+a_1b_2c_1)+(a_2b_1c_1-a_2b_2c_2)\\

&\iff a_1b_1c_1-a_2b_2c_1-a_1b_2c_2+a_2b_1c_2=a_1b_1c_1-a_2b_2c_1-a_1b_2c_2-a_2b_1c_2\\
&\phantom{\iff}\land -a_2b_2c_2+(a_1b_1c_2+a_1b_2c_1+a_2b_1c_1)=(a_1b_1c_2+a_1b_2c_1+a_2b_1c_1)-a_2b_2c_2\\

&\iff a_1b_1c_1-a_2b_2c_1-a_1b_2c_2+a_2b_1c_2=a_1b_1c_1-a_2b_2c_1-a_1b_2c_2-a_2b_1c_2\\
&\phantom{\iff}\land -a_2b_2c_2+(a_1b_1c_2+a_1b_2c_1+a_2b_1c_1)=-a_2b_2c_2+a_1b_1c_2+a_1b_2c_1+a_2b_1c_1\\
\hline
&(z_1z_2)z_3=z_1(z_2z_3)
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">4</span> Ley distributiva

\\((z_1+z_2)z_3=z_1z_3+z_2z_3\\)

#### Solución

$$\begin{align*}
&(z_1+z_2)z_3=z_1z_3+z_2z_3\\
&\iff (a_1+b_1,a_2+b_2)(c_1,c_2)\\
&\phantom{\iff}=(a_1c_1-a_2c_2,a_1c_2+a_2c_1)+(b_1c_1-b_2c_2,b_1c_2+b_2c_1)\\

&\iff ((a_1+b_1)c_1-(a_2+b_2)c_2,(a_1+b_1)c_2+(a_2+b_2)c_1)\\
&\phantom{\iff}=(a_1c_1-a_2c_2+b_1c_1-b_2c_2,a_1c_2+a_2c_1+b_1c_2+b_2c_1)\\

&\iff (a_1+b_1)c_1-(a_2+b_2)c_2=a_1c_1-a_2c_2+b_1c_1-b_2c_2\\
&\phantom{\iff}=(a_1+b_1)c_2+(a_2+b_2)c_1=a_1c_2+a_2c_1+b_1c_2+b_2c_1\\

&\iff (a_1b_1c_1-a_2b_2c_1)-(a_1b_2c_2+a_2b_1c_2)=(a_1b_1c_1-a_1b_2c_2)-(a_2b_1c_2+a_2b_2c_1)\\
&\phantom{\iff}\land (a_1b_1c_2-a_2b_2c_2)+(a_1b_2c_1+a_2b_1c_1)=(a_1b_1c_2+a_1b_2c_1)+(a_2b_1c_1-a_2b_2c_2)\\

&\iff a_1b_1c_1-a_2b_2c_1-a_1b_2c_2+a_2b_1c_2=a_1b_1c_1-a_2b_2c_1-a_1b_2c_2-a_2b_1c_2\\
&\phantom{\iff}\land -a_2b_2c_2+(a_1b_1c_2+a_1b_2c_1+a_2b_1c_1)=(a_1b_1c_2+a_1b_2c_1+a_2b_1c_1)-a_2b_2c_2\\

&\iff a_1b_1c_1-a_2b_2c_1-a_1b_2c_2+a_2b_1c_2=a_1b_1c_1-a_2b_2c_1-a_1b_2c_2-a_2b_1c_2\\
&\phantom{\iff}\land -a_2b_2c_2+(a_1b_1c_2+a_1b_2c_1+a_2b_1c_1)=-a_2b_2c_2+a_1b_1c_2+a_1b_2c_1+a_2b_1c_1\\
\hline
&(z_1+z_2)z_3=z_1z_3+z_2z_3
\end{align*}
$${:.math}

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">5</span> Existencia de neutro aditivo y neutro multiplicativo



#### Solución

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">6</span>


#### Solución

### Problema &nbsp;<span class="deg-sitio deg-sitio-texto">7</span>

#### Solución