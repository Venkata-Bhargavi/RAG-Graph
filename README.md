# Knowledge Graph Based New Music Discovery and Recommendation System with LLMs and neo4j



## Introduction

The rapid growth of digital platforms has revolutionized how content is consumed, offering both opportunities and challenges. In this project, we aim to develop a recommendation system leveraging knowledge graphs and large language models (LLMs) on the Million Songs dataset to provide personalized music recommendations.

## Complex Data Representation

- Enhanced Querying and Analysis

## Team

- Krishna J (Building Knowledge Graph, Query Analysis)
- Bhargavi S (Feature Extraction from Audio, Tags generation using DL models)

  
## Dataset Insights

The dataset used for this project categorizes song attributes, metadata, and user interactions, facilitating personalized recommendations and enhancing music discovery on platforms like TikTok Spotify.


![image](https://github.com/user-attachments/assets/81e7e498-cce4-4baf-a68b-d621a8d1796e)


### Key Features

- **Song Attributes**: Danceability, Acousticness, Energy, etc.
- **Metadata**: Genre, Year, Artist, Likes, etc.
- **User Interactions**: Tags, User, Playcount, etc.

## Implementation Strategies

### Enhancing Recommendations with Knowledge Graphs

- **Graph Data Model for Music**: Represents relationships between songs, artists, genres, etc.
- **Semantic Relationships**: Enriches understanding of music attributes and interactions.
- **User-Centric Recommendations**: Tailors recommendations based on user preferences.

### Leveraging LLMs

- **Natural Language Understanding**: Process user queries to generate relevant recommendations.
- **Contextual Recommendations**: Use LLMs to understand user context and preferences for better recommendations.

### Knowledge Graph Nodes and Relationships

- **Nodes**: Song, Genre, Year, Artist, Likes, Tag, User, Danceability, Acousticness, Energy, Liveness, Tempo, Valence
- **Relationships**:
  - (:Song)-[:HAS_TAG]->(:Tag)
  - (:Song)-[:LISTENED_BY]->(:User)
  - (:Song)-[:PERFORMED_BY]->(:Artist)
  - (:Song)-[:HAS_DANCEABILITY]->(:Danceability)
  - (:Song)-[:HAS_ACOUSTICNESS]->(:Acousticness)
  - (:Song)-[:HAS_ENERGY]->(:Energy)
  - (:Song)-[:HAS_LIVENESS]->(:Liveness)
  - (:Song)-[:HAS_TEMPO]->(:Tempo)
  - (:Song)-[:HAS_VALENCE]->(:Valence)
  - (:Song)-[:RELEASED_IN]->(:Year)
  - (:Song)-[:HAS_GENRE]->(:Genre)
  - (:Song)-[:TOTAL_LIKES]->(:Likes)
  - (:Artist)-[:HAS_GENRE]->(:Genre)

## Evaluation Strategy

To evaluate the effectiveness of our recommendation system, we will use the following metrics:

- **Recommender System Metrics**:
  - Precision and Recall
  - F1 Score
  - Mean Average Precision (MAP)
  - Mean Reciprocal Rank (MRR)
  - Normalized Discounted Cumulative Gain (NDCG)

## Conclusion

This proposal outlines a strategy to develop a recommendation system that leverages advanced recommendation algorithms and knowledge graphs using LLMs and Neo4j. By focusing on personalized recommendations, the project aims to transform the way users interact with music on various platforms.

## Future Works

Future developments include integrating with external platforms, enhancing NLP capabilities, analyzing user interactions, ensuring scalability, and improving visualization tools.


