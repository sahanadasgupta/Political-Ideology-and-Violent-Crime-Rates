# Political-Ideology-and-Violent-Crime-Rates
# The Effect of Political Ideology on Violent Crime Rates

R analysis code for a research poster (ATDP, UC Berkeley, 2024) examining whether a U.S. state's political ideology (liberal vs. conservative) is associated with differences in violent crime rates. Team project with Aditi and Tanya.

## Overview

Uses the built-in `USArrests` dataset (murder, assault, rape, and urban population rates per 100,000 residents for all 50 states) to explore whether violent crime patterns differ between states classified as liberal or conservative based on presidential voting history.

## What this notebook does

- Classifies all 50 states into "Liberal" or "Conservative" groups based on voting history
- Visualizes urban population and rape-arrest rates by state
- Breaks out murder, assault, rape, and urban population rates specifically for conservative states
- Runs regression diagnostics for conservative states — fitting urban population against each crime type (murder, assault, rape) and checking:
  - **Linearity** — scatter plots with linear and LOESS smoothers
  - **Homoskedasticity** — residual plots
  - **Normality** — Q-Q plots of standardized residuals

## Note on scope

This file covers the exploratory visualization and regression-assumption-checking stage of the project, focused on conservative states. The final poster's core result — a population regression model with an ideology × urban-population interaction term, tested across both liberal and conservative states (finding a statistically significant difference in rape rates, p = 0.034, but not in murder or assault rates) — was completed as part of the broader group project; that portion of the analysis isn't included in this file.

## Tools

R (tidyverse, ggplot2, broom)

## Team

Sahana Dasgupta, Aditi, Tanya — ATDP (UC Berkeley), Summer 2024
