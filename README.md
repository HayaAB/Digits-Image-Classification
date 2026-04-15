# 🔢 Digits Image Classification using PyTorch

This project builds a Neural Network model using PyTorch to classify handwritten digit images (0–9) from the Digits dataset.

---

# 📌 Project Overview

The goal of this project is to train a deep learning model to recognize handwritten digits based on pixel values.

Dataset used:
- sklearn Digits Dataset
- 1797 grayscale images
- Image size: 8×8 pixels
- 10 classes (digits 0–9)

---

# 📊 Dataset Information

Total samples: 1797  
Image shape: 8 × 8  
Flattened features: 64  
Number of classes: 10  

Pixel values range:
0 → 16

---

# 🔍 Exploratory Data Analysis (EDA)

Performed the following:

- Visualized sample digit images
- Checked class distribution
- Analyzed pixel value distribution
- Verified min/max pixel values
- Observed balanced class distribution

---

# ⚙️ Data Preprocessing

Steps:

- Flattened images from (8×8) → (64)
- Split dataset into:
  - Training set: 1437 samples
  - Test set: 360 samples
- Converted NumPy arrays into PyTorch tensors

---

# 🧠 Model Architecture

```python
Sequential(
  Linear(64 → 32)
  ReLU()
  Linear(32 → 16)
  ReLU()
  Linear(16 → 10)
)
```
---
Model Type:
Fully Connected Neural Network

Activation Function:
ReLU

Loss Function:
CrossEntropyLoss

Optimizer:
Adam (lr=0.001)

Training:
200 epochs
---
# 📉 Training Performance

Loss decreased steadily during training:

Example:

Epoch 0 → Loss ≈ 2.02
Epoch 180 → Loss ≈ 0.28

This indicates successful learning.
---
# 📊 Model Evaluation

Accuracy: 94%
Confusion Matrix

Shows strong performance across all digit classes with minimal misclassifications.

Most confusion occurred between visually similar digits such as:
	•	9 and 7
	•	8 and 1
	•	2 and 3

Classification Report

Average Scores:
Precision: 0.94
Recall: 0.94
F1-score: 0.94
---
# 🖼️ Sample Predictions

Displayed predicted digits alongside true labels to visually verify performance.

Example:

P:7 T:7 → Correct
P:3 T:2 → Misclassified
---
# 🚀 Technologies Used
	•	Python
	•	PyTorch
	•	NumPy
	•	Matplotlib
	•	Seaborn
	•	Scikit-learn
  ---
  # 📌 Key Learning Outcomes

Through this project, I learned:
	•	Neural Network design using PyTorch
	•	Image classification fundamentals
	•	Data preprocessing for deep learning
	•	Model training and evaluation
	•	Performance analysis using confusion matrix
	•	Visualization of predictions
  ---
  
