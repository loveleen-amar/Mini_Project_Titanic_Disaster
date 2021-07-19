# Mini_Project_Titanic_Disaster
Our aim in Titanic Dataset is to predict the survival status of passengers


## **The task:**  The sinking of the Titanic is one of the most infamous shipwrecks in history. Unfortunately, in that incident there weren’t enough lifeboats for everyone on board, resulting in the death of 1502 out of 2224 passengers and crew. Our aim in Titanic Dataset is to predict the survival status of passengers.

## **What type of problem:** Since we have to find the given passenger survived or not, thus this is a categorical problem which goes to classification.

EE **Dataset:** The dataset consists of in total 12 features. Namely: ['PassengerId', 'Survived', 'Pclass', 'Name', 'Sex', 'Age', 'SibSp', 'Parch', 'Ticket', 'Fare', 'Cabin', 'Embarked'].


## **Data Analysis using Visualization:** We first have to find out what features are affecting the survival columns. So for this, we find the correlation between each feature and the target column. Thus by checking we found that the Pclass, Sex, SibSp, Parch and embarkment were correlated to the survival column. Few observations from data analysis are listed below:-
1. The majority of passengers were in Pclass=3, however, the majority did not survive. Confirms our classifying assumption. The majority of infant passengers in Pclass=2 and Pclass=3 survived. This qualifies our classification assumption even further. The majority of passengers in Pclass=1 made it out alive.
2. Female passengers scored significantly better than male passengers in terms of survivability. Confirms the classification. Males exhibited a greater survival rate than females in Embarked=C. This might indicate a link between Pclass and Embarked, and then Pclass and Survived, rather than a straight link between Embarked and Survived. Pclass=3 and male passengers had different survival rates depending on the port of departure.
3. Unwanted features were dropped off.

## **The algorithm used:**  Decision tree classifier, Decision tree works by breaking down the dataset into small subsets. This breaking down process is done by asking questions about the features of the datasets. The idea is to unmix the labels by asking fewer questions necessary. As we ask questions, we are breaking down the dataset into more subsets. Once we have a subgroup with only the unique type of labels, we end the tree in that node. For Eg let's say we are asking to find out whether a certain person in the test dataset survived or not. We may ask a question like, is the person "male" or "female." Let's say the answer is "female." Then the algorithm might ask about the person's P-class. And likewise, it will compute further.
