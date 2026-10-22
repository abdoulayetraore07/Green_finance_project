# Asset Stranding in the EU Power Sector under NGFS Scenarios

Estimation of stranded-asset risk for fossil-fuel power plants in the European Union under NGFS climate transition scenarios. Academic project, Green Finance course (P. Tankov), ENSAE Paris / Institut Polytechnique de Paris.

## Overview

The project estimates how much of the EU fossil power generation fleet becomes economically unviable ("stranded") as carbon prices rise and market conditions evolve along NGFS transition pathways. For each plant we build a forward operating margin, identify when it turns unprofitable, and aggregate the resulting stranding by fuel, vintage and country.

## Methodology

- Plant-level dataset from the Global Power Plant Database, restricted to EU fossil plants, with imputation of missing commissioning years.
- NGFS scenario trajectories for carbon prices, electricity prices, fuel prices and the generation mix.
- Capacity-factor evolution per fuel, calibrated and sanity-checked against observed data.
- Plant operating margin under each scenario, with a stranding criterion based on persistently negative margins.
- Transition Risk Score (TRS) aggregation: expected vs worst-case, uniform vs vintage-weighted.
- Sensitivity and robustness analysis (carbon-price model, capacity-factor threshold, tornado charts, ranking stability).

## Repository structure

- notebooks/tasks/ : task1 scope and sample, task2 scenario selection, task3 plant metrics (and vintage), task4567 stranding and portfolio aggregation
- data/raw/ : source datasets (GPPD, NGFS/IAM, Ember, carbon and commodity prices, country shapes)
- data/processed/ : cleaned plant data, scenario tables, stranding results
- outputs/figures/ : generated figures
- report/ : project report

## Data sources

Global Power Plant Database, NGFS / IAM scenario data, Ember wholesale electricity prices, World Bank carbon pricing and commodity prices, Global Coal Plant Tracker, IEA Projected Costs of Generating Electricity.

## Authors

Abdoulaye TRAORE, Franck KOUASSI and another student
Green Finance, ENSAE Paris / Institut Polytechnique de Paris
