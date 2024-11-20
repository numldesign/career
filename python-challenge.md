### Task: Build a Real-Time Product Recommendation System

**Duration:** 3 hours

**Objective:** Assess the candidate's ability to design and implement a scalable real-time recommendation system for an e-commerce platform using Python, FastAPI, Celery, PostgreSQL, and machine learning techniques.

#### Task Breakdown

#### Part 1: Application Setup (30 minutes)

1. FastAPI Application:
  - Set up a FastAPI application with a well-structured project layout.
  - Configure necessary libraries such as FastAPI-SQLAlchemy for ORM and FastAPI-Cors for handling CORS issues.
2. Database Configuration:
  - Connect to PostgreSQL and create tables for users, products, orders, and user_product_interactions (to track user interactions with products).
  - Define relationships between tables.

#### Part 2: User Interaction Tracking (30 minutes)

1. Capture User Interactions:
  - Implement an API endpoint that logs user interactions with products (e.g., views, clicks, purchases).
  - Store these interactions in the user_product_interactions table.
2. Data Processing:
  - Create a background task using Celery that processes the interaction data periodically to update user profiles for recommendations.

#### Part 3: Recommendation Algorithm Implementation (1 hour)

1. Collaborative Filtering Algorithm:
  - Implement a simple collaborative filtering algorithm to generate product recommendations based on user interactions.
  - Use techniques such as cosine similarity or matrix factorization (e.g., SVD) to compute recommendations.
2. Real-Time Recommendations Endpoint:
  - Create an API endpoint that returns real-time product recommendations for a given user based on their interaction history.
  - Ensure that the recommendations are updated dynamically as new interactions are logged.

#### Part 4: Advanced Features and Testing (1 hour)

1. Integration with Machine Learning Model:
  - Integrate a pre-trained machine learning model (e.g., using scikit-learn or TensorFlow) that predicts user preferences based on historical data.
  - Allow the model to be retrained periodically using new interaction data.
2. Unit Testing and API Documentation:
  - Write unit tests for the recommendation logic and API endpoints using pytest.
  - Document the API endpoints using Swagger or Postman.
3. Serialization Methods:
  - Implement serialization of user interactions and recommendations using both pickle and JSON.
  - Demonstrate converting data from pickle format to JSON for API responses.

#### Evaluation Criteria

- Code Quality: Clarity, organization, adherence to Python best practices.
- Functionality: Completeness of features implemented within the time limit.
- Algorithm Understanding: Ability to explain and implement collaborative filtering concepts effectively.
- Real-Time Processing: Efficiency in handling real-time data updates for recommendations.
- Testing Rigor: Completeness and effectiveness of tests written.
- Creativity: Innovative approaches taken in implementing features or algorithms.

#### References for Implementation

- For guidance on building FastAPI applications:
  - [FastAPI Documentation](https://fastapi.tiangolo.com/)
- To understand how to set up Celery:
  - [Celery Documentation](https://docs.celeryq.dev/en/stable/index.html)
- For collaborative filtering algorithms:
  - [Introduction to Recommender Systems](https://towardsdatascience.com/introduction-to-recommender-systems-a-beginners-guide-8b5a6c8a7d0a)
- For machine learning with scikit-learn:
  - [Scikit-learn Documentation](https://scikit-learn.org/stable/)
