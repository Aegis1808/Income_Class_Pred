# Income_Class_Pred

## Abstract

This project focuses on the analysis and prediction of income levels using the census-income
dataset from the US Census Bureau. The dataset contains information for 48,842 individuals,
with attributes such as age, education, occupation, and more. The objective is to classify
whether a person's salary is greater than 50K or less than or equal to 50K based on the given
attributes.

The project involves several steps to build and evaluate decision tree models. First, missing
values in the dataset are handled using appropriate techniques such as replacing with mean
values/forward filling. Continuous attributes are discretized using custom bins to enable their
inclusion in the decision tree construction process.

Next, an optimal-sized decision tree is constructed using the Reduced Error Pruning
technique. The dataset is split into training, validation, and testing sets. The decision tree is
built on the training set and pruned using the validation set to find the optimal tree size. The
pruned tree is then evaluated on the testing set to assess its performance.
To compare the decision tree models, the process is repeated by combining the training and
testing datasets. Randomly selecting 67% of the data points as the training set and the
remaining points as the testing set, a new decision tree is built using the same procedure as
before.

The obtained decision trees are compared by analyzing their structures and evaluating their
performance on the respective testing datasets. If significant differences are observed, it
suggests sensitivity to the dataset split.

Interpretability is a crucial aspect of decision trees. The rules derived from the decision tree
model are examined and assessed for their intuitiveness and understandability.

Finally, a Random Forest classifier is constructed to further analyze and compare its results
with the decision trees obtained previously. The Random Forest approach combines multiple
decision trees to improve prediction accuracy and generalization.
