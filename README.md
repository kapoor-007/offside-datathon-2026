# OFFSIDE Datathon 2026

## Team Members
- Harshit Kapoor
- Mahatva Trivedi

## Competition
OFFSIDE Datathon 2026 conducted by IEEE CS MUJ.

## Problem Statement
Predict whether a football player will score at least one goal in a match (`scored_flag`).

## Approach

### Model
CatBoost Classifier

### Validation Metric
Average Precision (AP)

### Validation Strategy
- Train/Test Split: 80/20
- Stratified Sampling
- Random State: 42

## Best Results

| Metric | Score |
|----------|----------|
| Validation AP | 0.4785 |
| Public Leaderboard | 0.48414 |

## Key Features
- home_away
- home_club_goals
- away_club_goals
- goal_diff_abs
- home_club_name
- away_club_name
- home_club_id
- away_club_id
- position
- sub_position
- minutes_ratio
- value_pct_of_peak

## Models Tested

| Model | AP Score |
|---------|---------|
| Baseline CatBoost | 0.2740 |
| H2 | 0.4191 |
| H3 | 0.4310 |
| H4 | 0.4485 |
| H5 | 0.4517 |
| Final CatBoost | 0.4785 |

## Repository Contents
- Jupyter Notebook (.ipynb)
- Final Submission File
- Project Documentation

## Major Finding

Team goal context was the strongest predictor of player scoring probability. Features related to team goals and match context produced the largest gains in Average Precision.
