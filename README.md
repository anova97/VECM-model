# VECM-model
transformation of the VAR model into a vector error correction model - VECM

## Dataset
This project uses the data used in the VAR project. They were downloaded from (https://stooq.pl). 
Daily historical index data from January 2010 to December 2019 was downloaded.

## Methodology
an ADF test was carried out, the variables are non-stationary

Choice of model delay order
In order to choose the right one I create two models, test stationarity and autocorrelation in them. Based on the tests I will choose which lag order is more appropriate.

The cointegration of the time series was tested using the Johansen test: the maximum eigenvalue test and the trace test
there is one stable cointegrating relationship.

A VECM model with 2 lags (the VECM model is built with lags 1 less than in the VAR model) and one cointegrating relation is built.  

For the asestimated VECM model, the impact of one sector on another will be estimated using a stimulus response function. The SPX index was chosen as the stimulus because it is one of the most well-known and influential indices in the world. Its impact on the indices studied in this project can be significant.
