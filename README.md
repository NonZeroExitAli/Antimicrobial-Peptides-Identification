# Evaluating Machine Learning Classifiers for Effective Identification of Antimicrobial Peptides
This project applies machine learning to classify antimicrobial peptides (AMPs), integrating diverse datasets, extracting key sequence features, and training models like SVM and Random Forest to optimize accuracy.
## Pipeline description

![image](https://github.com/user-attachments/assets/d5a3d1b7-e3f0-41d3-a55e-a8ad5528de40)

## Installation

```bash
git clone https://github.com/NonZeroExitAli/EVALUATING-MACHINE-LEARNING-CLASSIFIERS-FOR-EFFECTIVE-IDENTIFICATION-OF-ANTIMICROBIAL-PEPTIDES.git
```

## Primary Scripts

1. **AMPs_Data_cleaning&Feature__extraction.ipynb**  
   - Preprocesses and cleans AMP and non-AMP datasets.  
   - Extracts features such as Amino Acid Composition (AAC), Autocorrelation, CTD, and PseudoAAC.  
   - Outputs: feature files for all possible combinations of feature classes.

2. **AMPs_Preprocessing_&_FS_&_Models.ipynb**  
   - Applies various feature selection techniques, including Variance Threshold (VT), Recursive Feature Elimination (RFE), and Random Forest-based selection.
   - Trains machine learning models (SVM, Random Forest, KNN) using selected features.
   - Evaluates models on accuracy, precision, recall, F1-score, and ROC-AUC. 
   - Outputs: Model performance metrics and visualizations.

## Primary Data Structures

The following dataframe is a required input for the computational platform:

1. **AMPs_Data.csv**  
   Merged and cleaned data of AMPs and non-AMPs. Example structure:
   | Peptide_ID | Sequence          | Activity |
   |------------|-------------------|----------|
   | AMP_001    | VGGVPAGPAQ        | AMP      |
   | NONAMP_001 | LLLKKVVGGAA       | nonAMP   |
   | ...        | ...               | ...      |


## External Packages of Note

1. **[ProPy](https://github.com/ShujiaHuang/Propy)**  
   - For feature extraction of protein sequences.

2. **[Imbalanced-learn](https://imbalanced-learn.org/)**  
   - For handling class imbalances using SMOTE.
## Contributors
  - Ali Afifi
  - Omar Loay
  - Ahmed Amr
