📌 Overview

This project implements a Deep Learning–based Plant Disease Detection System using EfficientNetB4.
It is designed to automatically classify plant leaf images into different disease categories.

The model uses Transfer Learning and Fine-Tuning, making it highly accurate even with limited training data.
Dataset preparation, visualization, training, evaluation, and prediction are all included.

🌟 Features

✔ Accurate plant leaf disease classification
✔ Pre-trained EfficientNetB4 model (ImageNet weights)
✔ Transfer Learning + Fine Tuning for better accuracy
✔ Automatic train/validation/test split
✔ Visualization of samples, accuracy, loss curves
✔ Predicts disease from new test images
✔ GPU-friendly (Google Colab compatible)

📂 Dataset
“Dataset used in this project is downloaded from TensorFlow’s publicly available dataset link.”

Model Architecture

EfficientNetB4 (base model)

GlobalAveragePooling2D layer

Dropout layer

Dense classification layer

Training is done in two phases:
1️⃣ Feature Extraction
Base model frozen
Only custom layers trained
Faster & prevents overfitting

2️⃣ Fine-Tuning
Unfreeze upper layers after layer index 100
Train at a lower learning rate
Improves accuracy significantly


📊 Results & Visualizations

The training notebook includes:
🟢 Training vs Validation Accuracy graph
🔵 Training vs Validation Loss graph
🟣 Test Accuracy on unseen images
🟠 Prediction results with sample images

🛠️ Tech Stack
✔ Python
✔ TensorFlow / Keras
✔ NumPy
✔ Matplotlib
✔ split-folders
✔ EfficientNetB4

🚀 How to Run This Project
1. Clone the repository:
git clone https://github.com/your-username/plant-disease-detection.git
cd plant-disease-detection

2. Install the required libraries:
pip install -r requirements.txt
Or simply run in Google Colab (recommended).

3. Run the training notebook/script:
✔ Upload the dataset or use the provided download command
✔ Run training cells step-by-step
✔ Evaluate the model on the test dataset
✔ View prediction results

📸 Prediction Sample
The model outputs:
✔ The input test image
✔ The predicted disease label
✔ Useful for explaining the model performance visually.


🎯 Project Aim

To build a robust and efficient AI system that can automatically detect plant diseases early, helping:
✔ Farmers
✔ Researchers
✔ Agriculture-based industries
✔ By improving crop health and minimizing loss.
