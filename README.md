# indoPacific_COVID19_model
**Associated paper**: Assessing the potential impact of oral COVID-19 antivirals and booster doses: a mathematical modelling study of selected middle-income countries in the Indo-Pacific - published in Vaccine: X, see https://doi.org/10.1016/j.jvacx.2023.100386

## Abstract
Booster doses and oral antivirals provide two options for reducing severe outcomes associated with COVID-19. In this project, we use a mathematical model to explore the benefits of booster doses and oral 
antivirals in four middle-income countries: Fiji, Indonesia, Papua New Guinea, and Timor-Leste. This paper answers key questions from policy makers in this region as we transition from pandemic to endemic
approaches of managing COVID-19 alongside regular healthcare priorities.

## Code history
The underlying deterministic SEIR model model was developed in a previous project (https://github.com/gizembilgin/vaccine_prioritisation_SLE). This study updated the original
model, adapted the model to four new settings (Fiji, Indonesia, Papua New Guinea, and Timor-Leste), and built a stochastic antiviral model component.

## Scripts included in this project
* *1_inputs/* contains all parameter files
* *2_fit/* contains scripts for fitting the transmission model to our study settings
* *3_antiviral_model/* contains the stochastic antiviral model
* *(0)_fitting.R* includes the initial conditions for maintaining consistency across fitting scripts (*2_fit/*)
* *(#)** scripts are the sub-scripts of the COVID-19 transmission model
* *(function)** scripts contain functions
* *(mech shop)** scripts create a subset of parameters used by the model
* *(sensitivity)** scripts run sensitivity analysis
* *(silho)** scripts reconstructe the vaccination history of our study settings
* *CommandDeck.R* runs all sub-scripts of the COVID-19 transmission model to complete one standard 'run' of the model


## Abbreviations
Please note that this list is not comprehensive. See the publication and associated Supplementary Material for any undefined abbreviations used in this code
* FJI = Fiji
* IDN = Indonesia
* NPI = non-pharmaceutical interventions
* PNG = Papua New Guinea
* R0 = basic reproduction number
* Reff = effective reproduction number
* TLS = Timor-Leste
* VE = vaccine effectiveness
