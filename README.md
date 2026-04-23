# # DFEN: Dual-Fusion Ensemble Network for Diabetic Retinopathy Classification

📌 Overview
This project proposes a Dual-Fusion Ensemble Network (DFEN) for automated Diabetic Retinopathy (DR) classification using retinal fundus images. The model integrates multiple CNN architectures with feature-level and decision-level fusion strategies.DFEN-DR-Classification

Clone the repository:
git clone https://github.com/yourusername/DFEN-DR-Classification.git
cd DFEN-DR-Classification
Install dependencies:
pip install -r requirements.txt
Prepare dataset:
Place images in the data/ folder
Organize into class-wise subfolders
Run the model:
python main.py
🔗 Fusion Strategy

The proposed DFEN framework integrates three levels of fusion:

1. Feature-Level Fusion

Deep features are extracted from multiple CNN models and concatenated to form a unified feature representation. This combined feature vector is used to train a meta-classifier (MLP).

2. Weighted Averaging Fusion

Softmax outputs from individual models are combined using normalized weights to generate an ensemble prediction, improving reliability and stability.

3. Soft Fusion

A hybrid fusion strategy is applied by combining the outputs of the meta-classifier and weighted averaging using a blending parameter (α), resulting in the final prediction.

---

## 📊 Dataset
- APTOS 2019 Blindness Detection
- DDR Dataset
- Custom retinal dataset

---

## 🧠 Models Used
- EfficientNet-B3  
- MobileNetV2  
- ResNet50  
- SqueezeNet  
- VGG19  
- DenseNet121  

---

## 🔄 Pipeline
1. Dataset loading  
2. Preprocessing (Resize, Crop, CLAHE, Normalization)  
3. Feature extraction using CNN ensemble  
4. Feature-level fusion  
5. Classification using MLP  

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
python train.py
