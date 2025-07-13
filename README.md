# 🐶🐱 DogCat Classifier using CNN 🚀
This project is a deep learning-based binary image classification system that distinguishes between dogs and cats. It leverages **transfer learning** using a pre-trained **VGG16** model, fine-tuned for this task. The project includes a training notebook and a Streamlit-based web app for live predictions.
## 🔍 Overview

- **Model**: VGG16-based CNN with custom classification layers
- **Learning Strategy**: Transfer Learning (feature extraction and fine-tuning)
- **Deployment**: Streamlit web app
- **Input**: Images of cats and dogs
- **Output**: Predicted class label (`Dog` or `Cat`)
## 🧠 Model Architecture
The classifier harnesses the power of a CNN architecture, and we've taken it up a notch by employing the pre-trained VGG16 model through transfer learning for perfectly accurate predictions!

## 🧠 Model Details

- **Base Model**: `VGG16` from `tensorflow.keras.applications` (pre-trained on ImageNet)
- **Top Layers**:
  - GlobalAveragePooling2D / Flatten
  - Dense layers with dropout
  - Final Dense layer with sigmoid activation for binary classification
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Input Shape**: (150, 150, 3)

## 💻 Streamlit App

You can run the interactive web app to classify uploaded images:

### ▶️ Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/dog-cat-classifier.git
   cd dog-cat-classifier
