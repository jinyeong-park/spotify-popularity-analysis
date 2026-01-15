# Music Trend analysis

## Executive Summary

This project leverages machine learning to predict Spotify track popularity and identify the key drivers of listener engagement. Analyzing 114,000 songs, we developed predictive models that achieve an R² of 0.42, explaining 42% of the variance in track popularity. Our findings reveal that genre, instrumentalness, and explicitness are the strongest predictors of success, providing actionable insights for artists, producers, and record labels to optimize their music production and marketing strategies.

---

## Business Problem

The music industry faces challenges in predicting which songs will resonate with audiences before release. Artists and producers invest significant time and resources into creating music without clear data-driven guidance on what features contribute to popularity. This project addresses three critical questions:

1. **Can we predict a song's popularity** based on its audio features and characteristics?
2. **What specific features** (genre, energy, acousticness, etc.) have the greatest impact on listener engagement?
3. **How can artists and producers** leverage these insights to make informed creative and strategic decisions?

Our goal is to provide a data-driven framework that helps music creators maximize their tracks' potential reach and audience appeal.

---

## Methodology

### Data Collection & Preparation
- **Dataset**: 114,000 Spotify tracks sourced from Kaggle
- **Target Variable**: Popularity score (0-100 rating)
- **Features**: Genre, danceability, energy, acousticness, valence, instrumentalness, explicitness, and additional audio characteristics

### Model Development
We implemented a progressive modeling approach, evaluating performance using R² and RMSE metrics:

1. **Baseline Model**: Mean-based prediction for performance benchmark
2. **Linear Regression**: Simple linear modeling approach
3. **Tree-Based Models**: Decision Tree and Random Forest for non-linear relationships
4. **Advanced ML**: XGBoost and Neural Networks for complex pattern recognition

### Model Evaluation
- Primary metrics: R² (explanatory power) and RMSE (prediction accuracy)
- Cross-validation to ensure model generalizability
- Feature importance analysis to identify key drivers

---

## Skills

### Technical Skills
- **Machine Learning**: Scikit-learn, XGBoost, TensorFlow/Keras
- **Data Analysis**: Pandas, NumPy
- **Data Visualization**: Matplotlib, Seaborn
- **Programming**: Python, Jupyter Notebooks

### Analytical Skills
- Predictive modeling and algorithm selection
- Feature engineering and importance analysis
- Model evaluation and comparison
- Statistical analysis and interpretation

### Business Skills
- Translating technical findings into actionable business recommendations
- Data storytelling and presentation
- Strategic decision-making support

---

## Results & Business Recommendations

### Model Performance
**Best Model: XGBoost**
- **R² Score**: 0.42 (explains 42% of popularity variance)
- **RMSE**: 15.05 (average prediction error of 15 points on 0-100 scale)
- Random Forest performed comparably, while Neural Networks showed lower explanatory power

### Top Feature Importance Rankings
1. **Genre** - Strongest predictor of popularity
2. **Instrumentalness** - Second most important factor
3. **Explicitness** - Third strongest contributor
4. **Acousticness** - Fourth most influential
5. **Energy** - Fifth key driver

### Genre-Specific Insights
**High-Performing Genres** (Avg. Popularity: 55-59)
- Pop-film, K-pop, Pop, Electro, House, Chill, EDM

**Low-Performing Genres** (Avg. Popularity: <20)
- Chicago-house, Detroit-techno, Romance

### Business Recommendations

#### 1. Strategic Genre Selection & Curation
- **For Artists**: Focus on high-performing genres (Pop, K-pop, EDM, House) to maximize reach
- **For Playlist Curators**: Segment playlists by top-performing genres to increase engagement
- **For Labels**: Use genre as a primary filter for A&R decisions and marketing investments

#### 2. Optimize Instrumental Quality
- Invest in high-quality instrumental production, particularly for lo-fi, chill, and cinematic genres
- Instrumentalness ranks as the second strongest predictor—don't underestimate its impact
- Consider instrumental versions or remixes to expand track appeal

#### 3. Embrace Authentic Expression
- Explicitness is the third strongest factor in popularity
- Artists should not shy away from authentic lyrical expression and explicit content
