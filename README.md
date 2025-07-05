# Stop Detection - CNN in PyTorch

This project implements a custom Convolutional Neural Network (CNN) from scratch using PyTorch to detect **STOP signs** in static images. The architecture is lightweight and designed for binary classification without relying on pretrained models.

## Project Structure
Stop_Detection/

├── notebooks/ # Training and evaluation notebooks

│ └── Stop_detection.ipynb

├── not_stop/ # Dataset used for training and validation

├── stop/ # Dataset used for training and validation

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
 
 ![Captura de pantalla 2024-08-15 174344](https://github.com/user-attachments/assets/1c7ab027-c87b-4937-ab66-b19e2e084bdb)


- **Validation Accuracy**: 85%
- **Observations**:
  - The model generalizes well to unseen STOP sign images.
  - Some confusion with similar-shaped signs suggests possible improvements via data augmentation or deeper architectures.



## 🚀 How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/LordAmadeus1/Stop_Detection.git
   cd Stop_Detection

2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt

3. **Open the notebook:**

   Launch Stop_detection.ipynb in Google Colab or a local Jupyter environment.

    Run each cell sequentially to process the video frames and detect stop signs.


This project is licensed under the MIT License
