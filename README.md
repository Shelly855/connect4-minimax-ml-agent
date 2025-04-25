# Connect 4 – Minimax-Trained ML Agent

This project folder contains the notebooks and model used to train a Connect 4 ML agent using minimax-generated data. Running it is **not required** to play the final game.

---

## Table of Contents

- [Connect 4 – Minimax-Trained ML Agent](#connect-4--minimax-trained-ml-agent)
- [Files](#files)
- [Notes](#notes)
- [References](#references)
- [Optional Setup (Not Required)](#optional-setup-not-required)
- [GitHub Version (Optional)](#github-version-optional)

---

## Files

- `generate_minimax_dataset.ipynb` – Generates a dataset of board states and best moves using minimax with alpha-beta pruning
- `minimax_labelled_data.csv` – The resulting dataset
- `train_minimax_model.ipynb` – Trains a `GradientBoostingClassifier` on the dataset
- `game.py` – Core Connect 4 logic used during dataset generation and model training
- `ml_agent_minimax.pkl` – Final trained minimax-trained ML model used in the main game
- `ml_agent.pkl` – Trained model based on the UCI dataset (used for the basic ML agent)

---

## Notes

- The minimax-labelled dataset is generated from scratch using the same evaluation heuristics as in-game.
- The trained model (`ml_agent_minimax.pkl`) mimics minimax behaviour and is loaded directly in the game.
- This folder is **not required** to play the game.

---

## References
- Scikit-learn: Machine Learning in Python
  - https://scikit-learn.org/stable/index.html

---

## Optional Setup (Not Required)

If you'd like to rerun the notebooks locally:

1. Ensure Python 3 is installed.
2. Install required packages:

   ```bash
   pip install numpy pandas scikit-learn
   ```
3. Open and run:
   -  `generate_minimax_dataset.ipynb`
   -  `train_minimax_model.ipynb`
> The notebooks was created in Jupyter Notebook. You can also open it in VS Code with the Jupyter extension.

---

## GitHub Version (Optional)

[View this folder on GitHub](https://github.com/Shelly855/connect4-minimax-ml-agent)  
> **Note:** This GitHub link is optional and not required for marking. The repository may be updated after submission.
