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

## Data Preparation

- **Image paths and labels** are stored in a Pandas DataFrame.
- Dataset split: **Train (80%)**, **Validation (10%)**, **Test (10%)**.
- Images resized to **224×224×3** for input to the model.

## Model Architecture

- **CNN layers:** Multiple Conv2D + MaxPooling layers.
- **Global Context Attention:** Added in deeper layers for refined feature extraction.
- **Dense layers & Dropout:** Fully connected dense layers for final classification, with dropout for regularization.
- **Softmax Activation:** Used for multi-class output (5 classes).

## Training

- **Optimizer:** Adam (`lr=0.0005`)
- **Loss Function:** Categorical Crossentropy
- **Epochs:** 20
- **Batch Size:** 64

## 📊 Results

- **Training Accuracy:** 99.6%
- **Validation Accuracy:** 99.0%
- **Test Accuracy:** 99.0%

### 🔹 Confusion Matrix

Shows strong classification performance across all classes.

## Getting Started

1. Clone the repo and install dependencies.
2. Download dataset from Kaggle using:
    ```
    kaggle datasets download -d andrewmvd/lung-and-colon-cancer-histopathological-images
    ```
3. Follow the Jupyter notebook steps for training and evaluation.

## License

Dataset: CC-BY-SA-4.0
