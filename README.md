# 🌾 Rice Leaf Disease Detection using Deep Learning

## 📌 Project Overview
This project focuses on building a **deep learning-based image classification system** to identify major rice leaf diseases. The goal is to assist in **early disease detection**, helping reduce crop loss and improve agricultural productivity.

The model classifies rice leaves into three disease categories:
- Leaf Smut  
- Brown Spot  
- Bacterial Leaf Blight  

---

## 🎯 Business Objective
To develop an automated and scalable solution that can accurately detect rice leaf diseases from images, enabling faster diagnosis and supporting farmers in taking timely action.

---

## 🧠 Problem Type
- Supervised Learning  
- Multiclass Image Classification  
- Domain: Agriculture + Computer Vision  

---

## 📂 Dataset Details
- Total Images: 120  
- Classes: 3  
- Images per Class: 40 (Balanced Dataset)  
- Format: JPG Images  

---

## ⚙️ Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib / Seaborn  
- Keras Tuner  

---

## 🔍 Approach

### 1. Data Preparation
- Loaded images using `image_dataset_from_directory`
- Converted images into NumPy arrays
- Normalized pixel values (0–1 scaling)

### 2. Model Building (CNN)
- Convolutional layers for feature extraction  
- MaxPooling layers for dimensionality reduction  
- Fully connected dense layers  
- Softmax output layer for classification  

### 3. Data Augmentation
- Applied transformations such as rotation, flipping, and zoom  
- Improved model generalization on unseen data  

### 4. Hyperparameter Tuning
- Used **Keras Tuner (RandomSearch)**  
- Tuned filters, dense units, dropout, and learning rate  

---

## 📊 Model Performance

| Model | Accuracy |
|--------|----------|
| CNN | 94.736844% |
| Data Augmentation | 94.736844% |
| Keras Tuner | 100.000000% |

---

## 📈 Key Insights
- CNN successfully captured disease patterns like spots, discoloration, and textures  
- Data augmentation improved robustness but did not significantly change accuracy  
- Hyperparameter tuning led to a noticeable improvement in model performance  
- Small dataset size can lead to overfitting (especially with 100% accuracy)  

---

## ⚠️ Challenges Faced
- Limited dataset size (only 120 images)  
- Overfitting risk due to small data  
- Pooling layer configuration caused dimension errors  
- Manual hyperparameter tuning was time-consuming  

---

## 📚 Learnings
- Importance of proper CNN architecture design  
- Role of data augmentation in improving generalization  
- Hyperparameter tuning significantly impacts performance  
- Validation strategy is crucial for small datasets  

---

## 💡 Future Improvements
- Use Transfer Learning (ResNet, MobileNet, EfficientNet)  
- Increase dataset size for better generalization  
- Deploy model using Streamlit for real-time predictions  
- Use cross-validation for more reliable evaluation  

---

## 🚀 How to Run the Project

```bash
# Clone the repository
git clone https://github.com/your-username/rice-leaf-disease-detection.git

# Navigate to project folder
cd rice-leaf-disease-detection

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook
```
---

## 👩‍💻 Author
**Sejal Kumari**  
Aspiring Data Analyst / Data Scientist  

---

## ⭐ If you found this project useful, feel free to give it a star!
