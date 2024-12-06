ClusterBoost: An Airbnb Recommendation Engine Using Metaclustering

This repository contains the implementation of **ClusterBoost**, a recommendation engine designed to provide personalized Airbnb accommodation suggestions by leveraging advanced clustering techniques and ensemble models.

---

## Project Overview

### Objective:
To enhance Airbnb recommendations by overcoming limitations of existing systems such as cold-start problems, lack of scalability, and poor personalization.

### Features:
- **Meta-Clustering Approach**: Combines K-Means, DBSCAN, and Agglomerative Clustering for grouping similar listings.
- **Spectral Clustering**: Aggregates results from individual clustering methods to improve accuracy and diversity of recommendations.
- **Cosine Similarity**: Matches user preferences with Airbnb listings for personalized suggestions.
- **Evaluation Metrics**: Uses Silhouette Scores and Davies-Bouldin Index for performance assessment.

---

## Dataset

- **Source**: Kaggle Airbnb dataset.
- **Size**: ~39,000 listings.
- **Attributes**: Includes property details, host information, pricing, amenities, availability, and user reviews.

---

## Methodology

1. **Data Collection**:
   - Extract detailed listing information such as location, property type, amenities, and reviews.

2. **Preprocessing**:
   - Handle missing values and outliers.
   - Convert categorical data into numerical format for analysis.

3. **Clustering Techniques**:
   - **K-Means**: Effective for large datasets and spherical clusters.
   - **DBSCAN**: Handles clusters of varying densities and outliers.
   - **Agglomerative Clustering**: Provides a hierarchical structure for clusters.

4. **Ensemble Approach**:
   - Combine outputs of individual clustering algorithms using Spectral Clustering.

5. **Recommendation**:
   - Rank listings based on similarity to user preferences using Cosine Similarity.

6. **Evaluation**:
   - Assess clustering quality using Silhouette Scores and Davies-Bouldin Index.

---

## Results

### Key Metrics:
- **Silhouette Score**:
  - K-Means: 0.44574
  - DBSCAN: 0.50151
  - Agglomerative: 0.44574
  - **ClusterBoost (Proposed Model)**: **0.67355**
  
- **Davies-Bouldin Index**:
  - K-Means: 1.82827
  - DBSCAN: 0.689973
  - Agglomerative: 1.82827
  - **ClusterBoost (Proposed Model)**: **0.54912**

### Conclusion:
ClusterBoost demonstrated superior performance compared to individual clustering algorithms by providing well-separated and accurate clusters.

---


## Usage

1. Load your dataset or use the provided Airbnb dataset.
2. Preprocess the data using the script.
3. Apply clustering and generate recommendations.
4. Visualize and evaluate the results.

---

## Future Enhancements

1. **Temporal Analysis**: Incorporate seasonal trends and event-based patterns.
2. **Semantic Analysis**: Use NLP to analyze listing descriptions and user reviews.
3. **Graph-Based Recommendations**: Model relationships between users, listings, and features using graph algorithms.
4. **Interactive UI**: Add real-time feedback features for improved personalization.
5. **Integration of Emerging Technologies**:
   - AI/ML for advanced modeling.
   - Blockchain for secure transactions.
   - IoT for dynamic property updates.

---

## Contributors

- **Ari Nikhil Sai**
- **Vuyyuri Bhavani Chandra**
- **Ongole Gandhi**

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

