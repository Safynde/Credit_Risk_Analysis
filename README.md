# Credit_Risk_Analysis 

# Overview 

There are different techniques to train and evaluate models with unbalanced classes. This project focused on using imbalance-learn and scikit- learn libraries to build and evaluate models using resampling. The procedure adopted for the project are: 
•	Oversampling the data using the Naive Randomoversampler 
•	Undersampling the data using the ClusterCentroids algorithm.
•	Use a combinatorial approach of over- and Undersampling using the SMOTEENN algorithm.

# Results 

## Naive RandomOverSampling Model

![image](https://user-images.githubusercontent.com/101475984/184223032-e6bae622-f935-4250-b8b4-5107f4a0e7c7.png)

![image](https://user-images.githubusercontent.com/101475984/184223059-0e2a60c8-3ef0-430a-b154-200102a1f786.png)

•	The balanced accuracy score is 65%.
•	The high-risk precision is about 1% with 74% sensitivity, which only makes an F1 of 2%.
•	Due to the high number of the low-risk population, its precision is almost 100%, with a sensitivity of 55%.

## SMOTE oversampling 

![image](https://user-images.githubusercontent.com/101475984/184223362-a1a5c237-c1e9-421c-bdbc-37ccca89c308.png)

![image](https://user-images.githubusercontent.com/101475984/184223398-9363e06e-1931-4fb8-9e26-f021e5a57a3b.png)

•	The balanced accuracy score is 64%.
•	The high-risk precision is about 1% only with 63% sensitivity which makes an F1 of 2% only.
•	Due to the high number of the low-risk population, its precision is almost 100%, with a sensitivity of 69%.

## Undersampling

![image](https://user-images.githubusercontent.com/101475984/184223800-54b36c10-c52f-4264-b01a-78046da01ded.png)

![image](https://user-images.githubusercontent.com/101475984/184223829-73cfd47e-1ce6-4620-a6c9-e7e733e5b18d.png)

•	Here the balanced accuracy score is down to about 54%.
•	The high_risk precision is still 1% only with 67% sensitivity which makes an F1 of 1%.
•	Due to the high number of false positives, the low-risk sensitivity is only 42%.

## Combination Sampling

![image](https://user-images.githubusercontent.com/101475984/184224006-6c11ad9e-d50a-423b-964e-4ff1dee3d4a6.png)

![image](https://user-images.githubusercontent.com/101475984/184224042-473c7d6e-6df5-486e-a73f-6321c3848a12.png)

•	The balanced accuracy score is about 64%.
•	The high-risk precision is still 1% only with 70% sensitivity which makes an F1 of only 2%.
•	Due to the high number of false positives, the low-risk sensitivity is 58%.

# Summary 

All the models used to perform the credit risk analysis show weak precision in determining if credit risk is high.
With a low precision, many low-risk credits are still falsely detected as high risk, which would penalize the bank's credit strategy and infer its revenue by missing those business opportunities.For those reasons, it would not be recommended to use any of these models to predict credit risk.

