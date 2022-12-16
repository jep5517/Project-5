# Project 5

Term: Fall 2022


Project title: Predicting Car Insurance Claims

Team members: 

John Podias


Project summary: 

Objectives:

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

Data set Description: It is a collection of information about
different car insurance policies at a given point in time. No further
information, such as source or valuation date, was provided. Variables
descriptions can be found in the data file and it is sourced from the Kaggle link
also provided below. We use the Kaggle "train" set as our main data set
before the train/test split and rename it `policy_data`:

https://www.kaggle.com/datasets/ifteshanajnin/carinsuranceclaimprediction-classification?resource=download&select=train.csv

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
 
