# Creating-Customer-Segments-with-Arvato
## Project Overview

In this project, you will work with real-life data provided to us by our Bertelsmann partners AZ Direct and Arvato Finance 
Solution. The data here concerns a company that performs mail-order sales in Germany. Their main question of interest is to 
identify facets of the population that are most likely to be purchasers of their products for a mailout campaign. Your job as 
a data scientist will be to use unsupervised learning techniques to organize the general population into clusters, then use 
those clusters to see which of them comprise the main user base for the company. Prior to applying the machine learning 
methods, you will also need to assess and clean the data in order to convert the data into a usable form.

## Install
- NumPy
- pandas
- Sklearn / scikit-learn
- Matplotlib (for data visualization)
- Seaborn (for data visualization)

## Data

- `Udacity_AZDIAS_Subset.csv`: Demographic data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
- `Udacity_CUSTOMERS_Subset.csv`: Demographic data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
- `Data_Dictionary.md`: Information file about the features in the provided datasets.
- `AZDIAS_Feature_Summary.csv`: Summary of feature attributes for demographic data.
- `Identify_Customer_Segments.ipynb`: Jupyter Notebook divided into sections and guidelines for completing the project. 


## Preprocessing

First explore and understand the data that I'm working with. In this section, I’ll be working with the general demographics data.
As part of investigation of dataset properties, I'll attend to a few key points:

- How are missing or unknown values encoded in the data? Are there certain features (columns) that should be removed from the 
analysis because of missing data? Are there certain data points (rows) that should be treated separately from the rest?
- Consider the level of measurement for each feature in the dataset (e.g. categorical, ordinal, numeric). 
What assumptions must be made in order to use each feature in the final analysis? 
Are there features that need to be re-encoded before they can be used? 
Are there additional features that can be dropped at this stage?
- Create a cleaning procedure that you will apply first to the general demographic data, then later to the customers data.


## Feature Transformation

Use dimensionality reduction techniques to identify relationships between variables in the dataset, resulting in the 
creation of a new set of variables that account for those correlations. In this stage of the project, I will attend to 
the following points:

- Feature scaling. What might happen if I don’t perform feature scaling before applying later techniques you’ll be using?
- Apply principal component analysis (PCA) to find the vectors of maximal variability. How much variability in the data 
does each principal component capture? How to interpret associations between original features in your dataset based on 
the weights given on the strongest components? How many components will you keep as part of the dimensionality reduction 
process?


## Clustering

Finally, on the transformed data, apply clustering techniques to identify groups in the general demographic data. 
Then apply the same clustering model to the customers dataset to see how market segments differ between the general population
and the mail-order sales company. I will tackle the following points in this section:

- Use the k-means method to cluster the demographic data into groups. How should I make a decision on how many clusters to use?
- Apply the techniques and models that I fit on the demographic data to the customers data: 
data cleaning, feature scaling, PCA, and k-means clustering. 
Compare the distribution of people by cluster for the customer data to that of the general population. 
Any insight about which types of people are likely consumers for the mail-order sales company?





