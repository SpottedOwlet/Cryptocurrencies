# Analysis of the Cryptocurrency Data

<h3> Overview Of The Analysis</h3>

<h3> Preprocessing the Data for PCA </h3>
Cryptocurrency market analysis using unsupervised machine learning. The crypto_data.csv file was cleaned using pandas operations. The cleaned dataset was then prepared by removing the unnecessary data and keeping only the relevant columns for further analysis. Since unsupervised machine learning only analyzes the columns in the numeric form, the text columns (Algorithm & ProofType) were converted into numeric columns using get_dummies functions in pandas. The data was then scaled to remove any large difference between datapoints using StandardScaler function from Scikitlearn package. 
<br>

<h3>  Reducing Data Dimensions Using PCA </h3>
Scaled data was used for principal component analysis PCA and reduced into 3 components. This step was essential for the k-means clustering technique used for classifying the cryptocurrency data.

<kbd> <img width="610" alt="Screen Shot 2022-02-26 at 2 43 02 AM" src="https://user-images.githubusercontent.com/90424752/155840232-14101efa-2d69-431a-a6bc-ab582cce9022.png"> </kbd>


<h3>  Clustering Crytocurrencies Using K-Means </h3>
To find the optimum number of clusters, elbow curve method was used. The optimum number of clusters as seen below, were observed to be 4, where the plot lost it's slope and became almost horizontal. This indicates that there would not be significant change in the accuracy of the model by increasing the number of clusters any further.

<br>
<h4> Elbow Curve </h4>

<kbd>  ![bokeh_plot](https://user-images.githubusercontent.com/90424752/155840386-f5f0d218-21c3-4942-adfa-460d7c5c59be.png)
</kbd>


<h3>  Visualizing Cryptocurrencies Results </h3>

The 3 Dimensional visualization of the classification achieved with the help of k-means clustering can be seen below.

<kbd> ![newplot (2)](https://user-images.githubusercontent.com/90424752/155840198-b6df24c2-07b8-4985-8392-491f97fc68e6.png) </kbd>


The 2 dimensional scatter plot of the same data shows Total Coins Mined vs Total Coin Supply.


<kbd>  <img width="997" alt="Screen Shot 2022-02-26 at 2 54 26 AM" src="https://user-images.githubusercontent.com/90424752/155840568-499b9ec3-896b-4ac3-811d-1464e1da6d7d.png">
</kbd>


