# News Classification using SVM

## Overview
This project implements a Support Vector Machine (SVM) model for classifying news articles into predefined categories based on their content. The goal is to interpret the text of the articles and accurately identify the corresponding category.

## Project Objectives
- **Text Interpretation**: Analyze and categorize real news articles using machine learning techniques.
- **Category Identification**: Develop a model that can effectively classify articles into 42 distinct categories.

## Methodology

### Data Exploration and Preprocessing
1. **Data Source**: The dataset used is the News Category Dataset, which contains news articles labeled with their respective categories.
2. **Visualization**: Initial analysis included visualizations to identify class imbalance among the 42 categories present in the dataset.
3. **Balancing the Dataset**: To improve the model's performance, we employed techniques such as oversampling to restore balance among categories.

### Model Selection and Training
1. **Vectorization**: We used Grid Search to optimize the vectorization process. This involved testing various parameters to find the most effective way to convert text data into numerical features for the SVM model.
2. **Model Selection**: The Stochastic Gradient Descent (SGD) classifier was used as a linear SVM model to classify the text data.
3. **Training**: The model was trained on the oversampled dataset to improve accuracy in categorizing minority classes.

### Evaluation
1. **Performance Metrics**: The model was evaluated on the original test dataset, yielding the following results:
   - **Accuracy**: 50%
   - **Macro Average Precision**: 0.45
   - **Macro Average Recall**: 0.60
   - **Macro Average F1-Score**: 0.47
   - **Weighted Average Precision**: 0.61
   - **Weighted Average Recall**: 0.50
   - **Weighted Average F1-Score**: 0.51
2. **Comparison**: The model's performance was compared to an unbalanced baseline model, which had an accuracy of 54% but lower precision and recall for critical categories.

## Results and Discussion
While the oversampled model demonstrated improved recall and F1 scores, indicating better performance on minority categories, there remains significant room for improvement. The current model's accuracy is lower than desired, highlighting the complexity of the news classification task.

### Future Work
- **Alternative Models**: Consider experimenting with different algorithms such as Random Forest (RF) or XGBoost, which may yield better performance on this dataset.
- **Feature Engineering**: Further work could include refining feature extraction techniques, experimenting with different text preprocessing methods, or incorporating additional features to improve model performance.
- **Hyperparameter Tuning**: Continued optimization of model parameters could lead to better results.

## Conclusion
This project illustrates the challenges and opportunities in using machine learning for text classification tasks. Although the current SVM model shows promise, further refinements and alternative approaches could enhance classification accuracy and robustness.
