# 🧠 CNN Development on Custom Dataset

**Course:** Computer Vision and Pattern Recognition (CVPR)  
**Assignment:** Mid Assignment – CNN Development on Custom Dataset  
**Student ID:** 23-50117-1  
**Framework:** PyTorch  
**Dataset:** Beans (Hugging Face)

---

## 📌 Project Overview

This project focuses on developing and training a custom Convolutional Neural Network (CNN) to classify bean leaf images into three different categories.

The model is implemented using PyTorch. The project includes dataset exploration, image preprocessing, data augmentation, CNN architecture development, model training, validation, and performance evaluation.

## 🎯 Objectives

- Load and explore a multi-class image dataset.
- Apply image preprocessing and data augmentation.
- Design a custom CNN architecture.
- Train and validate the model using PyTorch.
- Evaluate model performance on unseen test data.
- Save the trained model weights.

## 📂 Dataset Information

**Dataset:** Beans  
**Source:** [Hugging Face – AI-Lab-Makerere/beans](https://huggingface.co/datasets/AI-Lab-Makerere/beans)

The dataset contains three classes:

1. Bean Angular Leaf Spot
2. Bean Rust
3. Healthy Bean Leaves

## ⚙️ Data Preprocessing

The following preprocessing techniques were applied:

- Image resizing to 128 × 128 pixels.
- Conversion of images into tensors.
- Normalization of image values.
- Random horizontal flipping.
- Random rotation for training augmentation.

Training, validation, and testing datasets were used to develop and evaluate the model.

## 🏗️ CNN Architecture

A custom CNN architecture was developed using PyTorch.

The architecture consists of:

- Three convolutional blocks.
- Convolutional layers with 32, 64, and 128 channels.
- Batch Normalization.
- ReLU activation functions.
- Max Pooling layers.
- Adaptive Average Pooling.
- Dropout regularization.
- Fully Connected classification layer.

The final output layer predicts one of the three bean leaf categories.

## 🧪 Training Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | CrossEntropyLoss |
| Learning Rate | 0.001 |
| Batch Size | 32 |
| Epochs | 15 |
| Weight Decay | 0.0001 |
| Image Size | 128 × 128 |

The best model checkpoint was selected based on validation loss.

## 📊 Model Evaluation Results

The model was evaluated on the test dataset.

| Metric | Score |
|---|---:|
| Test Accuracy | 77.34% |
| Macro Precision | 0.7813 |
| Macro Recall | 0.7743 |
| Macro F1-Score | 0.7663 |

The healthy class achieved the highest class-wise F1-score, while bean_rust was the weakest-performing class.

## 📈 Visualizations

The notebook includes:

- Sample images from the dataset.
- Training and validation loss curves.
- Training and validation accuracy curves.
- Confusion matrix.
- Classification report.

These visualizations help analyze model performance and identify classification errors.

## 💾 Model Weights

The trained model weights are saved in:

`best_beans_cnn.pth`

The saved weights can be loaded later for model evaluation or inference.

## 🔮 Future Improvements

- Experiment with deeper CNN architectures.
- Tune hyperparameters for better performance.
- Apply additional data augmentation techniques.
- Address possible class imbalance.
- Compare the custom CNN with transfer learning models such as ResNet and MobileNet.

## 📁 Repository Structure

```text
CNN-Assignment/
│
├── CNN_23-50117-1.ipynb
├── best_beans_cnn.pth
└── README.md
```

## 🛠️ Technologies Used

- Python
- PyTorch
- Hugging Face Datasets
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab
- GitHub

---

**Developed as part of the CVPR Mid Assignment.**

**Student ID:** 23-50117-1
