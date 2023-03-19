
# Multiple Linear Regression in Power BI

Python Script -

import pandas as pd
import statsmodels.formula.api as smf
model = smf.ols(formula=""price ~ bedrooms + bathrooms + sqft_living"", data=dataset).fit()
df = pd.DataFrame(model.params, columns=[""coefficients""])#(lf)df[""variables""] = model.params.index.tolist()
