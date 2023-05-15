# 3_antiviral_model

## Visual representation ##
![antiviral model schema.jpg](https://github.com/gizembilgin/indoPacific_COVID19_model/blob/main/3_antiviral_model/antiviral%20model%20schema.png)

## Table breakdown ##
|Scipt Title| Purpose | 
| ----------- | ----------- |
*(antiviral) set up.R* | runs the COVID-19 model with a variety of COVID-19 booster dose eligibility strategies in 2023
*(antiviral set up_MASTER.R* | runs *(antiviral) set up.R* and *(antiviral)(run).R* multiple times across our different settings
*(antiviral)(function) antiviral_model_manager.R*  | runs antiviral_model_worker multiple times in parallel and collates the results
*(antiviral)(function) antiviral_model_worker.R* | **contains heart of the model** - it compares the impact of varies oral antiviral and booster dose eligiblity strategies and availabilities on the incidence of severe outcomes
*(antiviral)(function) stochastic_VE.R* | samples from the uncertainty underlying our estimates of vaccine effectiveness to construct vaccine effectiveness (VE) estimates for each stochastic run
*(antiviral)(function) stochastic_severe_outcomes_application.R* | applies the sampled estimates for this stochastic runs to the estimate the incidence of severe outcomes this run
*(antiviral)(function) stochastic_severe_outcomes_sampling.R* | samples from the estimates of all underlying parameters
*(antiviral)(function) VE waning distribution expander.R* | finds the closest possible estimate for vaccine effectiveness for each heterologous primary schedule - booster dose combination
*(antiviral)(mech shop) stochastic severe outcome projections.R* | fits distributions to parameter estimates where the interval but not distribution is avaliable
*(antiviral)(plot) cocooning.R* | examines the reduction in transmission to all adults, and reduction in transmission to adults aged over 65 across our booster dose eligiblity scenarios
*(antiviral)(plot) outcomes averted by vax vs antiviral_v3.R* | compares the individual- and population-level impact of different antiviral and booster dose eligiblity strategies
*(antiviral)(run).R* | runs the antiviral model for adults_with_comorbidities
*(antiviral)(run) special case pregnant women.R* | runs the antiviral model for pregnant_women
