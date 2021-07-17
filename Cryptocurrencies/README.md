# Cryptocurrencies
# **Business Objective**
Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of your most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrencies investment portfolio for its customers. The company, however, is lost in the immense universe of cryptocurrencies and asks you to present a report of what cryptocurrencies are on the trading market and how cryptocurrencies could be grouped toward creating a classification for developing this new investment product.

The data Martha will be working with is not ideal, so it will be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she decided to use **Unsupervised Learning**. To group the cryptocurrencies, Martha decided on a clustering algorithm to help determine about investing in this product. She’ll use **data visualization**s to share her findings with the board.
# **Abstract**
- Prepare the data for dimensions reduction with PCA and clustering using K-means.
- Reduce data dimensions using PCA algorithms from sklearn.
- Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.
- Create some plots and data tables to present your results.
# **Technologies and Resources used:**
- Jupyter Lab Notebook (mlenv kernals)
- Scikit-learn, Python machine learning library
- Clustering Data using K-means Alogrithm
- crypto_data.csv

# **Unsupervised Machine Learning Review**
Unsupervised learning is used in one of the following two ways:
- 1) Transform the data to create an intuitive representation for analysis 
     or to use in another machine learning model
- 2) Cluster or determine patterns in a grouping of data, 
     rather than to predict a classification.
### **Types of Unsupervised Learning**
#### **Transformations**
We use transformations when we need to take raw data and make it easier to understand. 
Transformations also can help prepare data so that it can be used for other 
machine learning algorithms.
#### **Clustering Algorithms**
We use clustering algorithms to group similar objects into clusters. For example, 
if a cable service wants to group those with similar viewing habits, 
we would use a clustering algorithm.

# **Cryptocurrency_Analysis Challenge**

## **Objectives**
**The goals for this challenge are for you to:**
- Prepare the data for dimensions reduction with PCA and clustering using K-means.
- Reduce data dimensions using PCA algorithms from sklearn.
- Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.
- Create some plots and data tables to present your results.

# **Project Instructions**
### **Data Preprocessin**

In this section, you have to load the information about cryptocurrencies from the provided CSV file and perform some data preprocessing tasks. The data was retrieved from CryptoCompare (Links to an external site.).

Start by loading the data in a Pandas DataFrame named “crypto_df.” Continue with the following data preprocessing tasks:
- Remove all cryptocurrencies that aren’t trading.
- Remove all cryptocurrencies that don’t have an algorithm defined.
- Remove the IsTrading column.
- Remove all cryptocurrencies with at least one null value.
- Remove all cryptocurrencies without coins mined.
- Store the names of all cryptocurrencies on a DataFramed named coins_name, and use the crypto_df.index as the index for this new DataFrame.
- Remove the CoinName column.
- Create dummies variables for all of the text features, and store the resulting data on a DataFrame named X.
- Use the StandardScaler from sklearn (Links to an external site.) to standardize all of the data from the X DataFrame. Remember, this is important prior to using PCA and K-means algorithms.

### **Reducing Data Dimensions Using PCA**
- Use the PCA algorithm from sklearn (Links to an external site.) to reduce the dimensions of the X DataFrame down to three principal components.
- Once you have reduced the data dimensions, create a DataFrame named “pcs_df” that includes the following columns: PC 1, PC 2, and PC 3. Use the crypto_df.index as the index for this new DataFrame.

### **Clustering Cryptocurrencies Using K-means**
- You’ll use the KMeans algorithm from sklearn (Links to an external site.) to cluster the cryptocurrencies using the PCA data.

#### **Complete the following tasks:**
- Create an elbow curve to find the best value for K, and use the pcs_df DataFrame.
- Once you define the best value for K, run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data. Use the pcs_df to run the K-means algorithm.
- Create a new DataFrame named “clustered_df,” that includes the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class. 

### **Visualizing Results**
**You’ll create data visualizations to present the final results.**
### **Complete the following tasks:**
- Create a 3D scatter plot using Plotly Express to plot the clusters using the clustered_df DataFrame. You should include the following parameters on the plot: hover_name="CoinName" and hover_data=["Algorithm"] to show this additional info on each data point.
- Use hvplot.table to create a data table with all the current tradable cryptocurrencies. The table should have the following columns: CoinName, Algorithm, ProofType, TotalCoinSupply, TotalCoinsMined, and Class.
- Create a scatter plot using hvplot.scatter to present the clustered data about cryptocurrencies having x="TotalCoinsMined" and y="TotalCoinSupply" to contrast the number of available coins versus the total number of mined coins. Use the hover_cols=["CoinName"] parameter to include the cryptocurrency name on each data point.
