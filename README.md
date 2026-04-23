# CNN-image-classification-using-FASHIN-MNIST-dataset
🧠 Fashion-MNIST CNN Classifier (PyTorch)
📌 Project Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images from the Fashion-MNIST dataset. The model learns to recognize different types of clothing items from grayscale images.

The goal is to demonstrate the application of deep learning and CNNs in computer vision tasks.

📂 Dataset
Dataset: Fashion-MNIST
Source: Kaggle (via kagglehub)
Total Images:
Training: 60,000
Testing: 10,000
Image Size: 28 × 28 pixels (grayscale)
Classes (10 categories):
T-shirt/top
Trouser
Pullover
Dress
Coat
Sandal
Shirt
Sneaker
Bag
Ankle boot
⚙️ Technologies Used
Python
PyTorch
NumPy
KaggleHub
Matplotlib (optional for visualization)
🏗️ Project Structure
Fashion-MNIST-CNN/
│
├── data/                     # Dataset files (auto-downloaded)
├── model.py                 # CNN model definition
├── train.py                 # Training script
├── README.md                # Project documentation
└── notebook.ipynb           # Jupyter Notebook (optional)
🧠 Model Architecture
CNN Structure:
Conv Layer 1 → 32 filters → ReLU → MaxPool
Conv Layer 2 → 64 filters → ReLU → MaxPool
Fully Connected Layer → 128 neurons
Dropout (0.5)
Output Layer → 10 classes
🔄 Workflow
Download dataset using kagglehub
Load IDX files (binary format)
Preprocess images (normalize to [0,1])
Build CNN model
Train model using Adam optimizer
Evaluate accuracy on test dataset
🚀 How to Run
1. Install dependencies
pip install torch torchvision kagglehub numpy
2. Run the script
python train.py
📊 Results
Training Loss decreases over epochs
Test Accuracy: ~88% – 92%

(Accuracy may vary depending on hardware and epochs)

⚠️ Important Notes
Dataset files may be:
.gz (compressed) OR
extracted binary files
Code handles both formats
IDX format requires manual parsing using byte offsets
🔍 Key Learnings
Understanding CNN architecture
Working with raw dataset formats (IDX)
Implementing training loops in PyTorch
Evaluating classification models
🔮 Future Improvements
Add Batch Normalization
Use Data Augmentation
Improve accuracy to 95%+
Add confusion matrix & visualization
Deploy model using Flask or Streamlit
🤝 Contributing

Contributions are welcome! Feel free to fork and improve the project.

📜 License

This project is open-source and available under the MIT License.
