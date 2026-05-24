# Jabri_lab — Jabri's Laboratory for Computational Proofs

Public verification of computational results using Zx function.  
One idea per file. Run it. Check it. Break it.

**Author:** Eng. Abdulla Al-Jabri - مهندس عبدالله الجبري  
**Independent Researcher**  
**Location:** Sana'a, Yemen  
**Contact:** jabri62018@gmail.com

## Core Model

This repo implements the functions used in the Zx verification work. All results come from zeros of the Zx function and its derivatives.

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

#### 1. Jabri_Planck
Connects Planck time to Hubble tension using Zx zeros.
- [Notebook](Jabri_Planck.ipynb) | [Table](Jabri_Planck_table.csv) | [Figure](Jabri_Planck_figure.png)

#### 2. Jabri_Spacetime
Reproduces spacetime constants: $t_P, l_P, h, G, c$.
- [Notebook](Jabri_Spacetime.ipynb) | [Table](Jabri_Spacetime_table.csv) | [Figure](Jabri_Spacetime_figure.png)

#### 3. Jabri_Darkenergy
Dark energy density from Z''' term. Target: $6.9 \times 10^{-27}$ kg/m³.
- [Notebook](Jabri_Darkenergy.ipynb) | [Table](Jabri_Darkenergy_table.csv) | [Figure](Jabri_Darkenergy_figure.png)

### Additional Experiments

#### 4. Jabri_5
- [Notebook](Jabri_5.ipynb) | [Table](Jabri_5_table.csv) | [Figure](Jabri_5_figure.png)

#### 5. Jabri_28
- [Notebook](Jabri_28.ipynb) | [Table](Jabri_28_table.csv) | [Figure](Jabri_28_figure.png)

#### 6. Jabri_Periodic
- [Notebook](Jabri_Periodic.ipynb) | [Table](Jabri_Periodic_table.csv)

#### 7. Jabri_Hubble
- [Notebook](Jabri_Hubble.ipynb) | [Table](Jabri_Hubble_table.csv)

#### 8. Jabri_Gravity
- [Notebook](Jabri_Gravity.ipynb)

#### 9. Jabri_all
Master notebook running all experiments.
- [Notebook](Jabri_all.ipynb)

## How to Verify

1. Open any `.ipynb` file in Google Colab or Jupyter.
2. Run all cells. Zero input needed.
3. Check the `Log Diff` column in the table. Values < 0.01 are strong matches.
4. Download the CSV and PNG for your own analysis.

## Repository Structure
