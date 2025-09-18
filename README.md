# 🧬 Lung and Colon Cancer Histopathological Image Classification  

This project implements a **Convolutional Neural Network (CNN)** with a **Global Context Attention mechanism** to classify **lung and colon cancer histopathological images** into five categories. The dataset is taken from Kaggle and the model achieves **99% accuracy** on the test set.  

---

## 📂 Dataset  

- **Source**: [Lung and Colon Cancer Histopathological Images - Kaggle](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images)  
- **License**: CC-BY-SA-4.0  
- **Size**: ~1.76 GB  
- **Classes**:  
  - Colon Adenocarcinoma  
  - Colon Benign Tissue  
  - Lung Adenocarcinoma  
  - Lung Benign Tissue  
  - Lung Squamous Cell Carcinoma  

The dataset contains **25,000 histopathological images**.  

---

## 🛠️ Tech Stack  

- **Languages**: Python  
- **Frameworks & Libraries**:  
  - TensorFlow / Keras  
  - OpenCV  
  - NumPy, Pandas  
  - Matplotlib, Seaborn  
  - scikit-learn  

---

## ⚙️ Project Workflow  

1. **Download & Extract Dataset**  
   ```bash
   !kaggle datasets download -d andrewmvd/lung-and-colon-cancer-histopathological-images
   unzip lung-and-colon-cancer-histopathological-images.zip
