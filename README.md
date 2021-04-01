# Task2-Predictive-Analysis-Supervised-Learning-Titanic
General steps to follow: data exploration and analysis, data preprocessing and transformation (handle missing values, convert categorical features into numeric, convert discrete features into binary etc.), implementing Machine Learning models.

**DATA EXPLORATION:**

Info: it displays info of dataframe like types and columns.
Describe: The training dataset describes mean,std,min,max.
Isnull : Identifying null values.that contain missing values (NaN = not a number),
that we need to deal with.features could contribute to a high survival rate:
To me it would make sense if everything except ‘PassengerId’, ‘Ticket’ and
‘Name’ would be correlated with a high survival rate.

**PCLASS:**

The PClass = 1 are the people who paid for their ticket in high-class, while Pclass
= 2 are the middle-class and Pclass = 3 are the less fortunate class.
differences between classes here, regardless of numbers of people, Pclass1 is the
only class which has more survivors, not much different on Pclass2 and only few
people from Pclass3 are survived.

**AGE AND SEX:**

Men have a high likelihood of survival when they are between 18 and 30 years of
age,which is also a bit true for women but not entirely.For women the chances of
survival are higher between 14 and 40.
For men, the likelihood of survival between the ages of 5 and 18 is very low ,but
this is not true for women.Another thing to note is that infants are also a little bit
more likely to survive.

**EMBARKED:**

The Embarked numbers indicated by the 0 and 1.The counts of the
Southampton is very high compared to Cherbourg and Queenstown.

**FARE:**

Fare attributes findings of fare distribution of survivors vs non
survivors.The based on fare is highly counted in survivors and the difference
between the survivors vs non survivors.
SibSp and Parch:SibSp and Parch would make more sense as a combined feature
that shows the total number of relatives, a person has on the Titanic. I will create it
below and also a feature that shows if someone is not alone.
DATA PREPROCESSING: SYNTAXES:
Drop: dropping unwanted columns.
Re: This is findings missing dataFillna: Filling with common values.

CONVERTING FEATURES: It converts float into integer and int to float
CREATING CATEGORIES:we need to convert the ‘age’ feature. First we will

convert it from float into integer. Then we will create the new ‘AgeGroup”
variable, by categorizing every age into a group.
For the ‘Fare’ feature, we need to do the same as with the ‘Age’ feature. But it isn’t
that easy, because if we cut the range of the fare values into a few equally big
categories,
80% of the values would fall into the first category.
CREATING NEW FEATURES: Add two new features to the dataset, it's compute
out of other features.

**BUILDING MACHINE LEARNING MODELS:**

DECISION TREE CLASSIFIER:The decision tree model is the model of
computation in which an algorithm is considered to be basically a decision tree,
i.e., a sequence of branching operations based on comparisons of some quantities,
the comparisons being assigned unit computational cost.
In this decision tree split the data to training and testing data then predict the
attributes of survived and passenger id in the decision tree model and find accuracy
of predicted models.The accuracy of the decision tree is 92.59 
