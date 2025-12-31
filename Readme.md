# Lost Ark Avatar Dye Recommendation System

## 1. Project Overview
This project aims to build a data-driven recommendation system that suggests avatar dye color combinations 
that visually match a Lost Ark character's appearance.

The motivation comes from a common problem among players: 
even if an avatar dye looks good in isolation, it often does not harmonize well with the character's overall appearance 
(skin tone, hair color, and class concept).

By leveraging community-validated dye examples and image-based features, 
this project explores whether visual preferences can be learned and recommended using data science techniques.

---

## 2. Problem Statement
Avatar dyeing in Lost Ark is a time- and cost-intensive process, yet players often experience trial and error due to:
- Visual differences between preview and in-game appearance
- Difficulty judging color harmony with character features
- Subjective aesthetic decision-making

**Core Question**  
> Can we recommend avatar dye combinations that visually match a character 
> using image features and community preference data?

---

## 3. Target Users
- Players who frequently customize avatar dyes
- Users who rely on community posts for dye inspiration
- Players who want to minimize dye trial-and-error costs

---

## 4. Data Strategy

### Data Sources
- Community posts containing avatar dye screenshots
- Extracted color information (RGB / HEX) from images
- Community engagement metrics (likes, comments) as preference signals
- Character metadata (class, gender) when available

### Label Definition
Community engagement metrics are used as a **proxy for aesthetic preference**, 
rather than an absolute ground truth.

---

## 5. Methodology

### Step 1: Exploratory Data Analysis (EDA)
- Analyze color distributions by skin tone and class
- Examine relationships between color harmony metrics and engagement

### Step 2: Baseline Recommendation
- Extract dominant color features from images
- Compute image similarity using cosine similarity
- Recommend top-N dye combinations

### Step 3: Model Enhancement
- CNN-based feature extraction using pretrained models
- Incorporate color harmony features
- Ranking-based recommendation approach

---

## 6. Evaluation

### Quantitative Evaluation
- Inclusion rate of highly engaged dye combinations
- Average engagement score of recommended results

### Qualitative Evaluation
- Human evaluation through small-scale surveys

---

## 7. Tech Stack
- Python
- Pandas, NumPy
- OpenCV / PIL
- Scikit-learn
- TensorFlow / Keras
- Streamlit (for MVP)

---

## 8. Project Status
🚧 **Currently in planning and data collection phase**

Upcoming steps:
- Finalize data sources
- Implement data pipeline
- Conduct EDA and baseline modeling
