# BERTopic Analysis of MBA Program Reviews

This repository contains the full code, data, and report for an NLP project that applies topic modeling techniques to student reviews of top U.S. MBA programs. By using the BERTopic algorithm, this project aims to help prospective MBA applicants gain deeper insights into each school's academic, professional, and community characteristics based on real experiences shared by students and alumni.

## Objective

To bridge the information gap between objective indicators (e.g., rankings, job placement) and subjective student experience by analyzing qualitative review data using Natural Language Processing (NLP) and topic modeling.

## Data

- **Source**: Publicly available student reviews from [GMAT Club](https://gmatclub.com) and [Niche](https://www.niche.com).
- **Scope**: 200 student reviews across the top 10 U.S. business schools based on the 2025 *U.S. News Best Business Schools* rankings.

Data is available in the [`/data`](./data) directory.

## Methods

- **Data Cleaning**:
  - Lowercasing, punctuation removal
  - Standard + custom stopword filtering
  - Synonym normalization using custom mapping

- **Topic Modeling**:
  - BERTopic (with n-gram range and `min_topic_size`)
  - Post-processing: topic merging and renaming for semantic clarity

- **Visualization**:
  - Keyword barcharts per topic
  - School-by-topic heatmap

All code is available in the [`/code`](./code) directory.

## Key Results

- Identified 10 main topics from MBA reviews, later merged into 8 semantically meaningful themes:  
  `finance`, `community`, `consulting`, `class quality`, `location`, `professor`, `entrepreneurship`, `course difficulty`.

- Created a heatmap showing the relative prevalence of each topic across schools.

- Revealed distinct institutional strengths:  
  e.g., NYU and Columbia for finance, Harvard and UChicago for academic rigor, Dartmouth for location and community, Stanford for entrepreneurship.

## Final Report

The full academic report, including abstract, methodology, results, interpretation, and future directions, is available in the [`/report`](./report) directory.


## Dependencies

- Python 3.9+
- `pandas`
- `nltk`
- `bertopic`
- `scikit-learn`
- `matplotlib`
- `seaborn`


