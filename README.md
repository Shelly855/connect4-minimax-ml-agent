# Minimax ML Agent – Training and Dataset Generation

This repository contains the training code and dataset used to build a Connect 4 ML agent trained on minimax-generated positions.

## Contents

- `generate_minimax_dataset.ipynb` – Generates a dataset of board states and best moves using minimax with alpha-beta pruning
- `minimax_labelled_data.csv` – The generated dataset of board positions and labels
- `train_minimax_model.ipynb` – Trains a `GradientBoostingClassifier` on the dataset
- `ml_agent_minimax.pkl` – Trained model using minimax-labelled data
- `ml_agent.pkl` – Older ML agent trained using the original UCI Connect 4 dataset

---

## Requirements

- Python 3.10 or later  
- Required packages:

```bash
pip install scikit-learn pandas numpy
```

---

## Notes
- The minimax dataset is generated programmatically using the same evaluation logic used during gameplay.
- The trained model (`ml_agent_minimax.pkl`) is used in the main Connect 4 project as an ML agent that mimics minimax decisions.
