### 1. Acute Upper Respiratory Analysis
Below is the OLS summary for Acute Upper Respiratory Infection based on age groups.
``` text
 OLS Regression Results                                   
=============================================================================================
Dep. Variable:     Acute upper respiratory infection   R-squared:                       0.016
Model:                                           OLS   Adj. R-squared:                 -0.181
Method:                                Least Squares   F-statistic:                   0.08230
Date:                               Tue, 07 Apr 2026   Prob (F-statistic):              0.786
Time:                                       21:23:31   Log-Likelihood:                -21.252
No. Observations:                                  7   AIC:                             46.50
Df Residuals:                                      5   BIC:                             46.40
Df Model:                                          1                                         
Covariance Type:                           nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 6.4125      4.062      1.579      0.175      -4.030      16.855
age_group_encoded    -0.3232      1.127     -0.287      0.786      -3.219       2.573
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   1.277
Prob(Omnibus):                    nan   Jarque-Bera (JB):                0.955
Skew:                           0.659   Prob(JB):                        0.620
Kurtosis:                       1.760   Cond. No.                         6.85
==============================================================================
```

### 2. Bronchiolitis Analysis
Below is the OLS summary for Bronchiolitis based on age groups.

``` text
 OLS Regression Results                            
==============================================================================
Dep. Variable:          Bronchiolitis   R-squared:                       0.032
Model:                            OLS   Adj. R-squared:                 -0.161
Method:                 Least Squares   F-statistic:                    0.1660
Date:                Tue, 07 Apr 2026   Prob (F-statistic):              0.701
Time:                        21:23:39   Log-Likelihood:                -17.245
No. Observations:                   7   AIC:                             38.49
Df Residuals:                       5   BIC:                             38.38
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 2.4339      2.292      1.062      0.337      -3.457       8.325
age_group_encoded    -0.2589      0.636     -0.407      0.701      -1.893       1.375
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   1.998
Prob(Omnibus):                    nan   Jarque-Bera (JB):                3.237
Skew:                           1.569   Prob(JB):                        0.198
Kurtosis:                       4.121   Cond. No.                         6.85
==============================================================================
```
### 3. Bronchitis Analysis
Below is the OLS summary for Bronchitis based on age groups.

``` text
OLS Regression Results                            
==============================================================================
Dep. Variable:             Bronchitis   R-squared:                       0.073
Model:                            OLS   Adj. R-squared:                 -0.112
Method:                 Least Squares   F-statistic:                    0.3937
Date:                Tue, 07 Apr 2026   Prob (F-statistic):              0.558
Time:                        21:23:50   Log-Likelihood:                 4.4973
No. Observations:                   7   AIC:                            -4.995
Df Residuals:                       5   BIC:                            -5.103
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 0.7893      0.103      7.692      0.001       0.526       1.053
age_group_encoded    -0.0179      0.028     -0.627      0.558      -0.091       0.055
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   2.955
Prob(Omnibus):                    nan   Jarque-Bera (JB):                0.571
Skew:                          -0.463   Prob(JB):                        0.752
Kurtosis:                       1.951   Cond. No.                         6.85
==============================================================================
```

### 4. Croup Analysis
Below is the OLS summary for Croup based on age groups.

``` text
         OLS Regression Results                            
==============================================================================
Dep. Variable:                  Croup   R-squared:                       0.010
Model:                            OLS   Adj. R-squared:                 -0.188
Method:                 Least Squares   F-statistic:                   0.05261
Date:                Tue, 07 Apr 2026   Prob (F-statistic):              0.828
Time:                        21:23:54   Log-Likelihood:                -12.918
No. Observations:                   7   AIC:                             29.84
Df Residuals:                       5   BIC:                             29.73
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 1.3750      1.235      1.113      0.316      -1.800       4.550
age_group_encoded    -0.0786      0.343     -0.229      0.828      -0.959       0.802
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   1.317
Prob(Omnibus):                    nan   Jarque-Bera (JB):                1.187
Skew:                           0.849   Prob(JB):                        0.552
Kurtosis:                       1.911   Cond. No.                         6.85
==============================================================================
```

### 5. Pneumonia Analysis
Below is the OLS summary for Pneumonia based on age groups.

``` text
OLS Regression Results                            
==============================================================================
Dep. Variable:              Pneumonia   R-squared:                       0.391
Model:                            OLS   Adj. R-squared:                  0.269
Method:                 Least Squares   F-statistic:                     3.204
Date:                Tue, 07 Apr 2026   Prob (F-statistic):              0.133
Time:                        21:23:59   Log-Likelihood:                -7.2141
No. Observations:                   7   AIC:                             18.43
Df Residuals:                       5   BIC:                             18.32
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 0.8964      0.547      1.640      0.162      -0.509       2.302
age_group_encoded     0.2714      0.152      1.790      0.133      -0.118       0.661
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   1.856
Prob(Omnibus):                    nan   Jarque-Bera (JB):                0.247
Skew:                          -0.018   Prob(JB):                        0.884
Kurtosis:                       2.081   Cond. No.                         6.85
==============================================================================
```


### 6. Sinus Infection Analysis
Below is the OLS summary for Sinus Infection based on age groups.

``` text
 OLS Regression Results                            
==============================================================================
Dep. Variable:        Sinus infection   R-squared:                       0.076
Model:                            OLS   Adj. R-squared:                 -0.108
Method:                 Least Squares   F-statistic:                    0.4128
Date:                Tue, 07 Apr 2026   Prob (F-statistic):              0.549
Time:                        21:24:07   Log-Likelihood:                 8.2392
No. Observations:                   7   AIC:                            -12.48
Df Residuals:                       5   BIC:                            -12.59
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 0.2750      0.060      4.574      0.006       0.120       0.430
age_group_encoded    -0.0107      0.017     -0.643      0.549      -0.054       0.032
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   1.669
Prob(Omnibus):                    nan   Jarque-Bera (JB):                1.044
Skew:                          -0.945   Prob(JB):                        0.593
Kurtosis:                       2.915   Cond. No.                         6.85
==============================================================================
```

### 6. Tonsilitis Infection Analysis
Below is the OLS summary for Tonsilitis Infection based on age groups.

``` text
OLS Regression Results                            
==============================================================================
Dep. Variable:            Tonsillitis   R-squared:                       0.000
Model:                            OLS   Adj. R-squared:                 -0.200
Method:                 Least Squares   F-statistic:                 0.0008892
Date:                Tue, 07 Apr 2026   Prob (F-statistic):              0.977
Time:                        21:24:11   Log-Likelihood:                 4.1418
No. Observations:                   7   AIC:                            -4.284
Df Residuals:                       5   BIC:                            -4.392
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
=====================================================================================
                        coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------------
const                 0.1509      0.108      1.398      0.221      -0.127       0.428
age_group_encoded     0.0009      0.030      0.030      0.977      -0.076       0.078
==============================================================================
Omnibus:                          nan   Durbin-Watson:                   1.467
Prob(Omnibus):                    nan   Jarque-Bera (JB):                0.466
Skew:                           0.478   Prob(JB):                        0.792
Kurtosis:                       2.173   Cond. No.                         6.85
==============================================================================
```





