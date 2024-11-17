#### Overview ✨

The **LASTFM-Asia** repository contains machine learning applications for network analysis, focusing on user behavior and graph-based modeling. It includes two main parts, with detailed notebooks exploring different aspects of social network analysis and node classification using the LastFM dataset. 🧑‍💻📊

---

#### Files and Structure 📂

1. **[part1.ipynb](https://github.com/shaySitri/LASTFM-Asia/blob/main/part1.ipynb)**  
   - 📝 **Introduction to the LastFM dataset** and initial data analysis.  
   - Includes:
     - 📉 **Data filtering**: Removing nodes with a degree < 2.  
     - 📊 **Graph analysis**: Degree distribution, network density, clustering coefficient, and path length.  
     - 🎨 **Network visualization**: Using community detection (Louvain method) and Gephi for clear, colorful representations.  

2. **[part2.ipynb](https://github.com/shaySitri/LASTFM-Asia/blob/main/part2.ipynb)**  
   - 🚀 **Advanced ML tasks** for node classification by country.  
   - Features include:
     - 🛠️ **Preprocessing**: Stratified train-test split and JSON parsing for user artist data.  
     - 🔍 **Feature Engineering**:
       - **Artist-level** 🎧: One-hot encoding of top 1,000 artists and normalization.  
       - **Network Architecture** 🏗️: Degree centrality, eigenvector centrality, and community labels.  
       - **Country-level** 🌍: Neighbor country probabilities and artist distributions by neighbors.  
     - 🤖 **Modeling**: Random Forest with hyperparameter tuning via GridSearch.  
     - 🌐 **Node2Vec**: Incorporation of graph embeddings with various parameter settings.  
   - 📈 **Evaluation**: Metrics like accuracy, precision, recall, and F1-score.  

---

#### Key Insights 💡

- **🏆 Best Performing Features**:  
  - Architectural features (e.g., centrality measures) provided the most predictive power, achieving notable precision and accuracy.  

- **⚠️ Limitations**:  
  - Imbalanced data impacted the classification of nodes from smaller countries.  
  - Artist-based features alone were less effective due to the global popularity of top artists.  
  - Node2Vec embeddings did not consistently improve performance due to potential similarities between neighbors from different countries.  

---

#### Future Work 🔮

- 🔗 Exploring advanced embedding techniques like Graph Neural Networks (GNNs) for node classification.  
- ⚖️ Addressing data imbalance with oversampling or weighted loss functions.  
- 🧪 Evaluating the impact of combining artist-level and network-level features in more depth.  

