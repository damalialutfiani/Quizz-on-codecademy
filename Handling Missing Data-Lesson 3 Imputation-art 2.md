**Article 2 – Linear Interpolation**

1.  Fill in the blank

    Fill in the properties that we look for when deciding if a dataset is a good fit for linear interpolation.

        datasetType = _____
        dataPattern = _____
        missingDataType = _____
        seasonalData = _____

    a.  Structurally Missing Data
    
    b.  **linear**
    
    c.  MNAR
    
    d.  **False**
    
    e.  **MCAR**
    
    f.  categorical
    
    g.  cubic
    
    h.  quadratic
    
    i.  polynomial
    
    j.  MAR
    
    k.  True
    
    l.  DataFrame
    
    m.  **time-series**
  
    Click or drag and drop to fill in the blank

        datasetType = time-series
        dataPattern = linear
        missingDataType = MCAR
        seasonalData = False

2.  Coding question

    i.  Calculate the missing value in the dataset using linear interpolation and strictly Python (no external libraries).

    ii.  Set y equal to that missing value and print it to the terminal. The missing data in this case is reported as a None.

    iii.  As a reminder, here is the equation for linear interpolation:
    
    ![3 - art 2 2](https://user-images.githubusercontent.com/74751990/212523046-912db50b-a164-4345-8e6a-89caee96c4ea.jpg)

    >   Code    :

        years = [2000,2001,2002,2003]
        values = [1000,1062,None,1180]

        # Calculate the missing value
        x1 = 2001
        y1 = 1062
        x2 = 2003
        y2 = 1180
        x = 2002

        y = y1 + (x - x1) * ((y2 - y1) / (x2 - x1)) 
        print(y)

    >   Result :
    
(pict)
