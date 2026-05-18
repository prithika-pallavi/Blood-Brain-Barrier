# BBB+ / BBB- Classification using Random Forest and RDKit

This project implements a basic **Machine Learning classification model** to predict whether a molecule is **Blood-Brain Barrier permeable (BBB+)** or **non-permeable (BBB-)** using **Random Forest** and molecular descriptors generated from **SMILES** strings.

The model combines:

* **Morgan Fingerprints (ECFP-like features)**
* **Physicochemical descriptors**
* **Random Forest Classification**

to perform binary BBB permeability prediction.

---

## Features

* Molecular feature extraction using RDKit
* Morgan Fingerprint generation (1024 bits)
* Physicochemical descriptor calculation
* Random Forest binary classification
* BBB+ / BBB- prediction with confidence score
* Simple and beginner-friendly workflow

---

## Tech Stack

* Python
* Pandas
* NumPy
* RDKit
* Scikit-learn

---

## Molecular Features Used

The model uses:

* Molecular Weight
* LogP
* TPSA (Topological Polar Surface Area)
* Hydrogen Bond Donors
* Hydrogen Bond Acceptors
* Morgan Fingerprints (Radius = 2, Size = 1024)

---

## Workflow

1. Convert SMILES into molecular objects
2. Generate fingerprints and descriptors
3. Create feature vectors
4. Split dataset into training and testing sets
5. Train Random Forest classifier
6. Evaluate model performance
7. Predict BBB permeability for new molecules

---

## Example Prediction

```python
test_smiles = "N[S](=O)(=O)c1cc(ccc1Cl)C2(O)NC(=O)c3ccccc23"

print(predict_bbb(test_smiles))
```

### Sample Output

```text
Molecule : N[S](=O)(=O)c1cc(ccc1Cl)C2(O)NC(=O)c3ccccc23
Prediction: Permeable (BBB+)
Confidence: 87.45%
```

---

## Model Evaluation

The script evaluates:

* Accuracy Score
* ROC-AUC Score

Example:

```text
Accuracy : 0.91
ROC-AUC  : 0.95
```

---

## Installation

Install dependencies:

```bash
pip install pandas numpy scikit-learn rdkit
```

---

## Project Structure

```text
├── bbb_classifier.py
├── README.md
└── dataset.csv (optional)
```

---

## Future Improvements

* Use larger BBB datasets
* Hyperparameter tuning
* Deep learning models (GNNs)
* Feature importance visualization
* Web deployment using Flask/FastAPI

---

## Applications

* Drug discovery
* CNS drug screening
* BBB permeability prediction
* Computational chemistry research

---

---

## ALSO CAN USE EXTRA DATA FROM GIVEN EXCEL SHEET NAMED DATA


---

## Repository Topics

`machine-learning` `random-forest` `rdkit` `drug-discovery` `bbb-prediction` `molecular-descriptors` `cheminformatics` `python`
