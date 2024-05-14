# Credit Card Fraud Detection

This repository contains code for detecting fraudulent transactions in credit card data. The project utilizes machine learning models to classify transactions as either fraudulent or legitimate. Below is an overview of the approach taken and the key steps involved:

## Approach
1. **Data Acquisition**: The Credit Card Fraud Detection dataset from Kaggle is used. This dataset contains transactions made by credit cards in September 2013 by European cardholders. It is highly imbalanced, with a small number of fraudulent transactions compared to legitimate ones.

2. **Data Preprocessing**: The dataset is preprocessed to prepare it for model training. This includes scaling the features, splitting the data into training, validation, and testing sets, and addressing class imbalance using techniques like undersampling.

3. **Model Training**: Several machine learning models are trained using the preprocessed data. The models used include Logistic Regression, Gradient Boosting Classifier, Random Forest Classifier, and a Shallow Neural Network. Hyperparameter tuning is performed to optimize model performance.

4. **Model Evaluation**: The trained models are evaluated using various metrics such as accuracy, precision, recall, and F1-score. The performance of each model is compared, and the best-performing model is selected for further analysis.

5. **Ensemble Learning**: An ensemble of the best-performing models is created using the Voting Classifier technique. This ensemble model combines the predictions of multiple base models to improve overall performance.

## Key Results

### Validation Data
- The ensemble model achieved an accuracy of 93% on the validation set.
- For the "Not Fraud" class, the ensemble model achieved a precision of 88%, recall of 100%, and F1-score of 94%.
- For the "Fraud" class, the ensemble model achieved a precision of 100%, recall of 86%, and F1-score of 92%.
- The macro-average F1-score for the ensemble model on the validation set is 93%.

### Test Data
- The ensemble model achieved an accuracy of 93% on the test set.
- For the "Not Fraud" class, the ensemble model achieved a precision of 88%, recall of 100%, and F1-score of 94%.
- For the "Fraud" class, the ensemble model achieved a precision of 100%, recall of 86%, and F1-score of 92%.
- The macro-average F1-score for the ensemble model on the test set is 93%.

The ensemble model demonstrates robust performance on both the validation and test datasets, with high accuracy and balanced precision, recall, and F1-scores for both classes. These results validate the effectiveness of the ensemble approach in detecting credit card fraud.

## Conclusion

In summary, both the Shallow Neural Network (shallow_nn) and the Ensemble Model demonstrate strong performance in detecting credit card fraud:

### Shallow Neural Network (shallow_nn)
- Achieved an accuracy of 93% on the validation set and 91% on the test set.
- Demonstrated high precision, recall, and F1-scores for both "Not Fraud" and "Fraud" classes.
- Showed consistent and robust performance across both datasets.

### Ensemble Model
- Achieved an accuracy of 93% on both the validation and test sets.
- Balanced precision, recall, and F1-scores for both classes, indicating effective fraud detection.
- Leveraged the strengths of multiple models to improve overall performance.

The Ensemble Model combines the predictions of multiple base models, including Logistic Regression, Gradient Boosting Classifier, and Random Forest Classifier, using the Voting Classifier technique. By integrating diverse model predictions, the ensemble approach enhances the overall fraud detection capabilities.

In conclusion, both the Shallow Neural Network and the Ensemble Model exhibit promising results in detecting credit card fraud. Further optimization and fine-tuning of these models could potentially enhance their performance and contribute to more effective fraud detection systems.
