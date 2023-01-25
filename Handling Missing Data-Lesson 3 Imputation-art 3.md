**Article 3 – Multiple Imputation**

1.  Fill in the blank

    In the below sections, fill in the properties that we look for when deciding if a dataset is a good fit for multiple imputation.

        datasetType = _____
        missingDataType = _____

    a.  MNAR
    
    b.  MCAR
    
    c.  **categorical**
    
    d.  time-series
    
    e.  Structurally Missing Data
    
    f.  polynomial
    
    g.  cubic
    
    h.  **MAR**
    
    i.  linear
    
    j.  quadratic
    
    k.  DataFrame

    Click or drag and drop to fill in the blank

        datasetType = categorical
        missingDataType = MAR

2.  Coding question

    Use the IterativeImputer module within sklearn to impute the missing data values.

Use 10 iterations.
Set random_state to 1.
Set dfComplete equal to the resulting DataFrame.

Code :

import numpy as np
from sklearn.experimental import enable_iterative_imputer
from sklearn.impute import IterativeImputer
import pandas as pd

d = {
    'D': [6.9,np.nan,5.4,4.7,4.5,5.1,4.1,4.5,np.nan,7.5],
    'E': [18.5,21.9,np.nan,21.2,12.4,16.7,11,11.5,21.6,np.nan],
    'F': [np.nan,36.3,50.6,48.7,51.9,np.nan,51.6,50.1,46.9,36.6],
    'G': [80,70.1,94.5,np.nan,76.3,84.6,np.nan,93.6,68.9,82]
}

dTest = {
    'D': [5.6,np.nan,4.5,3.2,5.9],
    'E': [16.1,20.7,np.nan,22.4,13.4],
    'F': [np.nan,31.2,53.2,47.8,50.8],
    'G': [79.9,71.3,92.4,np.nan,75.6]
}

# Define df and dfTest as pandas DataFrames 
df = pd.DataFrame(data=d)
dfTest = pd.DataFrame(data=dTest)

# Create the IterativeImputer model to predict missing values
imp = IterativeImputer(max_iter=10, random_state=0)
 
# Fit the model to the test dataset
imp.fit(dfTest)

# Transform the model on the entire dataset
dfComplete = pd.DataFrame(np.round(imp.transform(df),1), columns=['D','E','F','G'])
 
#print(dfComplete.head(10))


# Uncomment the following statement to print the result
print(round(dfComplete.mean(),2))

Result :
(pict)
