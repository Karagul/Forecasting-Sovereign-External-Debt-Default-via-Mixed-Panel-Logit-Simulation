# Forecasting-Sovereign-External-Debt-Default-via-Mixed-Panel-Logit-Simulation
Data Bootcamp course Project (NYU Stern Fall 2018)

We implement a panel data extension of a mixed logit model in order to forecast
sovereign external debt defaults from 2010 to 2017. We fit a simulated version of the
model on historical data using an assortment of lagged economic variables hypothesized
to signal default and include year-fixed effects to control for year-specific influences.
The marginal effects of the variables are allowed to be randomized across countries in
order to reflect country-level heterogeneity in variable-specific influences. The model is
simulated using Monte Carlo sampling over parameterized independent normal distributions. 
Maximum likelihood estimation is penalized with an L2 regularization term
to improve out-of-sample performance. The optimal tuning parameter is estimated
using 10-fold cross-validation. The fully calibrated model is then used to predict unconditional 
probabilities of external debt default using the test data. The performance
of the model is assessed using the receiver operating characteristic.

#
Note:

In 'mixed_panel_logit.py', the mixed-logit model specification was exclusively written by Kenneth Rios (https://github.com/kenrios1993). My contributions were limited to constructing the cross-validation loop. 

