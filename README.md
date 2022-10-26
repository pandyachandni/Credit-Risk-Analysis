# Credit-Risk-Analysis
# Overview of Analysis
Credit risk can be very tough to predict. This project will help us take a look in all the factors determine in the loan_stats csv to help see if someone is low or high risk. Data scientists create models that are trained to evaluate if someone is high or low risk. This specific project uses imbalanced-learn and scikit-learn libraries to build models and evaluate them using the resampling method.

# Results
Naive Random Oversampling Results:
The balanced accuracy test is at 65%. The Precision for the high_risk is very low at 1% and the recall is at 74%.
<img width="829" alt="Screen Shot 2022-10-25 at 9 38 00 PM" src="https://user-images.githubusercontent.com/107590706/197914200-78986655-777a-488d-bc2c-1bd3098b29ac.png">

SMOTE Oversampling Results:
The accuracy score is 66.2%. The precison for high risk loans was low again(which is good) at 1%. The recall was at 69% overall.
<img width="831" alt="Screen Shot 2022-10-25 at 9 41 07 PM" src="https://user-images.githubusercontent.com/107590706/197914562-5f0fe33d-33aa-4bd9-8c47-6bb36820dff2.png">

Undersampling Results:
The balanced accuracy score was at 54.4% overall. The precision is at 99% and the recall is at 42%.
<img width="825" alt="Screen Shot 2022-10-25 at 9 43 51 PM" src="https://user-images.githubusercontent.com/107590706/197914941-225842d5-ef4b-4f55-8a5b-342ba379db5d.png">

Combination(over and undersampling) Results:
The balanced accuracy score is at 64%. The precision is at 99% and the recall is at 58% overall.
<img width="833" alt="Screen Shot 2022-10-25 at 9 46 56 PM" src="https://user-images.githubusercontent.com/107590706/197915428-fd84ebb9-ffaf-4f29-8fdd-782e3ec6df6b.png">

Easy Ensemble AdaBoost Classifier Results:
The accuracy score is at 93.2% and the precision is 99% overall and the recall is 94% overall.
<img width="846" alt="Screen Shot 2022-10-25 at 9 49 29 PM" src="https://user-images.githubusercontent.com/107590706/197915676-afc50329-bdcb-466e-8a5f-36b0cb3f10ed.png">

# Summary
The first four models undersampled, oversampled then took a combination of both to try and see which of the four models is the best at predicting which loans are high risk. The two models that followed after resampled the data using ensemble classifers to try and predict which loans were either low or high risk. In the first four models the accuracy was not as high as the ensemble classifers. The recall in these models were low as well. In most models you typically want a balance of precision and recall which is why once they are enabled by ensemble classifers it gives the best of both worlds.
