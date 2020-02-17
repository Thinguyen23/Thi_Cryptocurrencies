# Crytocurrency Analysis
In this project, we use unsupervised learning to analyze [data](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/crypto_data.csv) on the cryptocurrencies traded on the market.
# Objectives
1. Prepare the data for dimensions reduction with PCA and clustering using K-means.
2. Reduce data dimensions using PCA algorithms from sklearn.
3. Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.
4. Create some plots and data tables to present your results.
## 1. Data Preprocessing
1. Remove all cryptocurrencies that aren’t trading.
2. Remove all cryptocurrencies that don’t have an algorithm defined.
3. Remove the "IsTrading" column.
4. Remove all cryptocurrencies with at least one null value.
5. Remove all cryptocurrencies without coins mined.
6. Store the names of all cryptocurrencies on a DataFramed named coins_name
7. Remove the CoinName column.
8. Create dummies variables for all of the text features, and store the resulting data on a DataFrame named X.
9. Use the StandardScaler from sklearn (Links to an external site.) to standardize all of the data from the X DataFrame.
![Xscaled](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/Xscaled.png)
## 2. Reducing Data Dimensions Using PCA
Create a DataFrame named “pcs_df” that includes the following columns: PC 1, PC 2, and PC 3.
![pca](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/pca.png)
## 3. Clustering Cryptocurrencies Using K-means
1. Create an elbow curve to find the best value for K.
![elbowcurve](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/elbowcurve.png)
The best value for K is 4.
2. Run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data. 
3. Create a new DataFrame named “clustered_df” with columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class. 
![finaldf](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/finaldf.png)
## 4. Visualizing Results
1. Create a 3D scatter plot using Plotly Express to plot the clusters using the clustered_df DataFrame.
![3d](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/3d.png)
2. Use hvplot.table to create a data table with all the current tradable cryptocurrencies.
![table](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/table.png)
3. Create a scatter plot using hvplot.scatter to present the clustered data about cryptocurrencies
![chart](https://github.com/Thinguyen23/Thi_Cryptocurrencies/blob/master/images/chart.png)




