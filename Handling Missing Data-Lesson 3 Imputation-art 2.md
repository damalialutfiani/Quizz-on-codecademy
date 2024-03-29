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

     ![3 - art 2 2 result](https://user-images.githubusercontent.com/74751990/212523226-a0a5ca89-98cf-449c-834b-85318e37dca7.jpg)

3.  Coding question

    i.  You have data on the even years from 2000 to 2008. Calculate the missing values for the odd years (2001, 2003, 2005, and 2007) as odd_values using the .interp() method included with numpy.

    ii.  Then print odd_values to the terminal.
    
    >   Code :
    
        import numpy as np

        evens = [2000,2002,2004,2006,2008]
        even_values = [10000,8300,6124,3971,1795]

        # Define odds and odd_values
        odd = [2001, 2003, 2005, 2007]

        odd_values = np.interp(odd, evens, even_values)

        print(odd_values)
        # y = 1460545.50

    >   Result :
    
       ![3 - art 2 3 result](https://user-images.githubusercontent.com/74751990/212797990-a543db43-790c-4865-8beb-b83f603fd252.jpg)

