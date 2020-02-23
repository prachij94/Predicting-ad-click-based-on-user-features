# Predicting-ad-click-based-on-user-features

In this repository is used a fake advertising data set, indicating whether or not a particular internet user clicked on an Advertisement. We create a Logistic Regression model that will predict whether or not they will click on an ad based on the features of that user.

This data set contains the following features:

- 'Daily Time Spent on Site': consumer time on site in minutes
- 'Age': cutomer age in years
- 'Area Income': Avg. Income of geographical area of consumer
- 'Daily Internet Usage': Avg. minutes a day consumer is on the internet
- 'Ad Topic Line': Headline of the advertisement
- 'City': City of consumer
- 'Male': Whether or not consumer was male
- 'Country': Country of consumer
- 'Timestamp': Time at which consumer clicked on Ad or closed window
- 'Clicked on Ad': 0 or 1 indicated clicking on Ad


The data is explored visually using **seaborn** by finding general relationships between the **Area Income** and **Age**, the **Daily Time Spent on Site** and **Age**, the **Daily Time Spent on Site** and **Daily Internet Usage**. Also, plot all the variables against each other using pairplot with value colors defined by the column **'Clicked on Ad'** to check the impact on clicks with each changing parameter. 

A logistic regression model is created with *'Daily Time Spent on Site','Age','Area Income','Daily Internet Usage','Male'* and then predictions are made for the test data.

Then the model performance is evaluated by calculating the *Classification Report* and *Confusion matrix*.

To conclude, the logistic regression model performs quite well i.e. *approx. 91% accuracy* with few mislabelled points which is not bad given the size of our artificially generated dataset.
