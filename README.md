# Recommendation-System-for-Retail-Stores
## Overview

The Retail Store Recommendation System is a collaborative filtering-based recommendation engine designed to provide personalized product recommendations to users based on their historical preferences and behaviors. This system uses the Surprise library with matrix factorization (SVD) to enhance recommendation accuracy.

## Features

- Collaborative filtering using SVD for accurate product recommendations.
- Integration of user and product data for a more personalized experience.
- Support for additional features such as product categories to enhance recommendation relevance.
- Easy-to-use interface for both users and developers.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Abhiruchi37/Recommendation-System-for-Retail-Stores.git
   cd Recommendation-System-for-Retail-Stores
   ```

2. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. Load your retail dataset into the appropriate file.

4. Run the recommendation system:

   ```bash
   jupyter notebook Recommendation_System_for_Retail_Stores.ipynb

   ```

## Dataset Format
Dataset link - https://www.kaggle.com/datasets/skillsmuggler/amazon-ratings \
The dataset includes the following columns:

- `User_ID`: Unique identifier for users.
- `Product_ID`: Unique identifier for products.
- `Rating`: User ratings for products (scale from 1 to 5).


## Usage

The system provides top N product recommendations for a specific user. To obtain recommendations, simply provide the user's ID as input.

Example usage:

```python
# Replace 'user_id' with the actual user ID
user_id = 'user_id'
user_recommendations = get_top_n_recommendations(predictions, n=5)[user_id]

print(f'Top 5 Recommendations for User {user_id}:')
for product_id, estimated_rating in user_recommendations:
    print(f'Product ID: {product_id}, Estimated Rating: {estimated_rating}')
```

## License

This project is licensed under the [MIT License](LICENSE).




