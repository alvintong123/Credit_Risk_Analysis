# Credit_Risk_Analysis 
## Overview 
The purpose of this analysis is to evaluate a credit risk model that looks to identify individuals who are at high credit risk based on their loan status. 
## Results 
* Naive Random Oversampling 
  * The accuracy score is 0.65 which is not good 
  * The precision score is heavily skewed toward low risk individuals 
  * The recall score is somewhat low with low risk being 0.66 and high risk being 0.64  
<img width="708" alt="image" src="https://user-images.githubusercontent.com/111672553/213042928-2c47a02f-4f1a-4511-89fb-a7ebc24737e5.png">
* SMOTE Oversampling 
  * The accuracy score is 0.62 which is not good 
  * The precision score is heavily skewed toward low risk individuals 
  * The recall score is somewhat low amongst low risk being 0.66 while high risk is low being 0.59  
<img width="709" alt="image" src="https://user-images.githubusercontent.com/111672553/213043066-039cae71-3cfc-4f8e-bb5b-da973d705927.png">
* Undersampling 
  * The accuracy score is 0.64 which is low 
  * The precision score is heavily skewed toward low risk individuals 
  * The recall score is higher among high risk individuals at 0.61 while low risk is 0.57 
<img width="707" alt="image" src="https://user-images.githubusercontent.com/111672553/213043258-942b64ec-a672-405d-8de7-fae9ece9fd9d.png">
* Combination 
  * The accuracy score is 0.64 which is low 
  * The precision score is heavily skewed toward low risk individuals 
  * The recall score is higher among high risk individials at 0.70 while low risk is 0.57  
<img width="716" alt="image" src="https://user-images.githubusercontent.com/111672553/213043411-899b108e-8aa1-40ab-8798-4cd7af9e4ea9.png">
* Balanced Random Forest Classifier 
  * The accuracy score is 0.79 which is good 
  * The precision score is skewed toward low risk individuals, 1.00 for low risk and 0.04 for high risk
  * The recall score is at 0.91 for low risk individuals and high risk is 0.68
<img width="711" alt="image" src="https://user-images.githubusercontent.com/111672553/213043588-13f71399-7b67-4679-bc52-3cdd6164e637.png"> 
* Easy Ensemble AdaBoost Classifier 
  * The accuracy score is 0.93 
  * The precision score is skewed toward low risk individuals, 1.00 for low risk and 0.07 for high risk 
  * The recall score is 0.91 for high risk and 0.94 for low risk 
<img width="715" alt="image" src="https://user-images.githubusercontent.com/111672553/213043814-516137fc-6d0d-4488-b88c-81e2c0d424dc.png">
## Summary 
Overall, the majority of the models performed veyr poorly the resampled models barely had an accuracy score of above 0.70 which is not really ideal in addition to having poor recall scores. The ensemble models were much better in boasting higher accuracy scores and higher recall scores for both cases. On e thing each model did have in common though was having precision scores heavily skewed toward low risk individuals. I would recommend the Easy Ensemble AdaBoost Classifier because it had the highest accuracy scores amongst the modles and higher recall scores, unfortunately it suffered the same flaw with the precision scores as did the other models.
