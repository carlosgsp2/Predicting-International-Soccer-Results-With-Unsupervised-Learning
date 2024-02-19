# Predicting International Soccer Results With Unsupervised Learning
This project uses data from FIFA world ranking and international soccer results. The goal of the project is to create models that predict the results of the home team. 
In addition, each subsequent model should improve the performance of the last model. 

FIFA rankings are constantly ranking international soccer teams. The data released includes total match points, rank, rank date, country name, and rank change. The results dataset includes home team, away team,
home result, away result, and date. The last dataset, goalscorers, shows the dates and time someone scored a goal. 

It was diffucult to merge three datasets when the data for one of them dated back to more than one hundred years. In order to maintain predictions that were up to date and reduce computing resources,
I decided to not use results that were older than 2015. The best way to merge the tables was to use the country and date, this ensured that results were correctly matched.

The project could be used by sports industries like sports commentators to talk about the possible outcome of a match just like a weather forcast shows the probability of rain. 

With the use of feature engineering, I was able to create home results from home score and away score; This feature was then used as the dependent variable in my models. Other features created were win percentage and goal difference total.

I was able to  establish a relationship between my features by doing scatter plots and bar graphs.

For this project I used Random Forest Classifier, Logistic Regression, Gradient Boosting Classifier, and LGBM Classifier. Gradient boosting had the best performance. In order to deal with class imbalance, I used
LGBM Classifier, which performed better in the classes where gradient boosting underperformed. In oerder to evaluate the models, I looked at accuracy, precision, recall, and f1-score.

In the future, I would like to try to improve the model accuracy. I was able to achieve a 69% accuracy for home result predictions. I think that more work can be done to deal with the class imbalance problem. There is too much data for win results and not enough for tie and loss. 

![image](https://github.com/carlosgsp2/Predicting-International-Soccer-Results-With-Unsupervised-Learning/assets/145519266/fad21e3f-a2a5-44e3-bb43-103fcdc48220)
![image](https://github.com/carlosgsp2/Predicting-International-Soccer-Results-With-Unsupervised-Learning/assets/145519266/257916ec-c8bb-419a-8f9b-20f07564a793)
![image](https://github.com/carlosgsp2/Predicting-International-Soccer-Results-With-Unsupervised-Learning/assets/145519266/17cc6957-a13e-42e8-88f8-66a0b55fb1c4)
![image](https://github.com/carlosgsp2/Predicting-International-Soccer-Results-With-Unsupervised-Learning/assets/145519266/cd9bf606-539d-40b9-88d6-3ed4cea6ddf1)
![Screenshot 2024-02-19 091802](https://github.com/carlosgsp2/Predicting-International-Soccer-Results-With-Unsupervised-Learning/assets/145519266/3b11591e-d937-4c8d-a2eb-1641f70c7c10)




