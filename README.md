# Personalised_Recipe_Recommendation_System

# Overview
 This project implements a personalized recipe recommendation system using both
 content-based filtering and collaborative filtering techniques. The system is designed to
 recommend recipes based on user preferences, available ingredients, and additional constraints
 such as time and dietary restrictions.
 The recommendation system was built using a dataset containing recipe information, such as
 ingredients, tags, descriptions, ratings, and user interactions. The goal was to simulate
 real-world challenges in building AI/ML systems and demonstrate creative solutions for
 generating recommendations.
 Approach
 1. Data Preprocessing
 The first step was to preprocess the dataset for efficient use in recommendation algorithms. The
 following preprocessing steps were performed:
 - Combining Relevant Features: Textual features such as tags, ingredients, and
 description were concatenated to create a combined_features column for
 content-based filtering.
-  Handling Missing Values: Missing descriptions or tags were replaced with empty
 strings.
-  TF-IDF Vectorization: The combined_features column was transformed into a
 numerical representation using TF-IDF (Term Frequency-Inverse Document Frequency)
 to capture the importance of terms across recipes.
 2. Content-Based Filtering
 This approach leverages recipe features to recommend similar items. Key steps include:
 -  Computing cosine similarity between recipes based on their TF-IDF representations.
-  Foragiven input recipe, identifying the most similar recipes and returning the top
 recommendations.
 3. Collaborative Filtering
 Collaborative filtering uses user-item interaction data (e.g., ratings and reviews) to make
 recommendations. In this project:
 -  A user-item matrix was created with users as rows, recipes as columns, and ratings as
 values.
 -  Similarities between users were calculated to recommend recipes that similar users
 liked
