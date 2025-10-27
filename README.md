# US population growth: exponential, logistic, Gompertz

**Goal**
Fit three growth models (exponential, logistic, Gompertz) to U.S. population data, estimate parameters, compare fits, and discuss limits.

**Contents**
- notebooks/Project3.ipynb  — analysis and plots
- latex/Project_3.pdf       — write-up (intro, methods, results, conclusions)

**Methods**
- estimate parameters by minimizing MAE/RMSE (and check residuals)
- get starting values from linearized forms:
  - exponential: log P vs t
  - logistic: log(P/(K−P)) vs t with a scanned K
  - gompertz: log(−log(P/L)) vs t with a scanned L

**Results**
- Exponential fits short spans but overpredicts the long run
- Gompertz is often best for recent U.S. deceleration
- Logistic can fit well when data sit near the mid S-curve
- report includes error tables and diagnostics

**Data sources**
- https://www.worldometers.info/

**Notes and limits**
- r, K, L depend on the time window; not fixed “capacities”
- models assume constant rates and a closed population; migration and shocks are omitted
