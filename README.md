🫁 Pneumonia Detection using Deep Learning (ResNet)

A deep learning project that detects pneumonia from chest X-ray images using transfer learning with ResNet.
The model achieves high recall for pneumonia cases, making it suitable for medical screening support.

🚀 Results
Test Accuracy: 87%
F1 Score: 0.87
Recall (Pneumonia): 99%
Strong performance on imbalanced medical dataset

🧠 Approach
Used ResNet18 (pretrained on ImageNet) for transfer learning
Replaced final layer for binary classification (NORMAL vs PNEUMONIA)
Applied data augmentation (rotation, flipping)
Handled class imbalance using weighted loss function
Evaluated using precision, recall, F1-score, confusion matrix

📊 Dataset
Source: Kaggle Chest X-ray Pneumonia Dataset
Contains labeled chest X-ray images:
NORMAL
PNEUMONIA
Dataset split:
Train
Validation
Test

⚙️ Model Details
Architecture: ResNet18
Input size: 224 × 224
Loss: CrossEntropyLoss with class weights
Optimizer: Adam
Epochs: 5 (trained on Google Colab GPU)

🔍 Explainability (Grad-CAM)
Used Grad-CAM to visualize regions of the X-ray that influenced model predictions.
Helps verify that the model focuses on lung regions instead of irrelevant areas.
