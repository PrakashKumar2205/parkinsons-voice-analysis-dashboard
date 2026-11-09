# Parkinson's Disease Detection Using Voice Signal Analysis

Machine-learning analysis of acoustic voice biomarkers: an interactive research dashboard.

> **Research prototype only.** Results are for educational and research purposes
> and must not be interpreted as a medical diagnosis.

## Overview
This project investigates whether acoustic voice features (jitter, shimmer, pitch,
HNR, NHR, RPDE, DFA, PPE, spread1, spread2, D2) can help machine-learning models
distinguish Parkinson's-related voice patterns from healthy-control patterns.

## Features
- Voice analysis studio: upload or record a sustained vowel, with waveform,
  spectrogram, pitch contour and frequency spectrum
- In-browser acoustic feature estimates (approximate, frame-level)
- Feature analysis: group comparisons, scatter, histogram, radar, effect sizes
- Model benchmarking: leaderboard, per-model metrics, radar comparison
- Model evaluation: confusion matrix, ROC and precision-recall curves, feature importance
- Dataset intelligence: CSV upload, target selection, data-quality score, correlations
- Command palette (Ctrl/Cmd + K), light/dark themes, responsive layout

## Data transparency
The built-in dataset is **synthetic demo data**, and the model metrics are
**simulated placeholders**. Both are labeled in the interface. Uploading a CSV
replaces the dataset statistics, but model results stay simulated until a trained
backend is connected.

## Tech stack
HTML, CSS, JavaScript, Chart.js, Web Audio API.
Planned backend: Python, FastAPI, scikit-learn, librosa, pandas, NumPy.

## Run locally
Open `index.html` in a modern browser (Chrome, Edge, Firefox or Safari).

## Limitations
Small and homogeneous datasets, recording and microphone variability, repeated
recordings per participant, class imbalance, and the need for external validation.
Voice analysis alone cannot establish a clinical diagnosis.

## Future work
Trained FastAPI backend with participant-grouped cross-validation, larger and more
diverse datasets, explainable AI (SHAP), longitudinal monitoring.

## Author
Prakash Kumar
