# 🎮 Steam Games Market Analysis (2021-2025)

## 📌 Project Overview
This project is a comprehensive data analytics portfolio case study investigating player engagement and market trends across the Steam PC gaming storefront. The primary business task was to determine which revenue models, genres, and developers generate the highest player recommendations, providing actionable insights for independent developers deciding on pricing and release strategies.

## 🗄️ Dataset
* **Source:** Kaggle (Steam Games Dataset 2021-2025)
* **Size:** 65,521 initial records
* **Features Analyzed:** Game Title, Release Year, Genres, Categories, Price, Recommendations, Developer, and Publisher.

## 🛠️ Methodology & Process
This project follows the six-step data analysis framework: Ask, Prepare, Process, Analyze, Share, and Act.

1. **Prepare & Process:** Cleaned the raw dataset using Python and Pandas by dropping records with missing critical metadata (genres, developer, publisher). The dataset was refined to 65,268 viable entries. Multi-tag string columns (like genres and categories) were exploded into lists for accurate aggregation.
2. **Analyze:** Conducted exploratory data analysis (EDA) to evaluate total game counts, average pricing strategies, and volume of positive player reception across various segments.
3. **Machine Learning (Prediction):** Engineered features to train a Random Forest Regressor model utilizing Scikit-Learn to test the predictive power of basic metadata on a game's total recommendations.
4. **Share:** Developed sophisticated data visualizations using Matplotlib and Seaborn to communicate insights effectively to stakeholders.

## 📊 Key Insights & Visualizations

* **Paid vs. Free Engagement:** Paid games generate significantly higher average engagement (422 recommendations) compared to Free-to-Play games (96 recommendations). 
* **Developer Dominance:** Established AAA studios, specifically FromSoftware, Inc. and Game Science, dominate total recommendations. This proves that blockbuster releases still capture the vast majority of player feedback despite the high volume of indie releases in the market.
* **Pricing Strategy does not Dictate Success:** A Random Forest model trained to predict player recommendations based strictly on price and release year yielded an R-squared score of 0.015 and a Mean Absolute Error of 626. This near-zero correlation provides a critical business insight: qualitative factors (gameplay, graphics, marketing, virality) drive player reception, not simply placing a game in an "optimal" pricing tier.

## 📁 Repository Structure
* `steam_analysis.ipynb`: The complete Jupyter Notebook containing all Python code for data cleaning, EDA, visualization, and machine learning.
* `a_steam_data_2021_2025.csv`: The dataset used for this analysis.
