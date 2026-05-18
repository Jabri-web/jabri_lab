# Jabri_lib — Jabri's Laboratory for Computational Proofs

One idea per file. Run it. Check it. Break it.  
Public verification of computational results.

## Core Model

This repo implements the functions used in the Zx_28 verification work.

![Model Equations](image/Showing_Equastions.png)
https://github.com/jabri62018/Jabri_lab/blob/Jabri_lab/Equations.png
### Equations

Set Planck units: $x_p = 1.0$

$$
\begin{aligned}
Z(x) &= x^5 \ln(x) \sin\left(\frac{2\pi}{x}\right) e^{-x/x_p} \\
A(x) &= \left(\frac{x}{x_p}\right)^2 e^{-x/x_p} \\
C(x) &= 1 - Z(x) - A(x) \\
Z_t &= Z + C + A = 1
\end{aligned}
$$

## Repository Structure
