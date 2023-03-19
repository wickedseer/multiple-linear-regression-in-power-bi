
# Multiple Linear Regression in Power BI

Python Script -

import pandas as pd <br>
import statsmodels.formula.api as smf <br>
model = smf.ols(formula=""price ~ bedrooms + bathrooms + sqft_living"", data=dataset).fit() <br>
df = pd.DataFrame(model.params, columns=[""coefficients""])#(lf)df[""variables""] = model.params.index.tolist() <br>
 
