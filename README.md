# CFTR QSAR Pipeline

**Machine Learning prediction of CFTR potentiator activity**  
Open-source RDKit + Random Forest / XGBoost pipeline for medicinal chemists working on cystic fibrosis (Verkman lab targets).

### Current Results (32 compounds from all your articles)
- **32 compounds** total
- Valid molecules with SMILES: **8/32**
- **Random Forest** R² = **-0.008** | RMSE = **0.343**
- **XGBoost**    R² = **-0.024** | RMSE = **0.346**
- Dominant scaffold: cyanoquinoline core (6 compounds)

This is a living project. The more compounds we add, the better and more useful the model becomes.

### How to use it (3 simple steps – no coding needed)

1. Click the button below:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/drjoykarmakar/cftr-qsar/blob/main/cftr-qsar.ipynb)

2. In Colab, click **Runtime → Run all** (or Ctrl+F9). Takes ~25–30 seconds.

3. You will see:
   - Full compound table
   - Two prediction plots (Random Forest + XGBoost)
   - Scaffold analysis

### How to test your own new molecule
After the notebook finishes:
- Scroll to the `csv_data` section
- Add your molecule’s SMILES string (and Activity if known)
- Click **Runtime → Run all** again
- Check the new prediction in the plots

**Note**: With 32 compounds the predictions are still exploratory. We are actively expanding the dataset with more literature data.

### Citation
If you use or build upon this work, please cite:
```bibtex
Karmakar, J. (2026). cftr-qsar: RDKit + ML pipeline for CFTR potentiators. 
GitHub repository. https://github.com/drjoykarmakar/cftr-qsar
