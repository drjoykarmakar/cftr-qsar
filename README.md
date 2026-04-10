# CFTR QSAR Pipeline

**Machine Learning for CFTR Potentiator Activity Prediction**  
Open-source RDKit + Random Forest / XGBoost pipeline built for medicinal chemists working on cystic fibrosis.

### Current Results (21 compounds)
- **21 compounds** total (7 with valid SMILES)
- **Random Forest** R² = **-0.109** | RMSE = **0.355**
- **XGBoost**    R² = **-0.068** | RMSE = **0.348**
- Dominant scaffold: cyanoquinoline core (5 compounds)

This is a living project — the more compounds we add, the stronger the model becomes.

### How to use it (3 simple steps – no coding required)

1. Click the button below:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/drjoykarmakar/cftr-qsar/blob/main/cftr-qsar.ipynb)

2. In Colab → **Runtime → Run all** (Ctrl + F9). Takes ~25 seconds.

3. You will see:
   - Full compound table
   - Two prediction plots
   - Scaffold analysis

### How to test your own new molecule
After the notebook finishes running:
- Scroll to the `csv_data` section
- Add your molecule’s SMILES (and Activity if known)
- Click **Runtime → Run all** again
- Check the new prediction in the plots

**Note**: With 21 compounds the model is still learning. We are actively expanding the dataset with more literature data.

### Citation
```bibtex
Karmakar, J. (2026). cftr-qsar: RDKit + ML pipeline for CFTR potentiators. 
GitHub repository. https://github.com/drjoykarmakar/cftr-qsar
--
Dr. Joy Karmakar
10th April 2026
