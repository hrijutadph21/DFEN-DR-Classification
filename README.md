# DFEN-DR-Classification
Dual-Fusion Ensemble Network for DR Classification
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
