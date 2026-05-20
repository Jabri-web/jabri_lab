# Jabri_lab — Jabri's Laboratory for Computational Proofs

Public verification of computational results using Zx function.  
One idea per file. Run it. Check it. Break it.

**Author:** Eng. Abdulla Al-Jabri - مهندس عبدالله الجبري  
**Independent Researcher**  
**Location:** Sana'a, Yemen  
**Contact:** jabri62018@gmail.com

## Core Model

This repo implements the functions used in the Zx verification work.  
All results come from zeros of the Zx function and its derivatives.

![Model Equations](Equations.png)

### Equations Set
Planck units: $x_p = 21.0$

$$
\begin{aligned}
Z(x) &= \exp(-x/x_p) \cdot \exp(-5\ln(x)) \cdot \ln(x) \cdot \sin\left(\frac{2\pi}{x}\right) \\
A(x) &= \left(\frac{x}{x_p}\right)^2 \exp(-x/x_p) \\
C(x) &= 1 - Z(x) - A(x) \\
Z_t &= Z + C + A = 1 \\
C_{calc} &= 0.5 \cdot \gamma^2 \cdot \text{Re}\left[\frac{Z'''( \gamma)}{Z(\gamma)}\right]
\end{aligned}
$$

Where $\gamma$ are the non-trivial zeros of Zx(t).

## Results

Each experiment has 3 files in the root:
- `Name_table.csv` - numerical results and matches
- `Name_figure.png` - plot of results  
- `Name.ipynb` - reproducible code

### Core Experiments

#### 1. Zx_Planck
Connects Planck time to Hubble tension using Zx zeros.
- [Table](Zx_Planck_table.csv) | [Figure](Zx_Planck_figure.png) | [Notebook](Zx_Planck.ipynb)

#### 2. Zx_Spacetime
Reproduces spacetime constants: t_P, l_P, h, G, c.
- [Table](Zx_Spacetime_table.csv) | [Figure](Zx_Spacetime_figure.png) | [Notebook](Zx_Spacetime.ipynb)

#### 3. Zx_DarkEnergy
Dark energy density from Z''' term. Target: 6.9e-27 kg/m³.
- [Table](Zx_Darkenergy_table.csv) | [Figure](Zx_Darkenergy_figure.png) | [Notebook](Zx_Darkenergy.ipynb)

### Additional Experiments

#### 4. Zx_5
- [Table](Zx_5_table.csv) | [Figure](Zx_5_figure.png) | [Notebook](Zx_5.ipynb)

#### 5. Zx_all
- [Table](Zx_all_table.csv) | [Figure](Zx_all_figure.png) | [Notebook](Zx_all.ipynb)

#### 6. Zx_28
- [Table](Zx_28_table.csv) | [Figure](Zx_28_figure.png) | [Notebook](Zx_28.ipynb)

#### 7. Zx_Periodic
- [Table](Zx_Periodic_table.csv) | [Figure](Zx_Periodic_figure.png) | [Notebook](Zx_Periodic.ipynb)

#### 8. Zx_Hubble
- [Table](Zx_Hubble_table.csv) | [Figure](Zx_Hubble_figure.png) | [Notebook](Zx_Hubble.ipynb)

#### 9. Zx_gravity
- [Table](Zx_gravity_table.csv) | [Figure](Zx_gravity_figure.png) | [Notebook](Zx_gravity.ipynb)

## How to Verify

1. Open any `.ipynb` file in Google Colab or Jupyter.
2. Run all cells. Zero input needed.
3. Check the `Log Diff` column in the table. Values < 0.01 are strong matches.
4. Download the CSV and PNG for your own analysis.

## Repository Structure
