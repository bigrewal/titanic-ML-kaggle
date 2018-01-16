# Titanic: ML from disaster

Data Analysis and feature engineering in this notebook was done using:
  [Notebook 1](https://github.com/minsuk-heo/kaggle-titanic/blob/master/titanic-solution.ipynb) and
  [Notebook 2](https://www.kaggle.com/helgejo/titanic/an-interactive-data-science-tutorial)

### Model Architecture: Tensorflow

    A = ((X*W1)+B1)
    B = ((Z*W2)+B2)

      (713,8)                               (713,5)
    X -------                           | A1-------------
      (8,5)   |         (713,5)         |    (5,1)      |        (300,10)
    W1 ------ --- Z1 -->sigmoid(A)--->  W2------------  Z2 --> sigmoid(Z2) --> A2
     (5,)     |                         |    (1,)       |
    B1 ------                           | B2------------
