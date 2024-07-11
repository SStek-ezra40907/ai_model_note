# AI in Medical Applications

## Machine Learning Algorithms

### Deep Learning
- **Convolutional Neural Networks (CNNs)**:
  - **Applications**: Medical image analysis, disease detection, tumor segmentation, organ localization.
  - **Architecture**: Convolutional layers, pooling layers, and fully connected layers for hierarchical feature extraction.
- **Recurrent Neural Networks (RNNs)**:
  - **Applications**: Sequential data analysis, patient health records, ECG data.
  - **Variants**: LSTM (Long Short-Term Memory) and GRU (Gated Recurrent Units) for handling long-term dependencies.

### Transfer Learning
- **Concept**: Using pre-trained models on large datasets (e.g., ImageNet) and fine-tuning them on smaller medical datasets.
- **Advantages**: Reduces the need for large amounts of labeled medical data, speeds up training, and often improves performance due to learned general features.

### Federated Learning
- **Principle**: Models are trained locally on devices or servers holding data samples, without centralizing data.
- **Application**: Collaborative learning across healthcare institutions while preserving patient data privacy.

## Data Preprocessing in Medical AI

### Normalization and Standardization
- **Normalization**: Scaling data to a range, typically [0, 1] or [-1, 1].
- **Standardization**: Transforming data to have a mean of zero and a variance of one.

### Data Augmentation
- **Techniques**: Rotating, flipping, scaling, translating images to artificially increase dataset size and improve model robustness.

### Handling Missing Data
- **Imputation**: Filling missing values with statistical estimates (mean, median) or using advanced techniques like KNN imputation.
- **Model Strategies**: Certain models like decision trees can inherently handle missing data by splitting based on available features.

## Model Evaluation Metrics

### Accuracy
- **Definition**: Proportion of correct predictions among total instances. Can be misleading in imbalanced datasets.

### Precision and Recall
- **Precision**: \( \frac{True Positives}{True Positives + False Positives} \) - Important when the cost of false positives is high.
- **Recall**: \( \frac{True Positives}{True Positives + False Negatives} \) - Crucial when missing a positive case has severe consequences.
- **F1 Score**: Harmonic mean of precision and recall, providing a single balanced metric.

### AUC-ROC Curve
- **Definition**: Area Under the Receiver Operating Characteristic curve, plotting true positive rate vs. false positive rate.
- **Use**: Evaluates model performance across various threshold settings, providing a comprehensive view of sensitivity and specificity trade-offs.
