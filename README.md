
# Multiple Linear Regression in Power BI

![Screenshot 2023-03-20 000235](https://user-images.githubusercontent.com/84715134/226199384-1cef99f2-6ba2-41f4-84fa-329f7d9c73d9.jpg)

Python Script -

import pandas as pd <br>
import statsmodels.formula.api as smf <br>
model = smf.ols(formula=""price ~ bedrooms + bathrooms + sqft_living"", data=dataset).fit() <br>
df = pd.DataFrame(model.params, columns=[""coefficients""])#(lf)df[""variables""] = model.params.index.tolist() <br>
 
