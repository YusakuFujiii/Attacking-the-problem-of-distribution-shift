# Attacking the problem of distribution shift

### Problem setting
The performance of a ML model falls if a shift in the distribution of features occurs in out-of-sample data. However, in financial time series, the distribution of features tends to change over time. How should we address this problem?

### Existing methods
1. richman non-stationary score 
   - What is it?
     - It is a metric that measures non stationarity of a feature.
   - What is good about it?
     - It is useful in feature engineering. 
     
     
