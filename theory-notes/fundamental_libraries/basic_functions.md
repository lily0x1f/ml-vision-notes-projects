#Some frequently used libraries

### numpy

NumPy is a Python library that provides a multidimensional array object, various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more

````
  np.array([])
	np.zeros((3, 3)) -> #3*3 array of zeros
	np.ones((2, 2)) -> #2*2 array of ones
	np.linspace(0, 1, 5) #generate 5 values between 0 and 1
	np.mean(arr) #calculates mean
	np.dot(A, B) #dot multiplication of two matrices
	np.random.rand(5) #random float array
	
````
Absolute beginner

https://numpy.org/devdocs//user/absolute_beginners.html

#### pandas
Tools for reading and writing data between in memory stuff and different formats such as CSV and text files, Microsoft Excel, SQL databases, and the fast HDF5 format;
merging and joining of data sets;
label-based slicing, fancy indexing, and subsetting of large data sets;
data filtering, transformation, and summarization

````
	pd.read_csv("file.csv")
	df.head() # shows first 5 rows
	df.describe() #summary stats
	df['column'] #access column
	df.iloc[0] # access row by indrex
	df[df['col'] > 5] # filter rows
	df.groupby('category').mean() # groupby and aggregate
````

https://jupyterlab.readthedocs.io/en/stable/user/interface.html

### plotly express plotly.express
````
	px.scatter(df, x= ->int, y= ->int) scatter plot
	px.line(df, x= ->int, y= ->int) line chart
	px.bar(df, x= ->int, y= ->int) bar chart
	px.histogram(df, x= ) histogram
````
  quick and interactive plotting


### seaborn
Seaborn is a library for making statistical graphics in Python. 
````
	sns.heatmap(df.corr()) correlation heatmap
	sns.boxplot(x="col", data=df)
	sns.histplot(df["feature"]) histogram
	sns..violinplot(x="group", y="value", data=df) violin plot
	sns.pairplot(df) pairwise scatter 
	
````

### keras

build and train neural networks
high level wrapper tensorflow
````

	from keras.models import Sequential
from keras.layers import Dense

model = Sequential([
    Dense(64, activation='relu', input_shape=(10,)),
    Dense(1, activation='sigmoid')
])
model.compile(optimizer='adam', loss='binary_crossentropy')
model.fit(X_train, y_train, epochs=10, batch_size=32)
````

burada baya bi kullanım vardı:
https://colab.research.google.com/github/google/eng-edu/blob/main/ml/cc/exercises/linear_regression_taxi.ipynb?utm_source=mlcc&utm_campaign=colab-external&utm_medium=referral&utm_content=linear_regression#scrollTo=EE7nBxoMUtE9


