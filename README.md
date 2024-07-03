# Link-Prediction-in-Social-Networks

## Introduction

This project focuses on predicting the likelihood of new relationships forming between individuals in a social network. Using the publicly available Facebook egonets from SNAP datasets, we compare the performance of the state-of-the-art node2vec model with traditional similarity-based feature representation methods such as Common Neighbors, Jaccard Coefficient, Preferential Attachment, and Resource Allocation.

## Project Overview

### Objectives
- Predict if there is a link between two entities in a social network (Facebook).
- Compare the performance of node2vec with traditional similarity-based measures for link prediction.

### Methodology
1. **Data Representation**: The Facebook network is represented as a graph where each user is a node, and the relationship between them is a link.
2. **Feature Engineering**:
   - **Similarity-Based Measures**: Common Neighbors, Jaccard Coefficient, Adamic/Adar, Resource Allocation, Preferential Attachment.
   - **Node2vec**: Utilized for creating feature vectors.
3. **Model Training**: Logistic regression model trained on the generated feature vectors.
4. **Performance Metrics**: Accuracy and ROC_AUC score.

## Results
The performance of node2vec and similarity-based methods were evaluated using accuracy and ROC_AUC score.
AUC scores for Node2Vec:

![image](https://github.com/hari1016/Link-Prediction-in-Social-Networks/assets/63118506/96b21199-70f7-4ead-9259-1a5d8aef71b6)

AUC scores for similarity-based methods:

![image](https://github.com/hari1016/Link-Prediction-in-Social-Networks/assets/63118506/478302c8-ff75-477a-a966-f24651cf7896)

The results indicate a clear improvement in performance with Node2Vec as Node2Vec have far better AUC scores than all of the similarity measures.

Embedding plot from Node2vec algorithm:

![image](https://github.com/hari1016/Link-Prediction-in-Social-Networks/assets/63118506/7f670077-13cd-497b-9d33-8f4d5350c3f3)

## Conclusion:
This project demonstrates the application of both traditional and advanced methods for link prediction in social networks. The comparison reveals the strengths and weaknesses of each approach, providing insights for further research and development in the field.

