# Overview

In this notebook I demonstrate an embedding space visualisation technique for LLMs. Specifically, I chose the most compact model from the MTEB overall leaderboard at the time of making this notebook. The chosen model is Stella_en_400m. This model can be used to extract sentence level as well as docment level embeddings. For this demo I chose to visualise the models embedding space using sentences and words. In order to make the plots readable, I restricted myself to 15 sentences coming from 5 distinct sectors. Similarly I chose 50 words again from 5 distinct sectors. The sectors chosen were "data science", "finance", "sports", "healthcare" and "Technology". 

In our embedding visualizations, we should expect to see entries from closer sectors being closer to each other. We should also see entries from the same sectors to be the closets to each other.

A table has been included at the end of the page to compare and contrasts the different visualization techniques used.

# Sample Visualizations

![image](https://github.com/user-attachments/assets/cc82662c-b695-4906-ad5f-3d2da8dc20de)

![image](https://github.com/user-attachments/assets/e926e0c8-55a7-4231-a25c-6b2ca5b7de8c)

# Compare and Contrast Methods

| Feature | PCA | t-SNE | UMAP |
|---|---|---|---|
| Speciality | Global structure (variance) | Local structure (neighborhoods) | Both global and local structure |
| Speed | Fastest | Slowest | Middle |
| Scalability | Good | Limited | Good |
| Preservation of high dimensional structure | Global | Local | Both |
| Interpretability | Somewhat easy | Somewhat Difficut difficult | Moderate (easy if less entries) |
