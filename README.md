# credit-risk-classification : Clustering Cryptocurrencies
In this project, I use the unsupervised learning method called K-Means clustering to categorize cryptocurrencies based on their performance. The goal is to create portfolio recommendations that can potentially yield profitable investment strategies.

# Data
"crypto_market_data.csv" contains market data for various cryptocurrencies recorded across different time periods.

# Summary
To begin, I utilize the elbow curve method with normalized data to determine the optimal value of "k" for the K-Means model, which will be applied using all the original features present in the dataset.
[fig]

After identifying the optimal "k" value, I proceed to train and predict the K-Means model, creating four clusters of cryptocurrencies. The inertia of each cluster is substantial, prompting consideration for reducing the number of features in the dataset.
[fig]

In order to reduce the number of features, I used Principal Component Analysis (PCA) to establish three primary clusters.
[fig]

After obtaining the PCA data, I recalculated the optimal "k" value for the K-Means model.
[fig]
Lastly, using the optimal "k" value for the PCA features, I visualize the new clusters by plotting them.

# Technologies
This is a Python 3.7 project ran using a JupyterLab in a conda dev environment.

The following dependencies are used:

Jupyter - Running code
Conda (4.13.0) - Dev environment
Pandas (1.3.5) - Data analysis
Matplotlib (3.5.1) - Data visualization
Numpy (1.21.5) - Data calculations + Pandas support
hvPlot (0.8.1) - Interactive Pandas plots
scikit-learn (1.0.2) - KMeans clustering, data normalization, and PCA

# Installation Instructions:
To run the program in JupyterLab, start by installing the Anaconda distribution. Once installed, launch JupyterLab within a conda development environment.

To ensure smooth execution of your notebook, use the "requirements.txt" file to replicate the exact conda development environment used during the project's development.

To create a duplicate of the conda development environment, use the following command:
    conda create --name myenv --file requirements.txt
Afterwards, install the requirements using this command:
    conda install --name myenv --file requirements.txt
These steps will set up the necessary environment to run the program successfully in JupyterLab.

# Usage:
The Jupyter notebook "crypto_investments.ipynb" contains all the necessary steps for data collection, preparation, and analysis. Data visualizations are displayed inline, and detailed analysis responses accompany each visualization.
