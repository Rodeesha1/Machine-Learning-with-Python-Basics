# ClimateWins: Predicting Pleasant Weather with Machine Learning 🌦️

This repository contains the work completed for ClimateWins to investigate whether machine learning models can predict and project weather in Europe, based on historical weather station data. The project was completed in two stages, culminating in a final proposal to ClimateWins.

## Repository Structure
data/                # Raw and cleaned weather + answers datasets
scripts/             # Python scripts for each ML model
results/             # Confusion matrices, accuracy results, written reports
notebooks/           # Jupyter notebooks for experiments
presentation/        # Final presentation slides (PPTX/PDF) + visuals
docs/                # Project briefs and reference materials


## Project Objectives
The objective was to determine if supervised learning models could accurately predict: 
1. Predict whether a given day is "pleasant" or "unpleasant" using historical weather data.  
2. Identify weather patterns outside regional norms in Europe.  
3. Determine if unusual patterns are increasing.  
4. Generate possible climate scenarios for the next 25–50 years.  
5. Locate the safest regions for people to live in Europe under future conditions.

## 🔹 Achievement 1 (Supervised Learning)
**Goal:** Predict "pleasant" vs. "unpleasant" daily weather.  

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


## 🔹 Achievement 2 (Advanced Machine Learning & Proposal)
**Goal:** Move beyond supervised learning into advanced ML methods, test unsupervised learning, deep learning, and GANs, then propose a final ClimateWins strategy.  

**Methods Explored**
- **Unsupervised Learning:** Clustering (k-means, hierarchical), PCA, anomaly detection.  
- **Deep Learning:** CNNs and RNNs for image recognition and time-series prediction.  
- **Classical ML:** Random Forests and SVMs for classification tasks.  
- **Generative Models:** GANs for simulating future weather scenarios.  
- **Hyperparameter Tuning:** Tested impact of tuning on CNN/RNN and ANN models.  

---

## 🔹 Final Proposal: Three Thought Experiments
The final recommendation to ClimateWins consisted of three thought experiments aligned with its goals:

1. **Climate Pattern Shift Detection**  
   - **Method:** Clustering + PCA + anomaly detection.  
   - **Goal Link:** Identify unusual weather patterns and track whether they are increasing.  

2. **Future Climate Projection GAN**  
   - **Method:** GANs for scenario simulation, RNNs for time-series forecasting.  
   - **Goal Link:** Generate plausible climate conditions 25–50 years into the future.  

3. **Safe Zones for Climate Refugees**  
   - **Method:** Ensemble models (Random Forest + CNN on geospatial data).  
   - **Goal Link:** Identify the safest places to live in Europe, considering weather + infrastructure + hazard maps.  

**Recommendation:**  
While all three approaches add value, **Safe Zones** offers the most immediate impact and aligns directly with ClimateWins’ humanitarian mission.  

---

## 📊 Results & Deliverables
- **Figures:** PCA variance, clustering plots, Europe livability heatmaps, GAN schematic.  
- **Notebooks:** Contain training code for clustering, GANs, and ensemble safe-zone models.  
- **Presentation:**
- [Final ClimateWins ACH1 (PDF)]((https://coach-courses-us.s3.amazonaws.com/exercises/1407/68985/c7118d26f34b30e9cc4b0dd4f9353407/ClimateWins-Presentation.pdf))
- [Final ClimateWins ACH2 (PDF)]([https://coach-courses-us.s3.amazonaws.com/exercises/1413/68985/168e4601986496e52e35f7bdbf3f9cac/ClimateWins-Final-Presentation.pdf))
- **Videos:**  
  - [Achievement 1 Presentation](https://www.youtube.com/watch?v=VeoaBEmftjc)  
  - [Achievement 2 presentation] editing...)  



## ⚙️ Requirements
Install dependencies with:  
```bash
pip install -r requirements.txt
```

*Core libraries:*  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  
- tensorflow / keras  
- geopandas  
- folium  
