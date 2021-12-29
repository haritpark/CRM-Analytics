# Campaign Response Model
## Import Dataset
The datasets containing 2 file.
  - Retail_Data_Response is the data of customer level and containing customer id and response.
  - Retail_Data_Transactions is the data of transaction level and containing customer id, transaction date and transaction amount.
## Prepare Data
The features are generated for recency, frequency, monetary, AOU and ticket_size before train model. The data is imbalance and Response rate in the dataset is 9.4% as below.

![image](https://user-images.githubusercontent.com/47063720/147652572-7bf4c5a1-5854-4772-992c-9928850eb9b5.png)

## EDA
The features should be analysis to be ensure the characteristics

![image](https://user-images.githubusercontent.com/47063720/147652832-b21a291d-4878-4f79-892e-0c70e68d2d95.png)
For the features in model should not correlate with other features.

![image](https://user-images.githubusercontent.com/47063720/147652906-d701b256-84fa-4803-8e11-051f73599791.png)

## Hyperparameter tuning and Cross validation
The model parameter estimation depend on the type of model. The parameters are necessary to be fine-tuned to arrive at a robust model. Grid-Search was performed to identify the best parameters.
The optimal parameters sets were chosen by analyzing the model predictive power of train and test sample to aim at a model with strong predictive power and generalization.
For Cross validation using K-fold (k=3)

## Evaluate Model
ROC Curve of Train and Test data

![image](https://user-images.githubusercontent.com/47063720/147653419-002edbfd-c04a-45d8-9257-d9a00a1e71a4.png)

## Feature Importance
Feature importance is measured by gain. Gain is the average gain in predictive power when the feature is used as split. Feature importance are shown as below.

![image](https://user-images.githubusercontent.com/47063720/147675638-c9c5d210-895a-4fff-adb0-43cfa7a57e7b.png)

## Monotonicity
The monotonic relationship between features and prediction proability was calculated using Spearman Correlation. 

![image](https://user-images.githubusercontent.com/47063720/147676118-f0f30be3-c16b-49e3-aa60-e6f5d47e912b.png)

## Partial Dependence Plot (PDP)
The partial dependence plot (short PDP or PD plot) shows the marginal effect a feature has on the predicted outcome of a model.

![image](https://user-images.githubusercontent.com/47063720/147676298-c52b0ee7-cf9d-4321-8016-18dc500f6715.png)

# Feature Contribution
SHAP value explain individual predictions and show the impact of having a certain value for a given feature in comparison to the prediction we'd make if that feature took some baseline value.

![image](https://user-images.githubusercontent.com/47063720/147676642-968c5467-7150-4384-9b9c-2c304ac0c54b.png)
![image](https://user-images.githubusercontent.com/47063720/147676649-1cb550d5-5c8d-4e42-a1b6-9b0a584c02ca.png)



