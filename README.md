# A new perspective for mitigation of SARS-CoV-2 infection: priming the innate immune system for viral attack
## Oren Kolodny, Michael Berger, Marcus W. Feldman, and Yoav Ram
## Open Biology 2020

This repository contains a [Jupyter notebook](notebooks/SEIR.ipynb) used to produce the Figure in the paper.
The notebook contains the model implementation.

The following equation system describes the model:

![](equations.png)

with these variables and parameters (all rates are in 1/day):

- S: susceptible
- E: exposed
- I1: infected without priming
- I2: infected with priming
- H: hospitalized
- R: recovered
- N: total population size (constant)
- β (beta): transmission rate
- δ (delta): incubation rate
- α (alpha): fraction of population receiving priming
- r: clearance rate infected
- ρ (rho): increase in clearance rate due to priming
- h: hospitalization rate of infected
- γ (gamma): clearance rate of hospitalized

# License

CC-BY-SA 4.0
