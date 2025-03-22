# 🎯 QR Code Authentication: First Print vs. Second Print  

A project to distinguish between original ("First Print") and counterfeit ("Second Print") QR codes using **SVM** and **CNN** models.  

---

## 📌 Project Overview  

This project builds a pipeline that:  
- 📥 **Loads and preprocesses QR code images**  
- 🔍 **Extracts features (Canny edges)** for SVM  
- 🧠 **Builds an enhanced CNN** with dropout and regularization  
- 🔧 **Implements early stopping and learning rate scheduling**  
- 📊 **Compares SVM vs CNN performance**  

---

## 🚀 Technologies Used  

- Python 🐍  
- TensorFlow / Keras  
- OpenCV  
- Scikit-learn  

---

## 🔧 Setup Instructions  

1️⃣ **Clone this repository:**  
```bash
git clone https://github.com/yourusername/QR-Code-Authentication.git
2️⃣ Install dependencies:

bash
Copy
Edit
pip install tensorflow opencv-python scikit-learn matplotlib
3️⃣ Run the project:

bash
Copy
Edit
python main.py
📁 Dataset Structure
Ensure your dataset is organized as follows:

sql
Copy
Edit
/QR_Dataset  
    /first_print  
        /First Print (all images)  
    /second_print  
        /Second Print (all images)  
🧠 Model Architectures
🎯 SVM (Support Vector Machine)
Feature extraction using Canny edge detection

Linear kernel for classification

🔥 CNN (Convolutional Neural Network)
3 Convolution layers with ReLU activation

Max Pooling layers

L2 Regularization (0.01)

Dropout layers (30%, 40%, 50%, 60%)

Sigmoid output for binary classification

Early stopping & learning rate scheduler

📊 Results
Metric	SVM Model	CNN Model
Precision	0.55	0.95
Recall	0.55	0.95
F1-Score	0.55	0.95
Accuracy	55%	95%
✅ CNN significantly outperforms SVM with better feature extraction and training strategies!

🔥 Future Improvements
🔧 Implement Transfer Learning with pre-trained models like MobileNet

🎯 Add data augmentation for more robust models

🚀 Build a web interface for live QR code uploads and authentication

💡 Author
Kaustubh Bhalerao
