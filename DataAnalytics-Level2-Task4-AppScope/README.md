# AppScope — Unveiling the Android App Market

## Project Overview
AppScope is a data analytics and natural language processing project that explores the Google Play Store ecosystem. It analyzes app categories, ratings, installs, pricing trends, and user-review sentiment.

**Internship Task:** Level 2 — Task 4  
**Domain:** Data Analytics and Natural Language Processing

## Objectives
- Clean and preprocess real-world app-store datasets.
- Analyze app categories and market saturation.
- Explore app ratings and category-level performance.
- Investigate app size, installs, and their correlation.
- Compare free and paid apps and estimate potential revenue.
- Classify user reviews as positive, negative, or neutral.
- Compare sentiment across app categories.
- Generate static and interactive visualizations.
- Develop data-driven recommendations for app developers.

## Technologies
- Python
- pandas and NumPy
- Matplotlib and Seaborn
- VADER Sentiment Analysis
- Plotly
- JupyterLab

## Datasets
The project uses Google Play Store app information and user reviews.

Dataset source: https://www.kaggle.com/datasets/lava18/google-play-store-apps

## Project Structure
- `AppScope.ipynb` — data cleaning, analysis, sentiment classification, and visualizations.
- `data/` — local source datasets; not committed.
- `outputs/` — generated charts and analysis results.
- `requirements.txt` — Python dependencies.

## Analysis
1. Data cleaning and preprocessing
2. Category distribution and market saturation
3. Ratings distribution and average rating by category
4. App size versus installs
5. Free versus paid app analysis
6. Estimated revenue by category
7. VADER review sentiment analysis
8. Sentiment comparison across categories
9. Interactive Plotly visualization
10. Data-driven conclusions and recommendations

## Important Limitations
- Estimated revenue is a rough calculation based on listed price and recorded installs, not actual earnings.
- Sentiment classification is automated and may misinterpret sarcasm, context, or mixed opinions.
- Correlation does not establish causation.
- Dataset results reflect the available dataset and may not represent the current Play Store.

## Conclusion
AppScope demonstrates how exploratory data analysis and sentiment analysis can reveal app-market patterns and inform decisions about competition, user experience, and monetization.

*Created as part of the OIBSIP Data Analytics internship tasks.*
