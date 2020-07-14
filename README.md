# fictional-fiesta
IBM Inroduction to Machine Learning Course (edX) notebooks and models.

The files are stored in 4 folders; `my_attempts` and `solutions` contain Jupyter notebooks of course assignments, `datasets` contains the CSV datasets the models were trained on, and `saved_models` contains pickle dumps of those models.

## How to use saved models

Just run the following code in your python script or jupyter notebook (where `[MODEL NAME]` is the name of the dumps file you want to use):

`import pickle`<br>
`with open("saved_models/[MODEL NAME].sav", "rb") as file:`<br>
&nbsp;&nbsp;&nbsp;&nbsp;`model = pickle.load(file)`


## Models

The `saved_models` directory contains the following models (more details can be found in the corresponding Jupyter notebooks):

&bull; Model 1: Simple Linear Regression model to predict a car's CO<sub>2</sub> emission levels based on its engine size.

&bull; Model 2: Multiple Linear Regression model to predict a car's CO<sub>2</sub> emission levels based on its engine size, number of cylinders and fuel consumption levels.

&bull; Model 3: Polynomial Regression model to predict a car's CO<sub>2</sub> emission levels based on its engine size.

&bull; Model 5: K-Nearest Neighbors-based classifier model to predict a telecommunications company's customer's category based on their demographic features.

&bull; Model 6: Decision Tree-based classifier model to predict the drug suitable for a patient based on their health data.

&bull; Model 7: Logistic Regression model to predict whether a telecommunications company's customer will churn (leave for a competitor) based on their demographic data.

&bull; Model 8: Support Vector Machine (SVM)-based model to predict whether a given cell sample if benign or malignant based on the sample features.

&bull; Model 9: K-Means Clustering model to segment bank customers based on their details.

&bull; Model 10: Heirarchical Clustering model to classify which car in the market a given car prototype most resembles based on its features.

&bull; Model 11: Density-Based Clustering model to categorize weather stations in Canada based on the weather conditions reported by them.

The notebooks `model_12.ipynb` and `model_13.ipynb` contain `numpy`-based implementations of a movie recommender system, which you can access through those notebooks (since these models were not made through `scikit-learn` and I wasn't sure whether I could save them in a pickle dumps file (and if I could, how), I decided to leave them just as code implementations).
