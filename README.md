# Adult-Census-Income
Predict whether income exceeds $50K/yr based on census data

[This data](https://www.kaggle.com/uciml/adult-census-income) was extracted from the 1994 Census bureau database by Ronny Kohavi and Barry Becker (Data Mining and Visualization, Silicon Graphics). A set of reasonably clean records was extracted using the following conditions: ((AAGE>16) && (AGI>100) && (AFNLWGT>1) && (HRSWK>0)). The prediction task is to determine whether a person makes over $50K a year.

Description of fnlwgt (final weight)
The weights on the Current Population Survey (CPS) files are controlled to independent estimates of the civilian noninstitutional population of the US. These are prepared monthly for us by Population Division here at the Census Bureau. We use 3 sets of controls. These are:

A single cell estimate of the population 16+ for each state.

Controls for Hispanic Origin by age and sex.

Controls by Race, age and sex.

We use all three sets of controls in our weighting program and "rake" through them 6 times so that by the end we come back to all the controls we used. The term estimate refers to population totals derived from CPS by creating "weighted tallies" of any specified socio-economic characteristics of the population. People with similar demographic characteristics should have similar weights. There is one important caveat to remember about this statement. That is that since the CPS sample is actually a collection of 51 state samples, each with its own probability of selection, the statement only applies within state.

Relevant papers
Ron Kohavi, "Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid", Proceedings of the Second International Conference on Knowledge Discovery and Data Mining, 1996. (PDF)

# RESULT: <br>
LR   -> LogisticRegression<br>
LDA  -> LinearDiscriminantAnalysis<br>
KNN  -> KNeighborsClassifier<br>
CART -> DecisionTreeClassifier<br>
NB   -> GaussianNB<br>
RF   -> RandomForestClassifier<br>
GBC  -> GradientBoostingClassifier<br>
XGB  -> XGBClassifier<br>

| Model | Accuracy |<br> 
  LR  :   0.841 <br>
  LDA :   0.831 <br>
  KNN :   0.842 <br>
  CART:   0.810 <br>
  NB  :   0.799 <br>
  RF  :   0.843 <br>
  GBC:   0.865 <br>
  XGB:   0.859 <br>

![alt text](https://github.com/Vladykart/Adult-Census-Income/blob/master/output_32_0.png)
