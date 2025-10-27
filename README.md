# US population growth: Exponential, Logistic, Gompertz

**Goal**

Fit three growth models (exponential, logistic, Gompertz) to U.S. population data, estimate parameters, compare fits, and discuss limits.

**Contents**
- Notebooks/Project3.ipynb  — analysis and plots
- Latex/Project_3.pdf       — write-up (intro, methods, results, conclusions)
- Presentation/Project 3.pptx - presentation of findings and methods

**Methods**
- Estimate parameters by minimizing MAE/RMSE (and check residuals)
- Get starting values from linearized forms:
  - Exponential: log P vs t
  - Logistic: log(P/(K−P)) vs t with a scanned K
  - Gompertz: log(−log(P/L)) vs t with a scanned L

**Results**
- Exponential fits short spans but overpredicts the long run
- Gompertz is often best for recent U.S. deceleration
- Logistic can fit well when data sit near the mid S-curve
- Report includes error tables and diagnostics

**Data sources**
- https://www.worldometers.info/

**Notes and limits**
- r, K, L depend on the time window; not fixed “capacities”
- Models assume constant rates and a closed population; migration and shocks are omitted
