---
layout: default
tema: Morado
tema_oscuro: MoradoOscuro
title: 2021 03 20 Problema de Inducción
nav_order: 2021-08-11
description: "Inducción"
last_modified_date: 2021-03-20T18:00:00+0000
grand_parent: Introducción a las Estructuras Algebraicas
parent: Ejercicios Introducción a las Estructuras Algebraicas
---

# Ejercicios de propiedades de&nbsp;<span class="deg-sitio deg-sitio-texto">\\(\mathbb{Z}\\)</span>
{:.fs-9}

11 de Agosto de 2021.
{:.fs-6 .fw-300}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

La suma es asociativa.

#### Demostración

$$
\begin{align*}
    &[a,b]+\left([c,d]+[e,f]\right)=\left([a,b]+[c,d]\right)+[e,f]\\
    &\iff [a,b]+[c+e,d+f]=[a+c,b+d]+[e,f]\\
    &\iff [a+(c+e),b+(d+f)]=[(a+c)+e,(b+d)+f]\\
    &\iff (a+(c+e))+(b+(d+f))=((a+c)+e)+((b+d)+f)\\
    &\iff ((a+c)+e)+((b+d)+f)=((a+c)+e)+((b+d)+f)\\
\end{align*}
$${:.math}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

El producto es conmutativo.

#### Demostración

$$
\begin{align*}
    [a,b]\cdot[c,d]=[c,d]\cdot[a,b]&\iff [ac+bd,ad+bc]=[ca+db,cb+da]\\   
    &\iff (ac+bd)+(cb+da)=(ca+db)+(ad+bc)\\
    &\iff (ac+bd)+(bc+ad)=(ac+bd)+(ad+bc)\\
    &\iff (ac+bd)+(ad+bc)=(ac+bd)+(ad+bc)
\end{align*}
$${:.math}

### Problema&nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

El producto es asociativo.

#### Demostración

$$
\begin{align*}
    &[a,b]\cdot([c,d]\cdot[e,f])=([a,b]\cdot[c,d])\cdot[e,f])\\   
    &\iff [a,b]\cdot[ce+df,cf+de]=[ac+bd,ad+bc]\cdot[e,f]\\
    &\iff [a(ce+df)+b(cf+de),a(cf+de)+b(ce+df)]\\
    &\phantom{\iff}\,=[(ac+bd)e+(ad+bc)f,(ac+bd)f+(ad+bc)e]\\
    &\iff a(ce+df)+b(cf+de)+(ac+bd)f+(ad+bc)e\\
    &\phantom{\iff}\,=(ac+bd)e+(ad+bc)f+a(cf+de)+b(ce+df)\\
    &\iff ace+adf+bcf+bde+acf+bdf+ade+bce\\
    &\phantom{\iff}\,=ace+bde+adf+bcf+acf+ade+bce+bdf\\
    &\iff ace+adf+bcf+bde+acf+bdf+ade+bce\\
    &\phantom{\iff}\,=ace+adf+bcf+bde+acf+bdf+ade+bce\\
\end{align*}
$${:.math}



