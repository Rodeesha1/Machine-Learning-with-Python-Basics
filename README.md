# ClimateWins: Predicting Pleasant Weather with Machine Learning 🌦️

This repository contains the work completed for ClimateWins to investigate whether supervised learning models can predict "pleasant" daily weather in Europe, based on historical weather station data.

## Repository Structure
data/ # Raw and cleaned weather + answers datasets

scripts/ # Python scripts for each ML model

results/ # Confusion matrices, accuracy results, written report

presentation/ # Final presentation slides (PPTX/PDF)

## Project Objective
The objective was to determine if supervised learning models (KNN, Decision Trees, and ANNs) could accurately predict "pleasant" days (labeled as 1) and "unpleasant" days (labeled as 0) using weather station data.

## Models Used
- **KNN (k-nearest neighbors):** Baseline model, tested with scaled and unscaled data.  
- **Decision Tree:** Both unpruned and pruned versions to test overfitting.  
- **ANN (Artificial Neural Network):** Multiple architectures, tested with scaling and hyperparameter tuning.  

##  Biases & Limitations
- **Biases:** Subjective definition of "pleasant weather"; missing data (GDANSK, ROMA, TOURS excluded).  
- **Accuracy:** Overall test accuracies remain low (25–35%). Models captured some patterns but not enough for strong predictions.  
- **Post-processing:** Feature scaling required for ANN; pruning applied for Decision Tree.  

## Next Steps
- Explore additional algorithms.  
- Engineer new features.  
- Expand dataset coverage for more stations and longer time spans.
- Compare supervised vs. unsupervised learning approaches for clustering weather patterns.

## Presentation
file:///C:/Users/user/OneDrive/Documents/Data%20Analysis%20Course/Machine%20Learning/Climate%20Wins/4.%20Sent%20to%20Shareholders/ClimateWins%20Presentation.pdf

##  Requirements
Install dependencies with:
```bash
pandas
numpy
scikit-learn
matplotlib
seaborn
