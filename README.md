# Trade-Ahead-Project
* Created a tool to group and examine 340 stocks based on performnce, value and company health
* Optimized K-means and Hierarchical clusters to reach the best model
* Defined profiles of stocks based on the cluster groups and the attributes and characteristics of these stocks to help decision makers with identifying the best stocks for investment

## Code and Resources 
**Python version:** 8.2.0

**Packages:** pandas, numpy, matplotlib, seaborn, sklearn, scipy, yellowbrick

## Data Cleaning and Pre-processing 
The dataset was mostly clean. Outliers were treated (capped) to reduce distribution distortion by large values. Also, the data was scaled to standardize the range of independent variables and features of the data. This helps to ensure thats features with a high magnitude will not dominate other features with lower magnitude in the dataset.
## Exploratory Data Analysis (EDA)
Below are a few highlights from the univariate analysis and an insight into the distribution of stocks by sector and subsector
![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/badcc40d-3a5b-4387-9118-8a26353b9bc2)
![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/7b1bbaaa-71bf-4a12-9b97-57cba5d1724e)
![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/0bf766db-d114-4418-a8b8-7b2cc151009a)
## Model Building
Numeric variables were first standadized after which 12 K-Means clustering models were built using the euclidean method. The elbow method and silhouette visiualization were used to select the most suitable clustering model.
![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/15aa02e2-0da3-4b30-8657-29a565c735a6)
![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/85058095-c533-4203-9011-a1d8ceb459c3)
Hierarchical clustering models were also built using various linkage methods and distance metrics, as well as visual examination of dendograms. 
![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/351efef2-8176-46a9-a183-b092c63342cd)
## Model Performance 
* For the K-Means clustering models, model with 8 clusters appeared to be the better as there are more clusters above the average distortion line and fewer negative values. ![image](https://github.com/Ariyo347/Trade-Ahead-Project/assets/113588909/e05a34db-0ae4-4b57-930e-e24ee343102c)

* For the hierarchical clustering models, the model with ward linkage appeared better spread and the stocks looked more evenly distributed between the clusters.
