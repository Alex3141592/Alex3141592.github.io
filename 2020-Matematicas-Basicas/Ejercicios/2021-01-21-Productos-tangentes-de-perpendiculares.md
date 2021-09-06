---
layout: default
title: 2021 01 21 Producto de tangentes de rectas y perpendiculares.
nav_order: 2021-01-18
description: "Página de la materia"
last_modified_date: 2021-01-18T15:36:00+0000
grand_parent: Matemáticas Básicas
parent: Ejercicios Matemáticas Básicas
---

# Ejercicio demstración con&nbsp;<span class="deg-sitio deg-sitio-texto">axiomas.</span>
{:.fs-9}

4 de febrero de 2021.
{:.fs-6 .fw-300}

### Ejercicio.

1. Se utiliza la definición.
2. Se multiplica por el neutro multiplicativo.
3. Propiedad del neutro multiplicativo y propiedad distributiva.
4. Existencia de neutros multiplicativos para \\(b\\) y \\(d\\). Propiedad del neutro multiplicativo.
5. Asociativa.
6. Conmutativa
7. Asociativa
8. **3.2.1** 12)
9. Conmutativa
10. Distributiva
11. Definición
12. Conclusión


$$
\begin{align*}
\forall a,b,c,d\in\mathbb{R}:&(b\ne 0\land d\ne 0)\land\frac{a}{b}+\frac{c}{d}=ab^{-1}+cd^{-1}\\
&\implies (b\ne 0\land d\ne 0)\land\left(\frac{a}{b}+\frac{c}{d}\right)1=(ab^{-1}+cd^{-1})1\\

&\implies  (b\ne 0\land d\ne 0)\land\frac{a}{b}+\frac{c}{d}=ab^{-1}\cdot 1+cd^{-1}\cdot 1\\

&\implies \frac{a}{b}+\frac{c}{d}=ab^{-1}(dd^{-1})+cd^{-1}(bb^{-1})\\

&\implies \frac{a}{b}+\frac{c}{d}=a(b^{-1}d)d^{-1}+c(d^{-1}b)b^{-1}\\

&\implies \frac{a}{b}+\frac{c}{d}=a(db^{-1})d^{-1}+c(bd^{-1})b^{-1}\\

&\implies \frac{a}{b}+\frac{c}{d}=(ad)b^{-1}d^{-1}+(cb)d^{-1}b^{-1}\\

&\implies \frac{a}{b}+\frac{c}{d}=(ad)(bd)^{-1}+(cb)(db)^{-1}\\

&\implies \frac{a}{b}+\frac{c}{d}=(ad)(bd)^{-1}+(bc)(bd)^{-1}\\

&\implies \frac{a}{b}+\frac{c}{d}=(ad+bc)(bd)^{-1}\\

&\implies \frac{a}{b}+\frac{c}{d}=\frac{ad+bc}{bd}\\

\hline

\forall a,b,c,d\in\mathbb{R}(b\ne 0\land d\ne 0)&\land\frac{a}{b}+\frac{c}{d}=ab^{-1}+cd^{-1}\implies \frac{a}{b}+\frac{c}{d}=\frac{ad+bc}{bd}
\end{align*}
$$
{:.math}