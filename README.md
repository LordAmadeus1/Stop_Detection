# Stop Detection - CNN in PyTorch

This project implements a custom Convolutional Neural Network (CNN) from scratch using PyTorch to detect **STOP signs** in static images. The architecture is lightweight and designed for binary classification without relying on pretrained models.

## Project Structure
Stop_Detection/

├── notebooks/ # Training and evaluation notebooks

│ └── Stop_detection.ipynb

├── data/ # Dataset used for training and validation

├── images/ # Sample results and visualizations

└── README.md

## Model Architecture

- **Input**: RGB images resized to 224x224 pixels.
- **Layers**:
  - 3 convolutional layers with ReLU activations
  - Pooling layers for downsampling
  - Fully connected layers for classification
- **Output**: Binary prediction (STOP sign present or not)

## Training and Evaluation

- **Framework**: PyTorch
- **Optimization**:
  - Optimizer: Adam
  - Loss Function: CrossEntropyLoss
  - Learning Rate Scheduler: StepLR
- **Metrics**:
  - Accuracy
  - Confusion Matrix

 ## Results

- **Validation Accuracy**: 85%
- **Observations**:
  - The model generalizes well to unseen STOP sign images.
  - Some confusion with similar-shaped signs suggests possible improvements via data augmentation or deeper architectures.

## 🖼️ Visualizations

![Confusion Matrix](images/confusion_matrix.png)  
*Figure 1: Confusion matrix on validation set.*

![Loss Curve](images/loss_curve.png)  
*Figure 2: Loss evolution during training.*

## 🚀 How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/LordAmadeus1/Stop_Detection.git
   cd Stop_Detection

2. **Run the notebook**:
   jupyter notebook notebooks/Stop_detection.ipynb

This project is licensed under the MIT License
