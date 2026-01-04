# Spotify Tracks EDA & Hypothesis Testing

This project explores a public Spotify tracks dataset to demonstrate an end-to-end analytics workflow:
data cleaning, feature engineering, exploratory data analysis (EDA), and hypothesis testing.

## Dataset
- Source: Spotify Tracks Dataset on Kaggle (maharshipandya)
- Observations include track metadata and audio features (e.g., danceability, energy, valence, tempo).

## Goals
- Assess dataset quality (missingness, duplicates, ranges, outliers)
- Engineer helpful features (e.g., duration in minutes, bins for popularity)
- Explore relationships between audio features and popularity
- Formulate hypotheses and run at least one statistical significance test

## Key Questions
- Do explicit tracks differ in popularity from non-explicit tracks?
- How does popularity vary across genres?
- Which audio features (e.g., energy, danceability, valence) relate most to popularity?

## Methods
- Cleaning: removed irrelevant index-like columns, handled duplicates, validated feature ranges
- Feature Engineering: `duration_min`, popularity bins, readable labels for mode (Major/Minor)
- EDA: distributions, group comparisons, correlation analysis, genre-focused plots
- Hypothesis Testing: Welch’s t-test (for two-group comparison with unequal variances) + effect size (Cohen’s d)

## Files
- `Coursera_Project_Dalileh_IBM_Spotify_UPDATED.ipynb` — main notebook with analysis and results

## How to Run
1. Clone this repo
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
