# EGFR Drug Discovery Pipeline

ML-powered computational drug discovery targeting EGFR 
(Epidermal Growth Factor Receptor) — a key cancer protein.

# Workflow
1. Fetch EGFR bioactivity data from ChEMBL (454 molecules)
2. Build Morgan fingerprint features using RDKit
3. Train Random Forest classifier → **92.31% accuracy**
4. Predict active/inactive molecules
5. Dock best candidate (Gefitinib) into EGFR via AutoDock Vina
6. Visualize 3D docked pose with Py3Dmol

# ML Results
| Molecule | Prediction | Result |
|---|---|---|
| Erlotinib | ACTIVE | ✅ Correct |
| Gefitinib | ACTIVE | ✅ Correct |
| Caffeine | INACTIVE | ✅ Correct |

# Tools & Libraries
- RDKit, ChEMBL API, BioPython
- Scikit-learn (Random Forest)
- AutoDock Vina, OpenBabel
- Py3Dmol

# Run in Google Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1B0L5qGl19etS1tUy12-yzIPc-xA6bCWF)

# Target
EGFR (CHEMBL203) — overexpressed in lung, breast & colorectal cancers

