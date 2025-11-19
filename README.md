# Waste Classification Project (Internship Submission)

## 📌 Project Overview
This project classifies household waste images into 5 categories:
- glass  
- metal  
- organic  
- paper  
- plastic  

The goal is to support automated waste sorting and sustainability initiatives.

## 📂 Dataset
Dataset: **Recyclable and Household Waste Classification (Kaggle)**  
Classes used: glass, metal, organic, paper, plastic  
Images per class: ~100 (total ~500)

Data was uploaded to Google Drive and accessed through Google Colab.

## ⚙️ Method
- Transfer Learning using **MobileNetV2** pretrained on ImageNet  
- Input image size: 224×224  
- Train/Validation split: 80/20  
- Batch size: 16 (later reduced to 8 to avoid memory issues)  
- Loss function: categorical_crossentropy  
- Optimizer: Adam  
- Data augmentation applied (rotation, zoom, flip, shift)  

## 🧠 Model Training
A baseline model was trained for **5 epochs**.  
Validation accuracy achieved: **~49%**, which is expected for a small dataset.

Predictions may change slightly between runs because:
- data augmentation introduces randomness  
- dataset is small  
- batches are shuffled  
This behavior is normal in machine learning.

## 📊 Results
- Validation accuracy: ~0.49  
- Loss decreased steadily during training  
- Accuracy and loss graphs were generated  
- Sample predictions (correct and incorrect) were visualized  
- Screenshots of graphs and predictions are included in PPT submission  

## 💾 Saved Model
The trained model is saved at:
MyDrive/waste_project/waste_classifier.h5

## 📘 Notebook
The full implementation is available in the notebook:
Waste_Classification_Project.ipynb

This file is uploaded in the GitHub repository.

## ✔️ Conclusion
This project demonstrates the full workflow of:
1. Dataset selection and preparation  
2. Preprocessing and augmentation  
3. Transfer learning using MobileNetV2  
4. Model building and training  
5. Evaluation  
6. Making predictions and visualizing results  

### 🔮 Future Improvements
- Add more images per class  
- Train for more epochs  
- Fine-tune deeper layers of MobileNetV2  
- Try other architectures like EfficientNet or ResNet  


