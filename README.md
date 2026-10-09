# Manuscript data

Quantum Monte Carlo (QMC) results for the normalized partition function
`R = Z(i g) / Z(0)`. Each CSV file gives the averaged values and their errors
at the sampled imaginary-source values `g`.

The folders are named by model and coupling. Within each folder, `L_008`
means an 8 × 8 lattice. The inverse temperature is `beta = L/2`.

| File | Channel |
| --- | --- |
| `AFM_hIm.csv` | Néel (AFM) |
| `PSS_etae.csv` | Plaquette-singlet solid (PSS) |
| `VBS_bond_xi_x.csv` | Bond-supported columnar VBS |
| `VBS_interaction_zeta.csv` | Interaction-supported columnar VBS |

The columns are:

| Column | Meaning |
| --- | --- |
| `g` | Amplitude of the imaginary source `i g`. |
| `ReR`, `ImR` | Mean real and imaginary parts of `R`. |
| `ReR_error`, `ImR_error` | Standard errors of these means. |
| `N_bins`, `N_replicas` | Numbers of contributing bins and replica files. |
| `V` | `-ln(abs(ReR + i*ImR))`. |
| `V_error` | Uncertainty of `V`. |
