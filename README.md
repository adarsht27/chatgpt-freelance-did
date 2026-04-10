\# Did ChatGPT Hurt Freelance Writers?

\### A Difference-in-Differences Analysis | Adarsh Tripathi



**[View the full rendered report →](https://adarsht27.github.io/chatgpt-freelance-did/)**



\---



\## Overview



This project uses a \*\*Difference-in-Differences (DiD)\*\* design to estimate the 

causal effect of ChatGPT's release (November 2022) on earnings in the freelance 

labor market, with particular focus on writing-adjacent occupations.



\*\*Treatment group:\*\* High AI-exposure occupations (writers, editors, translators)  

\*\*Control group:\*\* Low AI-exposure occupations (plumbers, electricians, etc.)  

\*\*Data strategy:\*\* Upwork-style earnings panel merged with Felten et al. (2023) 

AI exposure scores via occupation ID



\---



\## Key Result



The DiD estimate (β\_interaction) suggests a statistically significant earnings 

decline of \~$1,631 for high-exposure workers post-ChatGPT, relative to controls.



\---



\## Methods



\- Two-Way Fixed Effects (TWFE) regression

\- Clustered standard errors at the occupation level (`estimatr::lm\_robust`, CR2)

\- Parallel trends visualization

\- Placebo test (fake treatment date in pre-period)

\- Event-study plot (quarter-by-quarter coefficients)



\---



\## Files



| File | Description |

|------|-------------|

| `chatgpt\_freelance\_did.Rmd` | Full analysis in R Markdown |

| `docs/chatgpt\_freelance\_did.html` | Rendered HTML report |



\---



\## What I'd Do Differently



\- Use real Upwork/Freelancer API data rather than simulated panel data

\- Add a synthetic control as a robustness check

\- Explore heterogeneous treatment effects by platform and geography



\---



\## Tools



R · tidyverse · estimatr · ggplot2 · patchwork · kableExtra



\---



\## Reference



Felten, E., Raj, M., \& Seamans, R. (2023). \*Occupational Heterogeneity in Exposure 

to Generative AI.\* SSRN Working Paper.

