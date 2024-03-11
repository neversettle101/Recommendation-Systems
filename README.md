# Recommender System

## Types of Recommender Systems
- Popularity Based: Top ten most rated movies; based on some formula for rating

- Content Based
- Collaboratived Based

| Type                    | Definition                                                                    | Example                                                                                    |
|-------------------------|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| content-based filtering | Uses similarity between items to recommend items similar to what the user likes. | If user A watches two cute cat videos, then the system can recommend cute animal videos to that user. |
| collaborative filtering | Uses similarities between queries and items simultaneously to provide recommendations. | If user A is similar to user B, and user B likes video 1, then the system can recommend video 1 to user A (even if user A hasn’t seen any videos similar to video 1). |

- Collaborative Filtering: 
Matrix Factorization
It involved breaking down a large user-item interaction matrix into 2 smaller matrices - one representing users-feature and the other item-features.
    - Latent Factors:

        - User Matrix (U): This matrix represents users and their preferences for latent factors.

        - Item Matrix (V): This matrix represents movies and their characteristics in terms of latent factors.

    U*V contains the ratings given by all the users. This will be a sparse matrix as not all users have rated all items. 

    - Learning the Factors: MF algorithm learns the latent factors by minimzing the error between actual user-item interaction and predict interactions (U*V)

    - Recommendation Generation: Once the matrices are learned, predictions for missing user-item can be geenrated by dot product.

## References
- https://developers.google.com/machine-learning/recommendation
