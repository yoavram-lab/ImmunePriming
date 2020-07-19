# A new perspective for mitigation of SARS-CoV-2 infection: priming the innate immune system for viral attack
## Oren Kolodny, Michael Berger, Marcus W. Feldman, and Yoav Ram
## Open Biology 2020

This repository contains a [Jupyter notebook](notebooks/SEIR.ipynb) used to produce the Figure in the paper.
The notebook contains the model implementation.

The following equation system describes the model:
$$
\frac{dS}{dt} = - \beta \frac{S (I_1 + I_2)}{N}  \\
\frac{dE}{dt} = \beta \frac{S (I_1+I_2)}{N} - \delta E \\
\frac{dI_1}{dt} = (1-\alpha) \delta E - r I_1 - h I_1 \\
\frac{dI_2}{dt} = \alpha \delta E - \rho r I_2 - \frac{h}{\rho} I_2 \\
\frac{dH}{dt} = h (I_1 + I_2) - \gamma H \\
\frac{dR}{dt} = r (I_1 + \rho I_2) + \gamma H \\
N = S + E + I_1 + I_2 + H + R 
$$
with these variables and parameters (all rates are in 1/day):
- $S$ susceptible
- $E$ exposed
- $I_1$ infected without priming
- $I_2$ infected with priming
- $H$ hospitalized
- $R$ recovered
- $N$ total population size (constant)
- $\beta$ transmission rate
- $\delta$ incubation rate
- $\alpha$ fraction of population recieving priming
- $r$ clearance rate infected
- $\rho$ increase in clearance rate due to priming
- $h$ hospitalization rate of infected
- $\gamma$ clearance rate of hospitalized

# License

CC-BY-SA 4.0
