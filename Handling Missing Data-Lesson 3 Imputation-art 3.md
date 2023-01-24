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

2. Coding question
Use the IterativeImputer module within sklearn to impute the missing data values.

Use 10 iterations.
Set random_state to 1.
Set dfComplete equal to the resulting DataFrame.
