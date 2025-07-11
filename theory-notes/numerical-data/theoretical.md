# Numerical Data

Numerical data; quantitive data, consists of numeric values that represent measurable quantities. 

Which data are valid, to decide look at std and mean. Data with standard deviation almost as big as mean is irrelevant. 

# Scaling
Feautre scaling means putting data at the same level or range.

### Linear Scaling (Normalization)
X' = (X - X_min ) / (X_max - X_min)
Scales the value to range 0 to 1, inclusively.

Limitation of normalization is outliers. Normalization may not effectively handle their influence -> can lead to skewed or distorted results.
Normalization is a good choice when lower and upper bound dont change much over time. Feature contains few outliers, and those are not extreme.

### Z-score Scaling (standardization)
Input variables are rescaled so that all variables maintain a standard deviation of 1.

<img width="363" height="76" alt="image" src="https://github.com/user-attachments/assets/96fede4b-3fd6-4cb0-967b-7446c50ccb5a" />

No rule when to use normalization vs. standardization. However, if data have outliers use standardization.

### Log scaling

Computes the logarithm of the value. (mostly uses natural base -ln)

Log scaling is helpful when data conforms to a power law distribution.

There are more normalization techniques for sure (clipping, etc)

# Handling of Noisy Data
Noise is somewhat the unwanted variance, some random error in measurable variable.


### Smotthing or Binning Methods

Binning (bucketing) is a technique that groups different subranges into bins. 

Smoothing by bin mean: data is sorted, divide data into equal bins and calculate the mean of each bin. All elements int the data will be replaced by the arithmetic mean.





























