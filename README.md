# Marketing-Mix-Model-Staffing
MMM in staffing industry for Causality Analysis and to identify channels that lead to high value placement

#### Which marketing channels actually drive revenue?
#### How long does advertising continue to influence sales?
#### When does increasing spend stop producing returns?
#### What budget allocation maximizes ROI?

## Marketing Mix Modeling (Bayesian)

This project demonstrates an end-to-end implementation of Marketing Mix Modeling (MMM) using Bayesian techniques.

## Project Structure
data/
notebooks/
src/
configs/
tests/
reports/

## Objectives
Estimate the causal incremental contribution of marketing channels to high-value placements and determine optimal budget allocation under diminishing returns.

- Estimate channel contribution
- Apply adstock and saturation effects (capture delayed impact and dimishing returns)
- Bayesian MMM modeling
- Budget optimization


## Why MMM modeling is appropriate in staffing & recruitment Marketing strategy
## WHY MMM vs MTA ?
  At this organization most of the marketing channel was upper funnel or offline channels where we didnt have any data on user level journey hence last touch ie,attribution before conversion would have been misleading.

  MMM provides aggregated time series level causal estimation - in our case ut was weekly data over 2.5 years.
  MMM also capture cross channel interactions and delayed effects - carryover lag effects.


## Bayesian MMM with Adstock transformation model for MMM   
    This model has two different components 
      1. Marketing Response structure that captures how marketing effect sales over time this is done by Adstock transformations
      2. Statistical Estimation Method that is used to estimate the parameters and uncertainity which is done using Bayesian inference 
    ** distributed lag is not used due to unstable coeff estimations
## Adstock decay rate estimation
  
