# 🧪 Solubility Predictor (Based on SMILES Input)

This project predicts the aqueous solubility (logS) of a compound from its SMILES representation using molecular descriptors generated via **RDKit** and a machine learning model trained on real-world data.

---

## 🚀 Features

- 🔬 Predict solubility of molecules using only their **SMILES**.
- 🧠 Uses **RDKit Descriptors** for feature extraction.
- 📊 Machine Learning model trained on labeled solubility datasets.
- 🧾 Input validation for incorrect SMILES.
- 📈 Option to train your own model or use pre-trained model.

---

## 🧰 Tech Stack

- **Python**
- **RDKit** for chemical descriptor generation
- **Pandas & NumPy** for data processing
- **scikit-learn** for machine learning (Linear Regression, Random Forest, etc.)
- **Matplotlib/Seaborn** (optional) for visualization

---

## 📂 Project Structure

solubility-predictor/

│
├── data/

│ └── solubility_dataset.csv # Dataset with SMILES and logS

│
├── models/

│ └── trained_model.pkl # Pre-trained ML model

│
├── scripts/

│ ├── feature_generator.py # Generates RDKit descriptors

│ ├── train_model.py # Trains and saves model

│ └── predict.py # Loads model and predicts solubility

│
├── app.ipynb # Jupyter notebook for end-to-end demo

└── README.md

## How It Works
1. User inputs a SMILES string or compund name.

2. RDKit extracts molecular descriptors (e.g., MolWt, TPSA, NumHDonors).

3. The model (e.g., Random Forest) uses these features to predict logS.

Output: Predicted solubility in mols/L (log scale).

## 🔗 Dataset Source
  You can use any open solubility dataset such as:

   Delaney Solubility Dataset (ESOL)

## 👥 Author
Kumar Mohit
🔗 LinkedIn
📧 kumarmohitsspn969@gmail.com

## 📌 To Do
 Web interface using Streamlit or Flask

 Increase the accuracy of the model using other various ML methods, the project is at very initial stage

 Model export to ONNX

 Compare with neural net-based predictor
