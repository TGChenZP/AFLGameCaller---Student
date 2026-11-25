# AFL Win Probability — ML Workshop

A hands-on workshop where you build an in-game win probability model for AFL from scratch, stepping through four progressively more sophisticated approaches:

- **Model A** — a non-parametric lookup table (conditional means by quarter, score bracket, and minute)
- **Model B** — logistic regression on score margin alone
- **Model C** — logistic regression with elapsed time and an interaction term
- **Model D** — LightGBM (gradient boosting)

By the end you will have trained, evaluated, and compared all four models on 14 years of AFL data (2012–2025), and run a final held-out evaluation on 2024–2025.

## Getting started

1. Install dependencies: `pip install pandas numpy statsmodels lightgbm scikit-learn`
2. Place the data file (see below)
3. Open `workshop/afl_win_probability_student.ipynb` in Jupyter and work top to bottom
4. Each section has a `TODO` block — fill it in, then check your output against the reference answer hidden in the `<details>` dropdown below it

## Data

The dataset is **not included in this repository** and must be provided separately.

Place the file here:

```
data/
└── model_dataset.csv
```

The file is `model_dataset.csv` (~120 MB). Once it is in the `data/` folder, the notebook's data loading cell will work without any changes.
