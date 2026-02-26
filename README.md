# 🌍 World Happiness: Feature Stability & Ridge Regression from Scratch

This repo implements Ridge Regression (L2 regularisation) using pure NumPy and Matrix Algebra to analyse the dataset.
The goal is to demonstrate how regularization stabilizes a linear model when features (like GDP and Life Expectancy) are highly correlated, preventing "exploding" weights.

## Mathematical Formula
Unlike standard implementations, this project uses the Normal Equation derived from linear algebra:

```math

<div align="center">

\theta = (X^T X + \lambda I)^{-1} X^T Y

</div>
```
Each feature is Z-Score normalized to ensure the penalty is applied fairly across all features.

## Dataset
The [World Happiness Report](https://www.kaggle.com/datasets/unsdsn/world-happiness) is a landmark survey of the state of global happiness that ranks 150+ countries by how happy their citizens perceive themselves to be.

The dataset is primarily based on the Cantril Ladder question: **Respondents are asked to imagine a ladder, with the best possible life for them being a 10 and the worst possible life being a 0**.
