# Classification-Problem-on-Breast-Cancer-Dataset
Using Classification Algorithms on Breast Cancer Dataset available in the Sklearn library
## Loading and Preprocessing
Load the Breast Cancer Dataset:
loaded the Dataset Breast Cancer from Sklearn,The dataset contains 30 features and a target variable indicating benign or malignant tumors
Handling Missing Values:
checked the null values ,info(),describe()
drop missing values if any are found , in this dataset there was no missing data or null values
Feature Scaling:
Implemented StandardScaler, several normalizations and Scaling were executed on the dataset before their use in training to bring uniformity in the range of inputs.
Feature Scaling serves to ensure that all of these features contribute fairly in distances algorithms or hyperplane-based functions
Handling missing values avoids biased training due to possible insufficient data.
## Classification Algorithm Implementation
Implemented the Classification Algorithms
1. Logistic Regression
   Logistic Regression works by modeling the probability of the target class using a linear relationship between the features and the log-odds. It is suitable for the breast cancer dataset because of its binary       nature, interpretability, and the relatively linear relationships observed in the data.
2. Decision Tree Classifier
   It's a good choice for the breast cancer dataset as it handles complex feature interactions and gives interpretable results while requiring minimal preprocessing. Being able to choose the most informative          features at every step helps differentiate malignant and benign tumors effectively.
3. Random Forest Classifier
   Thus, Random Forest is suitable because it combines the best points of Decision Trees, with the ability to handle such non-linear relationships, by addressing their weaknesses, where it prevents overfitting. It    can rank in feature importance and give strong high accuracies, making it such an elegant choice for distinguishing between tumor malignancy and benign ones.
4. Support Vector Machine (SVM)
   SVM is suitable for the breast cancer dataset due to its ability to handle high-dimensional data, robustness against overfitting, and capacity to model non-linear relationships through kernels. Proper            preprocessing, such as feature scaling, and hyperparameter tuning would make SVM very accurate in distinguishing between malignant and benign tumors.
5. k-Nearest Neighbors (k-NN)
   k-NN is a good choice for the breast cancer dataset, as it is easily capable of modeling non-linear decision boundaries, is simple, and has proven effective on small datasets. Proper preprocessing (like          feature scaling) and a suitably chosen k make k-NN competitive with other classifiers in terms of performance on distinguishing between malignant and benign tumors.
## Model Comparison
               |index |         Model        | Accuracy | Precision | Recall | F1 Score |
               |  0   | Logistic Regression  | 0.9736   | 0.9722    | 0.9859 | 0.9790   |
               |  1   | Decision Tree        | 0.9298   | 0.9436    | 0.9436 | 0.9436   |
               |  2   | Random Forest        | 0.9649   | 0.9589    | 0.9859 | 0.9722   |
               |  3   | SVM                  | 0.9824   | 0.9726    | 1.0000 | 0.9861   |
               |  4   | k-Nearest Neighbors  |,0.9473   | 0.9577    | 0.9577 | 0.9577   |

From this we Can understand that
After testing several classification algorithms on the breast cancer dataset, SVM obtained the highest accuracy of 98.2%, suggesting that it is capable of successful classification between malignant and benign tumors. The F1-Score, which combines precision and recall and is vital in this application where false positives and false negatives both have severe repercussions, is 98.6% for SVM.
The lowest is Decision Tree, even if its accuracy remained at 92.9%. It is likely overfitting as individual decision trees tend to capture noise within the training data, reducing their ability to generalize.
## Conclusion
Comparing with other Algorithm in this dataset on the bases of accuracy ,precision,recall,f1score we get more favorable model as

Best: SVM 

Worst: Decision Tree
