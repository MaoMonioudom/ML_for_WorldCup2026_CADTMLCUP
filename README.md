# Machine Learning for FIFA World Cup 2026 Prediction

## Overview
This project builds machine learning models to predict FIFA World Cup 2026 match 
outcomes and scores, built for a prediction competition hosted by Makerspace at 
Cambodia Academy of Digital Technology (CADT).

Two models are built:
- **Outcome model** — predicts Win / Draw / Loss for each match
- **Score model** — predicts the exact scoreline (e.g. 2-1)

## Data Sources
- International football match results (1872–2025):
  [martj42/international_results](https://github.com/martj42/international_results) by Mart Jürisoo
- FIFA World Rankings:
  [FIFA World Ranking](https://www.kaggle.com/datasets/cashncarry/fifaworldranking) by cashncarry on Kaggle

## How to Use

### Quick Start (models already trained)
Open `Notebooks/V2/Predictions_R32.ipynb` and run all cells top to bottom, then call:

```python
predict('Brazil', 'France', is_neutral=1, tournament='FIFA World Cup')

```
├── data/               ← raw data (do not modify)
├── dataII/
│   ├── V1/             ← v1 models and features
│   ├── V2/             ← v2 models and features (current)
│   └── rankings.csv    ← FIFA rankings input
└── Notebooks/
    ├── V1/             ← old notebooks (reference only)
    └── V2/             ← active notebooks
        ├── Notebook03.ipynb       ← training
        └── Predictions_R32.ipynb ← predictions
```