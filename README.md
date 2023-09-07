# Sunbase-Customer-Churn-Prediction

### Introduction
Sunbase prioritize understanding our customers and ensuring their satisfaction. To achieve this, they want to develop a machine learning model that predicts customer churn based on historical customer data and 
will follow a typical machine learning project pipeline, from data preprocessing to model deployment.

Work Process
1. Data Preprocessing
2. Feature Engineering
3. Data Viz
4. Model Building
5. Model Optimization
6. Model Deployment

Conclusion
I used Jupiter Notebook to perform Python coding to achieve the targeted result. This project is divided into 5 parts as mentioned above in the work process section.

For final Model deployment I chose AdaBoostClassifier because it has the highest accuracy rate for the test and train dataset.

#### Here is detail about AdaBoost Classifier:

AdaBoost (Adaptive Boosting) is a popular ensemble learning technique used for classification tasks in machine learning. It is a boosting algorithm, which means it combines the predictions of multiple weak learners (typically decision trees) to create a strong classifier. AdaBoost is designed to improve the accuracy of the model by giving more weight to the examples that are misclassified by the previous weak learners in the ensemble.

#### A step-by-step explanation of how AdaBoost works:

1. Initialize Sample Weights: At the beginning, each training example is assigned an equal weight. These weights determine the importance of each example in the training process.

2. Training Weak Learners: AdaBoost iteratively trains a series of weak learners (usually decision trees with limited depth or "stumps"). In each iteration, it selects the weak learner that performs best on the weighted training data. The performance is measured in terms of how well the learner classifies the examples.

3. Weighted Training: During each iteration, AdaBoost gives more weight to the examples that were misclassified by the previous weak learners. This emphasizes the examples that are difficult to classify, forcing the algorithm to focus on them.

4. Combine Weak Learners: After each weak learner is trained, AdaBoost assigns a weight to it based on its accuracy. The more accurate a weak learner is, the higher its weight in the final model.

5. Final Ensemble: AdaBoost combines the weighted weak learners to create a strong classifier. The final prediction is made by taking a weighted majority vote or weighted average of the individual weak learner predictions. The more accurate weak learners have a greater influence on the final prediction.

6. Iterate: Steps 2-5 are repeated for a predetermined number of iterations or until a specific accuracy threshold is reached.

7. Final Model: The resulting ensemble model is a weighted combination of the weak learners, with each learner's weight determined by its accuracy. This model is used to make predictions on new, unseen data.

AdaBoost has several advantages, including its ability to handle complex datasets and its resistance to overfitting. However, it can be sensitive to noisy data and outliers. To mitigate this, robust weak learners like decision stumps are often used.

