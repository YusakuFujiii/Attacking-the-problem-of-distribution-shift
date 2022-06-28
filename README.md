# Attacking the problem of distribution shift

### Problem setting
The performance of a ML model falls if a shift in the distribution of features occurs in out-of-sample data. However, in financial time series, the distribution of features tends to change over time. How should we address this problem?

### Existing methods
1. richman non-stationarity score method
   - What is it?
     - This method regresses sample indicies on features, makes a prediction on a validation data, and computes r2 score. 
   - What is good about it?
     - Low r2 means that the features are bad at predicting their sample indicies that are increasing with time, implying that
       the distribution of the features can be considered as independent of time. 
     - By choosing features with this method, we could deal with the problem of distribution shift better. 
     
     
