# Project 5

**Term:** Fall 2022


**Project title:** Predicting Car Insurance Claims

**Team members:**

John Podias

[Rmarkdown PDF](https://github.com/jep5517/Project-5/blob/main/doc/Project%20_5_Rmarkdown_PDF.pdf)


**Project summary**

**Objectives:**

1. To fit and compare a traditional binary classification algorithm to
    a more modern binary classification model where they can both
    classify whether or not a given car insurance policy holder at a
    given point in time will file a claim within the next 6 months
    (model interpretation is not major concern).

    1.  In doing this, we hope to find a model that can give reasonable
        precision and recall for an insurance company to use or at least
        provide a baseline for them to work from

2.  In addition, we want to attempt to build these models using an
    imbalanced data set, which mirrors real world situations, and then
    test a solution to see if we can make any improvements to our base
    models.

    1.  A priority of the business would be to catch more positives
        cases rather than missing out. They are willing to hire more
        resources to review the large number of positive cases that get
        flagged.

3.  Lastly, I hope to use this analysis as a practice/learning
    opportunity and try to implement methods I've never used before to
    develop as a data scientist.

**Data Set Description:** It is a collection of information about
different car insurance policies at a given point in time with a target variable that tells if a policy had filed a claim in 6 months or not. No further information, such as source or valuation date, was provided. Variable descriptions can be found in the data file and it is sourced from the Kaggle link also provided below. We use the Kaggle "train" set as our main data set before the train/test split and rename it `policy_data`:

https://www.kaggle.com/datasets/ifteshanajnin/carinsuranceclaimprediction-classification?resource=download&select=train.csv

**Conclusion:** We fit two types of models, a logistic regression model and a random forest model, and compared performance. The performance was so bad we realized we had to improve the data set because of the target variable imbalance. We implement SMOTE, which is an oversampling technique to create synthetic examples of the minority class of the target variable (which were policies that had filed claim in the next 6 months). Once we balanced the training set to 50/50, we saw a huge increase in recall for both models and some increase in precision for both models. Even though we have low precision, we will ultimately choose the random forest model as our preferred model since its precision, recall and F1 score were higher than logistic regression. This project was a great learning opportunity to tackle the issue of target imbalance and provide some valuable baseline model for insurance companies. 

Following suggestions by RICH FITZJOHN (@richfitz). This folder is orgarnized as follows.

```
proj/

├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
 
