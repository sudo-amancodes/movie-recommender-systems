# Movie Recommendation Systems

## Overview

This project implements various recommendation algorithms using the MovieLens dataset to explore different approaches to movie recommendations. The implementation includes collaborative filtering techniques and graph-based random walk methods.

## Dataset

The project uses the MovieLens 100K dataset which contains:

- User ratings for movies (u.data)
- Movie information (u.item)
- User demographic information (u.user)

## Features

This project implements three main recommendation approaches:

1. **User-Based Collaborative Filtering**

   - Recommends movies based on similar users' preferences
   - Uses similarity metrics to find users with similar tastes

2. **Item-Based Collaborative Filtering**

   - Recommends movies similar to those a user has already liked
   - Calculates movie-to-movie similarity matrices

3. **Graph-Based Recommendations (Weighted Pixie)**
   - Implements a bipartite user-movie graph
   - Uses random walk algorithms to traverse the graph and discover recommendations
   - Weights recommendations based on visit frequency during random walks

## Files in the Repository

- `Movie_Recommendation.ipynb`: Jupyter notebook containing all code and explanations
- `users.csv`: Processed user demographic data
- `movies.csv`: Processed movie information
- `ratings.csv`: Processed user ratings
- `raw_data/`: Directory containing original dataset files:
  - `u.data`: User ratings
  - `u.item`: Movie information
  - `u.user`: User information

## Implementation Details

The project includes several key components:

- **Data Processing and Exploration**

  - Loading and cleaning the dataset
  - Handling missing values and inconsistencies
  - Converting timestamps to readable dates

- **Recommendation Algorithms**
  - User similarity calculation
  - Item similarity calculation
  - Bipartite graph construction
  - Random walk implementation

## Usage

To run this project:

1. Clone the repository
2. Ensure you have Python with required libraries installed:
   - pandas
   - numpy
   - sklearn
   - matplotlib
3. Open the Jupyter notebook:
   ```
   jupyter notebook Movie_Recommendation.ipynb
   ```
4. Run the cells to see the implementation and results

## Results

The project provides movie recommendations using different techniques and allows for comparison between methods. The random walk-based approach offers a novel recommendation mechanism that can discover unexpected but relevant movies.

## Future Improvements

Potential enhancements to the project:

- Implement hybrid recommendation models
- Add more features for content-based filtering
- Incorporate temporal dynamics in user preferences

## Course Information

This project was developed as part of ITCS 6162: Data Mining course.
