# Intel-Image-Classification

1. Introduction
This project focuses on classifying images into different categories using a Convolutional Neural Network (CNN). The model is trained and evaluated on a dataset containing images of buildings, forests, glaciers, mountains, seas, and streets. The goal is to achieve high classification accuracy and analyze the model’s performance through various evaluation metrics.
2. Methodology
2.1 Data Collection & Preprocessing
•	The dataset is taken from Kaggle and fetched using Kaggle API. It consists of images belonging to six different categories.
•	Images were resized and normalized to ensure consistency in model training.
•	Data augmentation techniques such as rotation, flipping, and zooming were applied to improve model generalization.
2.2 Model Architecture
•	A CNN model was designed with multiple convolutional layers followed by max-pooling layers.
•	Batch normalization and dropout were used to enhance performance and prevent overfitting.
•	The final layers consisted of fully connected (dense) layers and a softmax activation function to classify images into six categories.
2.3 Training & Evaluation
•	The model was trained using the categorical cross-entropy loss function and Adam optimizer.
•	Accuracy and loss were monitored over several epochs.
•	A confusion matrix was generated to evaluate class-wise performance.
•	Training and validation accuracy/loss graphs were plotted to analyze the model’s learning process.


3. Results & Findings
•	The training and validation accuracy curves show steady improvement, with the model achieving over 80% accuracy.
The accuracy graph shows the progression of training and validation accuracy over epochs:
o	Initially, both training and validation accuracy are low but steadily increase as training progresses.
o	The final validation accuracy is higher than training accuracy, suggesting that the model generalizes well to unseen data.
o	The upward trend indicates that the model is learning relevant features effectively without significant overfitting.
•	3. Training and Validation Loss
The loss graph provides insights into the model’s optimization process:
o	Both training and validation loss steadily decrease, indicating that the model is effectively minimizing errors.
o	A slight fluctuation in validation loss after a few epochs is visible but remains stable towards the end, suggesting that the model has not significantly overfitted.
o	The final validation loss is lower than the initial training loss, proving that the model has improved significantly over time.
 
•	The confusion matrix highlights the model’s performance across different classes, identifying areas for potential improvement.
From the confusion matrix:
o	The model performs well in classifying glaciers, sea, and mountains, as indicated by high TP values.
o	Misclassifications occur between classes such as forest and buildings, which might share similar visual features.
 
•	Feature visualization from the first convolutional layer demonstrates how the model detects important patterns in the input images.
