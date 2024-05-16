By Utilizing  unsupervised learning skills to reduce dimensionality and identify clusters in the penguins dataset!

Begin by reading in "data/penguins.csv" as a pandas DataFrame called penguins_df, then investigate and clean the dataset by removing the null values and outliers. Save as a cleaned DataFrame called penguins_clean.
Pre-process the cleaned data using standard scaling and the one-hot encoding to add dummy variables:
Create the dummy variables and remove the original categorical feature from the dataset.
Scale the data using the standard scaling method.
Save the updated data as a new DataFrame called penguins_preprocessed.
Perform Principal Component Analysis (PCA) on the penguins_preprocessed dataset to determine the desired number of components, considering any component with an explained variance ratio above 10% as a suitable component. Save the number of components as a variable called n_components.
Finally, execute PCA using n_components and store the result as penguins_PCA.
Employ k-means clustering on the penguins_PCA dataset, setting random_state=42, to determine the number of clusters through elbow analysis. Save the optimal number of clusters in a variable called n_cluster.
Create and fit a new k-means cluster model, setting n_cluster equal to your n_cluster variable, saving the model as a variable called kmeans.
Visualize your clusters using the first two principle components.
Add the label column extracted from the k-means clustering (using kmeans.labels_) to the penguins_clean DataFrame.
Create a statistical table by grouping penguins_clean based on the "label" column and calculating the mean of each numeric column. Save this table as stat_penguins.
