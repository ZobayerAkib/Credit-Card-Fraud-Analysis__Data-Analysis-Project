# Credit Card Fraud Detection Model Analysis

In this analysis, we evaluate the performance of various machine learning algorithms on a credit card fraud detection dataset sourced from Kaggle. The models compared include Random Forest Classifier, Decision Tree Classifier, Logistic Regression, Gradient Boosting Classifier, Gaussian Naive Bayes, and K-Neighbors Classifier. The performance of these models is measured using Accuracy, Precision, Recall, and F1 Score. Below is a detailed description of each model's performance:

## Model Performance Metrics

| Algorithm                  | Accuracy (Test) | Precision (Test) | Recall (Test) | F1 Score (Test) |
|----------------------------|-----------------|------------------|---------------|-----------------|
| RandomForestClassifier     | 0.999596        | 0.962963         | 0.795918      | 0.871508        |
| DecisionTreeClassifier     | 0.999350        | 0.821053         | 0.795918      | 0.808290        |
| LogisticRegression         | 0.998929        | 0.686869         | 0.693878      | 0.690355        |
| GradientBoostingClassifier | 0.998929        | 0.803279         | 0.500000      | 0.616352        |
| GaussianNB                 | 0.993118        | 0.144928         | 0.612245      | 0.234375        |
| KNeighborsClassifier       | 0.998332        | 1.000000         | 0.030612      | 0.059406        |

## Model Analysis

1. **RandomForestClassifier**
   - **Accuracy:** 0.999596
   - **Precision:** 0.962963
   - **Recall:** 0.795918
   - **F1 Score:** 0.871508
   - **Analysis:** The RandomForestClassifier shows the highest overall performance, with excellent accuracy, precision, and a well-balanced recall, leading to a high F1 Score. This indicates that the model is very effective at identifying fraudulent transactions with minimal false positives.

2. **DecisionTreeClassifier**
   - **Accuracy:** 0.999350
   - **Precision:** 0.821053
   - **Recall:** 0.795918
   - **F1 Score:** 0.808290
   - **Analysis:** The DecisionTreeClassifier also performs well, with high accuracy and balanced precision and recall. However, it is slightly less effective than the RandomForestClassifier, as indicated by the lower precision and F1 Score.

3. **LogisticRegression**
   - **Accuracy:** 0.998929
   - **Precision:** 0.686869
   - **Recall:** 0.693878
   - **F1 Score:** 0.690355
   - **Analysis:** LogisticRegression provides moderate performance, with balanced but lower precision and recall compared to tree-based methods. This results in a lower F1 Score, indicating more false positives and negatives.

4. **GradientBoostingClassifier**
   - **Accuracy:** 0.998929
   - **Precision:** 0.803279
   - **Recall:** 0.500000
   - **F1 Score:** 0.616352
   - **Analysis:** The GradientBoostingClassifier has high precision but low recall, leading to a moderate F1 Score. This suggests it is good at identifying true positives but misses many fraudulent transactions.

5. **GaussianNB**
   - **Accuracy:** 0.993118
   - **Precision:** 0.144928
   - **Recall:** 0.612245
   - **F1 Score:** 0.234375
   - **Analysis:** Gaussian Naive Bayes shows poor performance, with low precision and F1 Score, indicating many false positives. Despite a relatively high recall, its overall effectiveness is limited.

6. **KNeighborsClassifier**
   - **Accuracy:** 0.998332
   - **Precision:** 1.000000
   - **Recall:** 0.030612
   - **F1 Score:** 0.059406
   - **Analysis:** K-Neighbors Classifier achieves perfect precision but extremely low recall, resulting in a very low F1 Score. This indicates that while it identifies very few false positives, it misses almost all fraudulent transactions, making it unsuitable for practical use.
  
## Visualiztion of Model's performance
![acc](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/22133034-5699-4f7e-ad62-45fce603c7f9)

## Roc Auc Graph

![knn_roc](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/1b97e388-d353-4209-b792-c35a05e2e2b3)
![Roc_dt](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/81ada124-4d82-4ed1-bf98-47bda53e93aa)
![roc_gradientboost](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/4a99913f-e45d-40fd-bfe9-355403a67af0)
![roc_log](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/bff5eed9-bbdb-4643-ab30-8bad918f7d47)
![roc_nb](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/7bbc7bc2-1bf5-4f98-9010-f23d3a0d3a0d)
![roc_rdf](https://github.com/ZobayerAkib/Credit-Card-Fraud-Analysis__Data-Analysis-Project/assets/66842328/58374bec-f738-4901-a8d6-69a8aba10b6c)

## Conclusion

Based on the evaluation metrics, the **RandomForestClassifier** emerges as the best-performing model for credit card fraud detection, offering the best balance between precision, recall, and F1 Score. This makes it the most reliable choice for identifying fraudulent transactions while minimizing false positives.

## Data Source

The dataset used for this analysis is sourced from [Kaggle].

