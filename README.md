# ICE_ixa Sentiment Analysis

## Overview

This project presents a comprehensive **sentiment and thematic analysis of workspace environments and their impact on productivity, focus, cognitive fatigue, and output quality**. The study is built as part of a broader strategic exploration for **ixa – a nature-integrated creative workspace model**.

The analysis combines **Natural Language Processing (NLP), sentiment scoring, and qualitative thematic structuring** to uncover patterns in how different work environments influence human cognitive performance.

---

## Objective

The primary objective of this project is to:

* Analyze how **environmental factors influence productivity and cognitive performance**
* Identify key **pain points in modern work environments**
* Evaluate **willingness to shift toward alternative (remote/nature-based) workspaces**
* Translate raw sentiment data into **structured, strategic insights**

---

## Dataset Description

### 1. Raw Sentiment Dataset

* File: `ixa_Market_Research_Sentiment_...`
* Contains:

  * `category` (dimension)
  * `sentiment` (text input)
  * `polarity` (assigned score)

### 2. Fine-Grained Analysis Dataset

* File: `ixa_fine_grained_analysis.csv`
* Structured into:

  * **Variable**
  * **Subtopic**
  * **Verbatim Signal / Theme**
  * **Sentiment**
  * **Polarity**

This dataset is curated to reflect **real-world cognitive and behavioral signals** derived from qualitative sources.

---

## Key Dimensions Analyzed

1. **Impact of Environmental Setup on Productivity**
2. **Maintaining Consistent Productivity and Focus**
3. **Emotional Friction and Cognitive Fatigue**
4. **Levels and Quality of Output**
5. **Willingness to Shift to Remote Workspaces**

---

## Methodology

### 1. Data Preprocessing

* Text normalization (lowercasing, punctuation removal)
* Stopword removal
* Tokenization and lemmatization

### 2. Feature Engineering

* TF-IDF vectorization (including bigrams)
* Keyword extraction per category

### 3. Sentiment Analysis

* Rule-based model: **VADER**
* ML model: **Logistic Regression / SVM on TF-IDF features**

### 4. Weighted Sentiment Scoring

To improve accuracy beyond simple averaging:

* Sentiments are weighted based on **intensity and intent**
* Strong signals carry higher weight than passive expressions

### 5. Thematic Clustering

* Raw sentiments are grouped into:

  * Subtopics
  * Verbatim themes
* Enables conversion from **raw text → structured insights**

---

## Key Findings

### 1. Environmental Impact

* Clean, minimal, and nature-integrated environments significantly improve:

  * Focus
  * Clarity
  * Task initiation

### 2. Productivity & Focus

* Open and noisy environments severely disrupt deep work
* Interruptions and digital distractions are major productivity inhibitors

### 3. Cognitive Fatigue

* High levels of **mental exhaustion and burnout signals**
* Context switching and fragmented workflows are key contributors

### 4. Output Quality

* Work is often:

  * Reactive
  * Shallow
  * Below intended quality
* Deep work environments significantly improve output depth

### 5. Willingness to Shift

* Strong positive inclination toward:

  * Nature-based workspaces
  * Temporary relocation for focused work
* Indicates **emerging behavioral shift**

---

## Insights for ixa (Strategic Relevance)

The findings strongly support the ixa concept:

* **Problem:** Urban work environments create cognitive overload and fragmented attention
* **Need:** Deep work, clarity, and uninterrupted focus
* **Opportunity:** Controlled, biophilic environments can unlock higher cognitive performance

This positions ixa as:

> A solution that converts **latent demand for focus and clarity into actionable work environments**

---

## Visualizations

The project includes:

* Sentiment distribution charts
* TF-IDF keyword analysis
* Word clouds per category
* Confusion matrix (model evaluation)
* Dimension-level sentiment summary tables

---

## Tools & Technologies

* Python (Google Colab)
* Pandas, NumPy
* Scikit-learn (TF-IDF, ML models)
* NLTK / spaCy (NLP preprocessing)
* Matplotlib (visualization)

---

## How to Use

1. Upload dataset to Google Colab
2. Run preprocessing and analysis pipeline
3. Generate:

   * Sentiment outputs
   * Visualizations
   * Final summary tables

---

## Project Structure

```
ICE_ixa_sentimentanalysis/
│
├── README.md
├── ixa_Market_Research_Sentiment_...
├── ixa_fine_grained_analysis.csv
└── analysis_notebook.ipynb (recommended)
```

---

## Limitations

* Dataset is partially **synthetic but grounded in real qualitative signals**
* Sentiment scoring may not capture full nuance of human cognition
* Results should be interpreted as **directional insights**, not absolute measures

---

## Future Improvements

* Incorporate real survey data
* Use transformer-based models (BERT, RoBERTa)
* Expand dataset for higher statistical robustness
* Add behavioral segmentation (user personas)

---

## Conclusion

This project demonstrates that:

* **Work environment is a critical driver of cognitive performance**
* There is clear dissatisfaction with current setups
* There is growing openness toward alternative work models

This creates a strong foundation for solutions like **ixa**, which aim to redesign work environments around **focus, clarity, and deep output**.

---
