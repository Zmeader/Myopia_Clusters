# Myopia_Clusters

## Project Goal
Process and create models with myopia data in order to better understand if patient clusters exist by utilizing scikit learn. 

## Main Technologies Used
* Python
* Scikit Learn

## Process
1. Pulled in the data and dropped the target column given the model is for unsupervised learning.

2. Scaled the data and used `fit_transform` to create the scaled data.

3. Applied PCA in order to perform dimensionality reduction.

4. Added t-sne to create a scatter plot of the data with label colors based on the original target column.

5. Created and ran the KMeans model and added the new class column through `model_labels`.

6. Created a loop to append the k items into the inertia list.

7. Plotted the k and inertia data in order to discover the proper k variable number which was 3.

8. Wrote a function called `get_clusters` in order to create a new dataframe with clusters.

9. Applied another function called `show_clusters` to portray the groupings of which patients would fall in.

## Conlusion
After creating the unsupervised model, it appears there are three distinct clusters for which each patient would fall into when dealing with myopia. 