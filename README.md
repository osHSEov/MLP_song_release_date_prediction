# MLP_song_release_date_prediction

🎶 Predicting Song Release Year with MLP

📌 Overview

This project trains a multi-layer perceptron (MLP) neural network to predict the release year of a song based on its audio features. The task is formulated as a regression problem.
The work follows ideas from this [reference](https://samyzaf.com/ML/song_year/song_year.html),where simple models achieve strong results.

📂 Dataset

Source: Million Song Dataset – YearPredictionMSD

Shape: 515,345 rows × 91 columns

Features: 90 audio features per song (first-order and second-order spectral descriptors)

Target: Release year of the song (integer between 1922 and 2011)

🛠️ Methods & Tools

Languages/Libraries: Python, Pandas, NumPy, Matplotlib, scikit-learn, PyTorch

Baseline: Ridge Regression (MSE ≈ ~90)

Model: Multi-Layer Perceptron (MLP) built with PyTorch

Optimization: Adam optimizer, learning rate tuning

🤖 Modeling Approach

Baseline: Ridge Regression → MSE around 90. Plus XGboost with result of 80.

MLP:

Fully connected feed-forward network

ReLU activations

Batch size = 100

Adam optimizer with tuned learning rate

Experiments: Adjusting hidden layers, neurons, learning rate.

📊 Results

Baseline (Ridge Regression): MSE ≈ 90, XGboost 80.

MLP: Achieved result comparably better than Rigid - 78.2 and slightly better than XGBoost

Further hyperparameter tuning showed potential for improvements
