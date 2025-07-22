# GC10-DET Steel Defect Classifier

This project applies deep learning to classify steel surface defects using the GC10-DET dataset. It is tailored for industrial applications such as submarine and ship hull fabrication, where early detection of surface defects can improve quality assurance, reduce rework, and enhance safety.

## 📁 Project Structure

- `data/`: Raw and preprocessed images (not included in repo)
- `notebooks/`: Jupyter notebooks for training and analysis
- `scripts/`: Python scripts for preprocessing, training, explainability
- `models/`: Saved TensorFlow models
- `outputs/`: Plots, Grad-CAM images, logs
- `README.md`: Project overview
- `requirements.txt`: Python dependencies

## 🚀 Getting Started

1. Clone this repository
2. Download and extract the GC10-DET dataset into `data/raw/` [a link](https://www.kaggle.com/code/jasonkung98/defects-classification-for-steel-defects-gc10-det)
3. Preprocess the data into `train/` and `val/` folders
4. Run the notebook in `notebooks/GC10_Classifier_Training.ipynb`

## 🧠 Model

Uses a MobileNetV2 CNN with transfer learning to classify 10 surface defect types from 224x224 images. Supports Grad-CAM for explainability and confusion matrix evaluation.

## 🔍 Defect Categories

- Punching (Pu)
- Weld Line (Wl)
- Crescent Gap (Cg)
- Water Spot (Ws)
- Oil Spot (Os)
- Silk Spot (Ss)
- Inclusion (In)
- Rolled Pit (Rp)
- Crease (Cr)
- Waist Folding (Wf)

These defects can be grouped into structural, contamination, deformation, or process-related categories.

## 📈 Results

The model achieves high classification accuracy with clear Grad-CAM visualizations to support explainability.

## 📌 Future Work

- Add segmentation for pixel-level localization
- Integrate with AR or CAD visualization systems
- Deploy via lightweight web interface (e.g., Streamlit)
