# CFTR QSAR Pipeline

**Machine Learning prediction of CFTR potentiator activity**  
Open-source RDKit + Random Forest / XGBoost pipeline for medicinal chemists working on cystic fibrosis (Verkman lab targets).

### Results (current dataset)
- **8 compounds** (5 with valid SMILES)
- **Random Forest** R² = **-0.477** | RMSE = 0.401
- **XGBoost**    R² = **-0.113** | RMSE = 0.348
- Dominant scaffolds: cyanoquinoline derivatives + quinazolinone core

This is a **starting point**. The more compounds we add, the better the model becomes.

### How to use it (3 simple steps – no coding needed)

1. Click the button below:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/drjoykarmakar/cftr-qsar/blob/main/cftr-qsar.ipynb)

2. In Colab, click **Runtime → Run all** (or Ctrl+F9).  
   It takes ~20–30 seconds.

3. You will see:
   - All compounds used
   - Two prediction plots (Random Forest + XGBoost)
   - Scaffold analysis

### How to test your own new molecule
After the notebook finishes:
- Scroll to the `csv_data` section
- Add your molecule’s SMILES string (and Activity if known)
- Click **Runtime → Run all** again
- Check the new prediction in the plots

**Note**: With only 8 compounds the predictions are still rough. We are actively expanding the dataset.

### Citation
If you use or build upon this work, please cite:
```bibtex
Karmakar, J. (2026). cftr-qsar: RDKit + ML pipeline for CFTR potentiators. 
GitHub repository. https://github.com/drjoykarmakar/cftr-qsar

---  
Dr. Joy Karmakar  
April 2026
