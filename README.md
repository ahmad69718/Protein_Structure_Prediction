
# **Protein_Structure_Prediction**

## **Overview**

This project aims to predict the structure of proteins using machine learning techniques. Given a dataset of protein sequences and their associated structures, the goal is to classify residues and predict their positions in 3D space based on their features. The models used in this project include **Support Vector Machine (SVM)**, **Random Forest (RF)**, and **Artificial Neural Networks (ANN)**.

## **Project Structure**

```
Protein_Structure_Prediction/
│
├── data/
│   └── pdb4hhb.ent  # Protein Data Bank (PDB) file used for the analysis
│
├── src/
│   ├── extract_atom_info.py  # Extracts atom information from PDB file
│   ├── preprocess_data.py  # Preprocesses data (one-hot encoding, scaling, etc.)
│   ├── models.py  # Defines and trains SVM, RF, and ANN models
│   └── evaluate_models.py  # Evaluates models and prints accuracy
│
├── README.md  # This file
└── main.py  # Executes the workflow, from data loading to model evaluation
```

## **Requirements**

- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `matplotlib` (optional for visualization)

You can install the required libraries using pip:

```
pip install numpy pandas scikit-learn matplotlib
```

## **Data**

The data used in this project consists of a **Protein Data Bank (PDB)** file (`pdb4hhb.ent`). This file contains the atomic coordinates and other details of the protein. The project preprocesses the PDB data to extract key features such as residue names and atomic coordinates, which are used to train machine learning models.

## **Example Output**

After training and evaluating the models on the test set, the following accuracies were achieved:

```
SVM Accuracy: 0.5680
Random Forest Accuracy: 0.9383
ANN Accuracy: 0.9215
```

## **MIT License**

```
MIT License

Copyright (c) 2024 Ahmad Raza

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
