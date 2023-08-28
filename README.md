

# Multi-Class Credit Score Classification

Credit score is designed to represent your creditworthiness, or how likely you are to repay a lender on time. Potential lenders and creditors look at your credit score as one factor when deciding whether to offer you new credit. Lenders may also use your credit score to set the interest rates and other terms for any credit they offer.

Your credit score is calculated using the information found on your credit report. Your payment history, the mix of credit accounts you have, the length of your credit history and your credit utilization rate (the percentage of available credit limits you are using) are all factors that might influence your credit scores.

![](https://github.com/sudhanshu2198/Multi-Class-Credit-Score-Classification/blob/main/images/dataset-cover.jpg)


**The main goal of this project is to develop a machine learning model to predict credit score given credit related information..**

## 🔗 Links

- [Dataset](https://www.kaggle.com/datasets/parisrohan/credit-score-classification)
- [Medium Article](https://medium.com/@sudhanshurastogi/credit-score-classification-problem-5dbe1cb3636f)
- [Kaggle Notebook](https://www.kaggle.com/code/sudhanshu2198/multi-class-credit-score-classification/notebook)

## 🛠 Frameworks
Numpy, Pandas, Matplotlib, Seaborn, Scikit-learn, Imblearn, Xgboost, Lightgbm, Optuna

## Results

![](https://github.com/sudhanshu2198/Multi-Class-Credit-Score-Classification/blob/main/images/dist4.png)
-While the precision recall curve is nearly same for all three classifier, different features holds differnet significance for models, with xgboost model feature importance quite different from other model. This signifies that model are diffrent and using their values in an ensemble or stacking might increase performance.
- LightGBM model performed better than XGBoost and Random Forest classifier.
- The precision recall curve also tells us that good credit score is misclassified more than standard and poor credit score class. Standard Credit Score class is misclassified least across all three models.
- The models are performing better on standard instances, underperforming on good and poor instances this can be due to class imbalance. Therefore we can use data sampling technique specially those that increase the instances of classes in borderline or overlapping area.
  
### Calibration Curve of Ensemble Model
![](https://github.com/sudhanshu2198/Multi-Class-Credit-Score-Classification/blob/main/images/calibration_curve.png)

- The ensemble of model performed better than individual model, we can also try weights ensemble and stacking. Plus data oversampling of minority instances classes and undersampling of overlapping instances using imblearn library.

### Confusion Matrix
![](https://github.com/sudhanshu2198/Multi-Class-Credit-Score-Classification/blob/main/images/image18.png)





