# Evaluating-Real-Estate
Predicting house prices for real estate investments using machine learning

1. Created script for fetching csv data, which should be run anytime you expect the data to have updated. 









## Tips/Lessons Learned:

1. The histograms were tail-heavy (most of the data was skewed right relative to median). 
This could make it harder to detect patterns depending on the algorithm. Uniform, Bell-Shaped data is preferred.

2. Be aware for capped values of data if you expect to receive data points outside of this 
range in the real world. Model wont be accurate for values above. Either collect proper labels for values that were capped or remove them entirely from the test and train set.


3. You want to keep the same test set no matter how many times you run the algoirthm because if not, the algorithm will eventually see the entire dataset. So once you run the code to split into test and train the first time, set the test aside. There are other methods for this like hashing each row's uniqe identifier to decide whether or not it goes in test.

4. Finding correlations between one category (column) and the rest can be useful for new insights as well as potentially combining attributes. Some attributes dont make sense as stand-alone.







## Useful library functions

pd.info()
pd.value_counts()
pd.describe()
pd.hist() (with matplotlib)



