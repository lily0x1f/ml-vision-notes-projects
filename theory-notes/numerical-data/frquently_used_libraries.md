# Pandas
import pandas ad pd

  pd.options.display.max_rows()
  pd.options.display.max_columns()
  pd.options.display.max_coldwidth()
  pd.options.display.chop_threshold
  iloc() -> basic motive is to select rows and columns by number

### pd.describe_option() 
When called with no argument will print out the descriptions 

  pd.read_csv("") -> imports the dataset
There are other IO tools, read from user guide (https://pandas.pydata.org/docs/user_guide/io.html)

  df.describe() -> get statistics on the dataset

  pd.get_dummies(dataset, columns = [""], drop_first= (true or false))
    this line will apply one-hot encoding on the whole data frame datased

# NumPy

import numpy as np

  


# Matplotlib

import matplotlib.pyplot as plt (from matplotlib import pyplot as plt)



# sklearn

handling of missing data
from sklearn.impute import SimpleImputer

create and object calles imputer of class SimpleImputwe

imputer = SimpleImputer(missing_Values = np.nan, strategy = '')
