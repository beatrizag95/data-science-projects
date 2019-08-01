# Titanic Survivals Classifier
_Author: Beatriz Golindano_

This project is a basic demonstration of the assembly method (combination) of base learning models, in particular the assembly variant known as Stacking. __Stacking__ is used as a prediction of some basic classifiers and then uses another model in the second level to predict the result of previous first level predictions.

For the design of the model, Python libraries were used for machine learning, such as: __Pandas__ (Used for cleaning and data processing), __NumPy__ (To create data arrays), __Seaborn and Matplotlib__ (For data visualization through graphs), and also, the __Sckit-Learn__ library for the creation of prediction models and classifiers. Together with this, statistical concepts were used for the treatment of the data set, such as: the median.

The data set was taken from the Kaggle community in the competition of [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic). The documents presented in the project are described below:

1. [Training dataset (train.csv)](https://github.com/beatrizag95/data-science-projects/blob/master/Data%20Science%20Project%201:%20Titanic/train.csv): The training set used to build the machine learning model. For the training set, we provide the result (also known as the "basic truth") for each passenger.
2. [Test dataset (test.csv)](https://github.com/beatrizag95/data-science-projects/blob/master/Data%20Science%20Project%201:%20Titanic/test.csv): The test set used to demonstrate how well the model works with unseen data. The test does not provide the basic truth for each passenger.
3. [Gender Submission (gender_submission.csv)](https://github.com/beatrizag95/data-science-projects/blob/master/Data%20Science%20Project%201:%20Titanic/gender_submission.csv): A set of predictions that assume all and only female passengers survive, as an example of what a submission file should look like.
4. [Pearson Correlation Example (pearson_correlation.png)](https://github.com/beatrizag95/data-science-projects/blob/master/Data%20Science%20Project%201:%20Titanic/pearson_correlation.png): An example for Pearson's correlation when its values have a strong relationship with each other, given that in the project carried out its variables were independent, that is, no correlation between them was visualized. 
5. [Titanic Survivals Classifier Notebook (Titanic survivals clasiffier.ipynb)](https://github.com/beatrizag95/data-science-projects/blob/master/Data%20Science%20Project%201:%20Titanic/Titanic%20survivals%20classifier.ipynb): The jupyter notebook used to create and run the models.
6. [Stacking Model Results (StackingSubmission.csv)](https://github.com/beatrizag95/data-science-projects/blob/master/Data%20Science%20Project%201:%20Titanic/StackingSubmission.csv): Prediction results with the designed model.


## Data Dictionary

### __Survival__
 0 = No, 1 = Yes 

### __Pclass__ 
* A proxy for socio-economic status (SES).
* 1st = Upper, 2nd = Middle,3rd = Lower.
* Ticket class: 1 = 1st, 2 = 2nd, 3 = 3rd.

### __Sex__ 
Female/Male.

### __Sibsp__
* Number of siblings/spouses aboard the Titanic. 
* The dataset defines family relations in this way.
* Sibling = brother, sister, stepbrother, stepsister.
* Spouse = husband, wife (mistresses and fiancés were ignored).

### __Parch__
* Number of parents/children aboard the Titanic.
* Parch: The dataset defines family relations in this way.
* Parent = mother/father.
* Child = daughter, son, stepdaughter, stepson.
* Some children travelled only with a nanny, therefore parch=0 for them.

### __Ticket__
Ticket number fare Passenger fare.

### __Cabin__ 
Cabin number embarked Port of Embarkation: C = Cherbourg, Q = Queenstown, S = Southampton.

### __Age__
Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5.

## References:

* [Titanic best working Classifier](https://www.kaggle.com/sinakhorami/titanic-best-working-classifier).