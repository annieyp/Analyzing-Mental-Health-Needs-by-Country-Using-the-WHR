# Analyzing Mental Health Needs by Country Using WHR

This project uses the **World Happiness Report (WHR)** dataset to explore how socio-economic factors relate to **Negative Affect**, negative emotions experienced daily, with the goal of identifying potential mental health needs by country.  
Through **unsupervised machine learning (KMeans clustering)**, countries are grouped based on their happiness indicators, enabling targeted recommendations for mental health organizations.

---

## Dataset

The project uses the `WHR2018Chapter2OnlineData.csv` dataset, which contains:

- **GDP per capita**
- **Social Support**
- **Freedom to Make Life Choices**
- **Generosity**
- **Perceptions of Corruption**
- **Negative Affect** (our focal metric)

---

## Problem Definition

- **Type**: Unsupervised Learning → Clustering (KMeans)
- **Features**:
  - GDP
  - Freedom
  - Generosity
  - Perceptions of Corruption
  - Social Support
  - Negative Affect
- **Goal**: Identify relationships between **Negative Affect** and socio-economic indicators, enabling mental health-focused organizations to prioritize regions with higher needs.

---

## Methodology

1. **Data Exploration**
   - Inspected dataset structure
   - Checked missing values and distributions
   - Analyzed correlations between socio-economic factors and Negative Affect

2. **Preprocessing**
   - Selected relevant features
   - Scaled data for KMeans
   - Removed or imputed missing values

3. **Modeling**
   - Applied **KMeans clustering**
   - Determined optimal number of clusters using the Elbow Method
   - Interpreted clusters in the context of mental health needs

4. **Visualization**
   - Scatter plots and cluster maps
   - Cluster centers compared to global averages
   - Highlighting countries with highest Negative Affect

---

## Results

- Countries are segmented into distinct clusters representing varying **mental health risk profiles**
- Patterns observed:
  - Higher GDP does not always correlate with lower Negative Affect
  - Low social support and high perceptions of corruption tend to cluster with higher Negative Affect

---

## Applications

- **Mental Health NGOs**: Target interventions where socio-economic factors are high but still experience higher mental health needs
- **Policy Makers**: Allocate resources to improve social support and trust in institutions
- **Researchers**: Extend analysis with additional well-being or health datasets

---

## Tech Stack

- **Python**
- **Pandas**, **NumPy** for data manipulation
- **Scikit-learn** for clustering
- **Matplotlib**, **Seaborn** for visualizations

##License
- **This project is licensed under the MIT License — see the LICENSE file for details.**
