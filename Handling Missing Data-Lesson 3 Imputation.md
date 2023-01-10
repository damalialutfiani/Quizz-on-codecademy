**Article 1 - Single Imputation**

In general, single imputation can be an effective technique to handle missing data for our time-series datasets. While it might not be the most sophisticated approach, it can be a useful quick-fix in the right circumstances.

1.

  >   Coding question :

   You are presented with this dataset that has two separate values reported over the course of 10 minutes. Use either LOCF or NOCB to fill in the missing value in the value1 column.

  ![3 - art 1 1](https://user-images.githubusercontent.com/74751990/210445612-e7dcb440-a904-4e77-bbbf-a331707a6fec.jpg)

  >   Code  :

    import pandas as pd
    import numpy as np

    d = {'timestamp': ['2021-11-11 12:00:00','2021-11-11 12:01:00','2021-11-11 12:02:00','2021-11-11 12:03:00','2021-11-11 12:04:00',
                      '2021-11-11 12:05:00','2021-11-11 12:06:00','2021-11-11 12:07:00','2021-11-11 12:08:00','2021-11-11 12:09:00'],
          'value1': [1,1,2,3,4,4,4,np.nan,6,6],
          'value2': [10,10,9,7,np.nan,5,5,5,5,5]
        }

    df = pd.DataFrame(data=d)

    ## Fill in the missing data in the value1 column
    df['value1'].ffill(axis=0, inplace=True)
    
    #impyute.imputation.ts.locf(data, axis=0)

    df['value2'].bfill(axis=0, inplace=True)
    #impyute.imputation.ts.nocb(data, axis=0)

    print(df)

  >   Result  :

   ![2hasil2](https://user-images.githubusercontent.com/74751990/210630067-4eecd426-8530-47dd-be66-7ee46ef7c753.png)

2.  

  >   Coding question :

  You are presented with this dataset that has two separate values reported over the course of 10 minutes. Use either LOCF or NOCB to fill in the missing value in the value2 column.

  ![3 - art 1 2](https://user-images.githubusercontent.com/74751990/211128175-7f100f08-6fe1-4dbc-8264-0a502854b2ad.jpg)

  >   Code :

    import pandas as pd
    import numpy as np

    d = {'timestamp': ['2021-11-11 12:00:00','2021-11-11 12:01:00','2021-11-11 12:02:00','2021-11-11 12:03:00','2021-11-11 12:04:00',
                    '2021-11-11 12:05:00','2021-11-11 12:06:00','2021-11-11 12:07:00','2021-11-11 12:08:00','2021-11-11 12:09:00'],
        'value1': [1,1,2,3,4,4,4,np.nan,6,6],
        'value2': [10,10,9,7,np.nan,5,5,5,5,5]
        }

    df = pd.DataFrame(data=d)

    ## Fill in the missing data in the 'value2' column
    df['value2'].bfill(axis=0, inplace=True)

    print(df)

  >   Result  :

  ![ini](https://user-images.githubusercontent.com/74751990/211536456-7052e240-3122-4292-8d87-f1f3ba97e910.jpg)
