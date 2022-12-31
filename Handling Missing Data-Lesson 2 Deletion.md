**Article 1 - Handling Missing Data with Deletion**

1. Listwise Deletion

   >  Coding question   :

   Consider the following dataset   :

   ![2 - art 1 1](https://user-images.githubusercontent.com/74751990/210073645-5eb3eaf2-4be9-4fa2-a6cb-e846ad588b79.jpg)

   Use listwise deletion to clean up the DataFrame so that there is no missing data.

   >  Code :
   
         import pandas as pd
         import numpy as np

         d = {'Date': ['01-Sept','02-Sept','03-Sept','04-Sept','05-Sept',
            '06-Sept','07-Sept','08-Sept','09-Sept','10-Sept'], 
            'Temperature': [18,17,14,16,15,14,16,19,13,14],
            'WindSpeed': [9,12,np.nan,6,np.nan,10,13,np.nan,18,5],
            'Rainfall': [1,3,np.nan,0,np.nan,4,5,np.nan,7,6]}

         df = pd.DataFrame(data=d)

         # TO DO
         print(df.head(10))

   >  Result :

      ![2 - art 1 satu](https://user-images.githubusercontent.com/74751990/210112666-d7e4476c-aac1-4e8b-ab52-f24a927ace12.jpg)

2. Pairwise Deletion

   >  Coding question   :

   Consider the following dataset:

(pict)
